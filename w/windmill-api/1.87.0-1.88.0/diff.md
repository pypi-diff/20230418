# Comparing `tmp/windmill_api-1.87.0.tar.gz` & `tmp/windmill_api-1.88.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.87.0.tar", max compression
+gzip compressed data, was "windmill_api-1.88.0.tar", max compression
```

## Comparing `windmill_api-1.87.0.tar` & `windmill_api-1.88.0.tar`

### file list

```diff
@@ -1,1241 +1,1267 @@
--rw-r--r--   0        0        0    11348 2023-04-11 19:13:28.384709 windmill_api-1.87.0/LICENSE
--rw-r--r--   0        0        0     2952 2023-04-11 19:13:28.388709 windmill_api-1.87.0/README.md
--rw-r--r--   0        0        0      717 2023-04-11 19:13:28.384709 windmill_api-1.87.0/pyproject.toml
--rw-r--r--   0        0        0      100 2023-04-11 19:12:48.844307 windmill_api-1.87.0/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-04-11 19:12:49.536314 windmill_api-1.87.0/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.688316 windmill_api-1.87.0/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-04-11 19:13:01.724438 windmill_api-1.87.0/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-04-11 19:13:01.732438 windmill_api-1.87.0/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-04-11 19:13:01.780439 windmill_api-1.87.0/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-04-11 19:13:01.780439 windmill_api-1.87.0/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-04-11 19:13:01.836439 windmill_api-1.87.0/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3031 2023-04-11 19:13:01.832439 windmill_api-1.87.0/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-04-11 19:13:01.896440 windmill_api-1.87.0/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-04-11 19:13:01.888440 windmill_api-1.87.0/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-04-11 19:13:01.936440 windmill_api-1.87.0/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-04-11 19:13:02.024441 windmill_api-1.87.0/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-04-11 19:13:01.984440 windmill_api-1.87.0/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-04-11 19:13:02.024441 windmill_api-1.87.0/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.588315 windmill_api-1.87.0/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-04-11 19:13:02.076441 windmill_api-1.87.0/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-04-11 19:13:02.164442 windmill_api-1.87.0/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.756316 windmill_api-1.87.0/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-11 19:13:02.108442 windmill_api-1.87.0/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-04-11 19:13:02.144442 windmill_api-1.87.0/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-04-11 19:13:02.180442 windmill_api-1.87.0/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.756316 windmill_api-1.87.0/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-04-11 19:13:02.204443 windmill_api-1.87.0/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-04-11 19:13:02.216443 windmill_api-1.87.0/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.680316 windmill_api-1.87.0/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     1789 2023-04-11 19:13:02.244443 windmill_api-1.87.0/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-04-11 19:13:02.252443 windmill_api-1.87.0/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-04-11 19:13:02.280444 windmill_api-1.87.0/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-04-11 19:13:02.304444 windmill_api-1.87.0/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-04-11 19:13:02.328444 windmill_api-1.87.0/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     2667 2023-04-11 19:13:02.360444 windmill_api-1.87.0/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-04-11 19:13:02.380445 windmill_api-1.87.0/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-04-11 19:13:02.480445 windmill_api-1.87.0/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-04-11 19:13:02.424445 windmill_api-1.87.0/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-04-11 19:13:02.464445 windmill_api-1.87.0/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.744316 windmill_api-1.87.0/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-04-11 19:13:02.504446 windmill_api-1.87.0/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-04-11 19:13:02.516446 windmill_api-1.87.0/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-04-11 19:13:02.544446 windmill_api-1.87.0/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-04-11 19:13:02.568446 windmill_api-1.87.0/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-04-11 19:13:02.596447 windmill_api-1.87.0/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-04-11 19:13:02.628447 windmill_api-1.87.0/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-04-11 19:13:02.668448 windmill_api-1.87.0/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-04-11 19:13:02.664447 windmill_api-1.87.0/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-04-11 19:13:02.704448 windmill_api-1.87.0/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.752316 windmill_api-1.87.0/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-04-11 19:13:02.720448 windmill_api-1.87.0/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-04-11 19:13:02.788449 windmill_api-1.87.0/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-04-11 19:13:02.764449 windmill_api-1.87.0/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.736316 windmill_api-1.87.0/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-04-11 19:13:02.824449 windmill_api-1.87.0/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-04-11 19:13:02.824449 windmill_api-1.87.0/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-04-11 19:13:02.860449 windmill_api-1.87.0/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-04-11 19:13:02.872449 windmill_api-1.87.0/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-04-11 19:13:02.920450 windmill_api-1.87.0/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-04-11 19:13:02.944450 windmill_api-1.87.0/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-04-11 19:13:02.960451 windmill_api-1.87.0/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-04-11 19:13:02.984451 windmill_api-1.87.0/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.696316 windmill_api-1.87.0/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-04-11 19:13:03.004451 windmill_api-1.87.0/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-04-11 19:13:03.036451 windmill_api-1.87.0/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-04-11 19:13:03.072452 windmill_api-1.87.0/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-04-11 19:13:03.084452 windmill_api-1.87.0/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-04-11 19:13:03.128452 windmill_api-1.87.0/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-04-11 19:13:03.120452 windmill_api-1.87.0/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-04-11 19:13:03.176453 windmill_api-1.87.0/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-04-11 19:13:03.164452 windmill_api-1.87.0/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-04-11 19:13:03.220453 windmill_api-1.87.0/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-04-11 19:13:03.272454 windmill_api-1.87.0/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-04-11 19:13:03.316454 windmill_api-1.87.0/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-04-11 19:13:03.344454 windmill_api-1.87.0/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    12602 2023-04-11 19:13:03.492456 windmill_api-1.87.0/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    11829 2023-04-11 19:13:03.520456 windmill_api-1.87.0/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12367 2023-04-11 19:13:03.680458 windmill_api-1.87.0/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-04-11 19:13:03.560457 windmill_api-1.87.0/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-04-11 19:13:03.596457 windmill_api-1.87.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2994 2023-04-11 19:13:03.652458 windmill_api-1.87.0/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-04-11 19:13:03.728458 windmill_api-1.87.0/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-04-11 19:13:03.780459 windmill_api-1.87.0/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-04-11 19:13:03.780459 windmill_api-1.87.0/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-04-11 19:13:03.856459 windmill_api-1.87.0/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-04-11 19:13:03.848460 windmill_api-1.87.0/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-04-11 19:13:03.904460 windmill_api-1.87.0/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     3215 2023-04-11 19:13:03.912460 windmill_api-1.87.0/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     3521 2023-04-11 19:13:03.964461 windmill_api-1.87.0/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0     3356 2023-04-11 19:13:03.972461 windmill_api-1.87.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.632315 windmill_api-1.87.0/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-11 19:13:04.016461 windmill_api-1.87.0/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-04-11 19:13:04.008461 windmill_api-1.87.0/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-04-11 19:13:04.044461 windmill_api-1.87.0/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-04-11 19:13:04.052461 windmill_api-1.87.0/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-04-11 19:13:04.080462 windmill_api-1.87.0/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-04-11 19:13:04.088462 windmill_api-1.87.0/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-04-11 19:13:04.132462 windmill_api-1.87.0/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-04-11 19:13:04.128462 windmill_api-1.87.0/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.636315 windmill_api-1.87.0/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-11 19:13:04.180463 windmill_api-1.87.0/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-04-11 19:13:04.168463 windmill_api-1.87.0/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-04-11 19:13:04.204463 windmill_api-1.87.0/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-04-11 19:13:04.216463 windmill_api-1.87.0/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-04-11 19:13:04.276464 windmill_api-1.87.0/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-04-11 19:13:04.268464 windmill_api-1.87.0/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-04-11 19:13:04.324464 windmill_api-1.87.0/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-04-11 19:13:04.324464 windmill_api-1.87.0/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-04-11 19:13:04.360465 windmill_api-1.87.0/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-04-11 19:13:04.420465 windmill_api-1.87.0/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-04-11 19:13:04.420465 windmill_api-1.87.0/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-04-11 19:13:04.472466 windmill_api-1.87.0/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-04-11 19:13:04.460466 windmill_api-1.87.0/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-04-11 19:13:04.504466 windmill_api-1.87.0/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-04-11 19:13:04.512466 windmill_api-1.87.0/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.728316 windmill_api-1.87.0/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-11 19:13:04.548467 windmill_api-1.87.0/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-04-11 19:13:04.548467 windmill_api-1.87.0/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-04-11 19:13:04.596467 windmill_api-1.87.0/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-04-11 19:13:04.612467 windmill_api-1.87.0/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-04-11 19:13:04.688468 windmill_api-1.87.0/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-04-11 19:13:04.672468 windmill_api-1.87.0/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-04-11 19:13:04.712468 windmill_api-1.87.0/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-04-11 19:13:04.728469 windmill_api-1.87.0/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.660315 windmill_api-1.87.0/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-04-11 19:13:04.768469 windmill_api-1.87.0/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-04-11 19:13:04.764469 windmill_api-1.87.0/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-04-11 19:13:04.812469 windmill_api-1.87.0/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-04-11 19:13:04.804469 windmill_api-1.87.0/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-04-11 19:13:04.860470 windmill_api-1.87.0/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-04-11 19:13:04.860470 windmill_api-1.87.0/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-04-11 19:13:04.912470 windmill_api-1.87.0/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-04-11 19:13:04.928470 windmill_api-1.87.0/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-04-11 19:13:04.960471 windmill_api-1.87.0/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-04-11 19:13:04.968471 windmill_api-1.87.0/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-04-11 19:13:05.016471 windmill_api-1.87.0/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-04-11 19:13:05.020471 windmill_api-1.87.0/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3276 2023-04-11 19:13:05.088472 windmill_api-1.87.0/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-04-11 19:13:05.068472 windmill_api-1.87.0/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-04-11 19:13:05.124472 windmill_api-1.87.0/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-04-11 19:13:05.124472 windmill_api-1.87.0/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-04-11 19:13:05.316474 windmill_api-1.87.0/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-04-11 19:13:05.180473 windmill_api-1.87.0/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-04-11 19:13:05.216473 windmill_api-1.87.0/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-04-11 19:13:05.252474 windmill_api-1.87.0/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0     2119 2023-04-11 19:13:05.292474 windmill_api-1.87.0/windmill_api/api/script/raw_script_by_path_tokened.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.552314 windmill_api-1.87.0/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-11 19:13:05.332475 windmill_api-1.87.0/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-04-11 19:13:05.352475 windmill_api-1.87.0/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.592315 windmill_api-1.87.0/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-04-11 19:13:05.372475 windmill_api-1.87.0/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-04-11 19:13:05.384475 windmill_api-1.87.0/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     1991 2023-04-11 19:13:05.412475 windmill_api-1.87.0/windmill_api/api/user/create_token_impersonate.py
--rw-r--r--   0        0        0     2058 2023-04-11 19:13:05.424476 windmill_api-1.87.0/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-04-11 19:13:05.448476 windmill_api-1.87.0/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-04-11 19:13:05.460476 windmill_api-1.87.0/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-04-11 19:13:05.488476 windmill_api-1.87.0/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-04-11 19:13:05.496476 windmill_api-1.87.0/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-04-11 19:13:05.520476 windmill_api-1.87.0/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-04-11 19:13:05.548477 windmill_api-1.87.0/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-04-11 19:13:05.556477 windmill_api-1.87.0/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-04-11 19:13:05.588477 windmill_api-1.87.0/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-04-11 19:13:05.620478 windmill_api-1.87.0/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-04-11 19:13:05.640478 windmill_api-1.87.0/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-04-11 19:13:05.656478 windmill_api-1.87.0/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-04-11 19:13:05.688478 windmill_api-1.87.0/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-04-11 19:13:05.708478 windmill_api-1.87.0/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-04-11 19:13:05.744479 windmill_api-1.87.0/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-04-11 19:13:05.784479 windmill_api-1.87.0/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-04-11 19:13:05.792479 windmill_api-1.87.0/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-04-11 19:13:05.820479 windmill_api-1.87.0/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-04-11 19:13:05.828480 windmill_api-1.87.0/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-04-11 19:13:05.856480 windmill_api-1.87.0/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-04-11 19:13:05.864480 windmill_api-1.87.0/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-04-11 19:13:05.900480 windmill_api-1.87.0/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-04-11 19:13:05.916480 windmill_api-1.87.0/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-04-11 19:13:05.956481 windmill_api-1.87.0/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.624315 windmill_api-1.87.0/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-11 19:13:05.976481 windmill_api-1.87.0/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-04-11 19:13:05.996481 windmill_api-1.87.0/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-04-11 19:13:06.028482 windmill_api-1.87.0/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-04-11 19:13:06.080482 windmill_api-1.87.0/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-04-11 19:13:06.084482 windmill_api-1.87.0/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-04-11 19:13:06.136483 windmill_api-1.87.0/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-04-11 19:13:06.132483 windmill_api-1.87.0/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.752316 windmill_api-1.87.0/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     3896 2023-04-11 19:13:06.204483 windmill_api-1.87.0/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-04-11 19:12:49.612315 windmill_api-1.87.0/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-04-11 19:13:06.176483 windmill_api-1.87.0/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-04-11 19:13:06.212484 windmill_api-1.87.0/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-04-11 19:13:06.240484 windmill_api-1.87.0/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-04-11 19:13:06.252484 windmill_api-1.87.0/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-04-11 19:13:06.272484 windmill_api-1.87.0/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-04-11 19:13:06.292484 windmill_api-1.87.0/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-04-11 19:13:06.312485 windmill_api-1.87.0/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-04-11 19:13:06.332485 windmill_api-1.87.0/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-04-11 19:13:06.344485 windmill_api-1.87.0/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-04-11 19:13:06.368485 windmill_api-1.87.0/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-04-11 19:13:06.392485 windmill_api-1.87.0/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-04-11 19:13:06.440486 windmill_api-1.87.0/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-04-11 19:13:06.424486 windmill_api-1.87.0/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-04-11 19:13:06.464486 windmill_api-1.87.0/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-04-11 19:13:06.492486 windmill_api-1.87.0/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-04-11 19:13:06.520487 windmill_api-1.87.0/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-04-11 19:13:06.544487 windmill_api-1.87.0/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-04-11 19:13:06.588487 windmill_api-1.87.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-04-11 19:13:06.580487 windmill_api-1.87.0/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-04-11 19:13:06.620488 windmill_api-1.87.0/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-04-11 19:13:28.376709 windmill_api-1.87.0/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-04-11 19:13:06.652488 windmill_api-1.87.0/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-04-11 19:13:06.688488 windmill_api-1.87.0/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      301 2023-04-11 19:13:00.616427 windmill_api-1.87.0/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-04-11 19:13:06.724489 windmill_api-1.87.0/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-04-11 19:13:06.772489 windmill_api-1.87.0/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-04-11 19:13:06.776489 windmill_api-1.87.0/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-04-11 19:13:06.840490 windmill_api-1.87.0/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-04-11 19:13:00.512426 windmill_api-1.87.0/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-04-11 19:13:06.804489 windmill_api-1.87.0/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-04-11 19:13:06.884490 windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-04-11 19:12:59.828419 windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-04-11 19:13:06.880490 windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-04-11 19:13:06.908491 windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     6879 2023-04-11 19:13:06.992491 windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-04-11 19:13:06.952491 windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-04-11 19:13:00.080421 windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-04-11 19:13:00.664427 windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-04-11 19:13:06.984491 windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-04-11 19:13:07.056492 windmill_api-1.87.0/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-04-11 19:12:59.984420 windmill_api-1.87.0/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-04-11 19:12:59.864419 windmill_api-1.87.0/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-04-11 19:13:07.024492 windmill_api-1.87.0/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-04-11 19:13:07.072492 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-04-11 19:13:07.144493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-04-11 19:12:59.944420 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-04-11 19:13:07.104493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-04-11 19:13:07.136493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-04-11 19:13:07.172493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-04-11 19:13:07.196493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-04-11 19:12:59.692417 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-04-11 19:13:07.200493 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-04-11 19:13:07.248494 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-04-11 19:13:00.556426 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-04-11 19:13:07.232494 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-04-11 19:12:59.648417 windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-04-11 19:13:07.276494 windmill_api-1.87.0/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-04-11 19:13:07.296495 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-04-11 19:13:07.392495 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-04-11 19:13:07.348495 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-04-11 19:13:07.384495 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-11 19:13:07.444496 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-11 19:13:07.428496 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-11 19:13:00.096421 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-11 19:13:07.460496 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-11 19:13:00.228423 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-11 19:13:07.488496 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-11 19:13:07.504497 windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-04-11 19:13:00.932430 windmill_api-1.87.0/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-04-11 19:13:07.540497 windmill_api-1.87.0/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-04-11 19:13:07.556497 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-04-11 19:13:07.652498 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-04-11 19:13:07.604498 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-04-11 19:13:07.640498 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-11 19:13:07.684498 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-11 19:13:07.692499 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-11 19:12:59.984420 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-11 19:13:07.720499 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-11 19:13:00.780428 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-11 19:13:07.744499 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-11 19:13:07.756499 windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-04-11 19:13:07.844500 windmill_api-1.87.0/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-04-11 19:13:07.824500 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-04-11 19:13:07.860500 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-04-11 19:13:07.892500 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-04-11 19:13:07.896501 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-04-11 19:13:00.420425 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-04-11 19:13:07.956501 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-04-11 19:12:59.816419 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-04-11 19:13:07.932501 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-04-11 19:13:07.972501 windmill_api-1.87.0/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-04-11 19:13:00.328424 windmill_api-1.87.0/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-04-11 19:13:07.996502 windmill_api-1.87.0/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-04-11 19:13:08.000502 windmill_api-1.87.0/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10376 2023-04-11 19:13:08.180503 windmill_api-1.87.0/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-04-11 19:13:08.024502 windmill_api-1.87.0/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-04-11 19:13:08.084503 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-04-11 19:13:08.192504 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-04-11 19:13:08.216504 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-04-11 19:13:08.232504 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-04-11 19:13:00.580426 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-04-11 19:13:08.256504 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-04-11 19:13:08.276504 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-04-11 19:13:00.072421 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-04-11 19:13:08.368505 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-04-11 19:13:08.324505 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-04-11 19:13:08.360505 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-04-11 19:13:00.644427 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-04-11 19:13:08.396506 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-04-11 19:13:08.420506 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-04-11 19:13:00.084421 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-04-11 19:13:08.444506 windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-04-11 19:13:00.016420 windmill_api-1.87.0/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-04-11 19:13:00.128422 windmill_api-1.87.0/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-04-11 19:13:08.512507 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-04-11 19:13:08.544507 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-04-11 19:13:08.564507 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-04-11 19:13:08.580508 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-11 19:13:08.608508 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-11 19:13:08.620508 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-11 19:13:00.320424 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-11 19:13:08.648508 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-11 19:13:00.936430 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-11 19:13:08.656508 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-11 19:13:08.688509 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-04-11 19:13:08.788510 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-04-11 19:13:08.744509 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-04-11 19:13:08.780510 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-04-11 19:13:08.832510 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-04-11 19:13:08.824510 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-04-11 19:13:00.904430 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-04-11 19:13:08.860510 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-04-11 19:12:59.860419 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-04-11 19:13:08.872511 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-04-11 19:13:08.896511 windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-04-11 19:13:08.908511 windmill_api-1.87.0/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-04-11 19:13:08.948511 windmill_api-1.87.0/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-04-11 19:13:08.944511 windmill_api-1.87.0/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-04-11 19:13:09.012512 windmill_api-1.87.0/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-04-11 19:13:08.992512 windmill_api-1.87.0/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2035 2023-04-11 19:13:09.036512 windmill_api-1.87.0/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-04-11 19:13:09.076513 windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-04-11 19:13:00.200422 windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-04-11 19:13:09.072512 windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-04-11 19:13:09.104513 windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-04-11 19:13:09.144513 windmill_api-1.87.0/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-04-11 19:13:09.132513 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-04-11 19:13:09.188514 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-04-11 19:13:09.260514 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-04-11 19:13:09.248514 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-04-11 19:13:09.308515 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-04-11 19:13:09.304515 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-04-11 19:13:09.344515 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-04-11 19:13:00.240423 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-04-11 19:13:09.348515 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-04-11 19:13:00.896429 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-04-11 19:13:09.388516 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-04-11 19:13:09.396516 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-04-11 19:13:09.524517 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-04-11 19:13:09.452516 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-04-11 19:13:09.492517 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-04-11 19:13:09.540517 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-04-11 19:13:09.560517 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-04-11 19:13:00.348424 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-04-11 19:13:09.584518 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-04-11 19:13:00.488425 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-04-11 19:13:09.600518 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-04-11 19:13:09.624518 windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2126 2023-04-11 19:13:09.652518 windmill_api-1.87.0/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-04-11 19:13:09.660519 windmill_api-1.87.0/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     2094 2023-04-11 19:13:09.696519 windmill_api-1.87.0/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-04-11 19:13:09.704519 windmill_api-1.87.0/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-04-11 19:13:09.744519 windmill_api-1.87.0/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2780 2023-04-11 19:13:09.756519 windmill_api-1.87.0/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-04-11 19:13:09.768519 windmill_api-1.87.0/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     4616 2023-04-11 19:13:09.872521 windmill_api-1.87.0/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-04-11 19:13:00.320424 windmill_api-1.87.0/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-04-11 19:13:00.004420 windmill_api-1.87.0/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-04-11 19:13:09.800520 windmill_api-1.87.0/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2534 2023-04-11 19:13:09.848520 windmill_api-1.87.0/windmill_api/models/create_token_impersonate_json_body.py
--rw-r--r--   0        0        0     2169 2023-04-11 19:13:09.892521 windmill_api-1.87.0/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-04-11 19:13:09.920521 windmill_api-1.87.0/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-04-11 19:13:09.932521 windmill_api-1.87.0/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-04-11 19:13:09.976522 windmill_api-1.87.0/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-04-11 19:13:10.012522 windmill_api-1.87.0/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-04-11 19:13:10.020522 windmill_api-1.87.0/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-04-11 19:13:10.048522 windmill_api-1.87.0/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-04-11 19:13:10.052523 windmill_api-1.87.0/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    10978 2023-04-11 19:13:10.224524 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-04-11 19:13:10.080523 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-04-11 19:13:10.140523 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-04-11 19:13:10.256525 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-04-11 19:13:10.260525 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-04-11 19:13:10.296525 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-04-11 19:12:59.828419 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-04-11 19:13:10.296525 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-04-11 19:13:10.392526 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-04-11 19:13:00.764428 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-04-11 19:13:10.412526 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-04-11 19:13:10.428526 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-04-11 19:13:10.460527 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-04-11 19:13:00.704428 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-04-11 19:13:10.468527 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-04-11 19:13:10.540527 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-04-11 19:13:00.968430 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-04-11 19:13:10.512527 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-04-11 19:13:00.912430 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-04-11 19:13:00.948430 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-04-11 19:13:10.576528 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-04-11 19:13:10.648528 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-04-11 19:13:10.628528 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-04-11 19:13:10.668529 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-04-11 19:13:10.692529 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-04-11 19:13:10.732529 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-04-11 19:12:59.764418 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-11 19:13:10.744530 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-04-11 19:13:00.576426 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-04-11 19:13:10.772530 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-04-11 19:13:10.780530 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-04-11 19:13:10.908531 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-04-11 19:13:10.832530 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-04-11 19:13:10.872531 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-04-11 19:13:10.912531 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-04-11 19:13:10.948531 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-04-11 19:12:59.868419 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-04-11 19:13:10.952532 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-04-11 19:13:00.456425 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-04-11 19:13:10.992532 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-04-11 19:13:11.012532 windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-04-11 19:13:11.032533 windmill_api-1.87.0/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     6853 2023-04-11 19:13:11.116533 windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-04-11 19:13:11.068533 windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-04-11 19:13:00.520426 windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-04-11 19:13:00.852429 windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-04-11 19:13:11.100533 windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-04-11 19:13:11.152534 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-04-11 19:13:11.196534 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-04-11 19:13:00.176422 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-04-11 19:13:11.188534 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-04-11 19:13:11.228534 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-04-11 19:13:11.232535 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-04-11 19:13:11.276535 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-04-11 19:12:59.812419 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-04-11 19:13:11.268535 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-04-11 19:13:11.320535 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-04-11 19:13:00.252423 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-04-11 19:13:11.312535 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-04-11 19:13:00.384424 windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-04-11 19:13:11.348536 windmill_api-1.87.0/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-04-11 19:13:11.368536 windmill_api-1.87.0/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-04-11 19:13:11.408536 windmill_api-1.87.0/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1845 2023-04-11 19:13:11.408536 windmill_api-1.87.0/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-04-11 19:13:11.436537 windmill_api-1.87.0/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-04-11 19:13:11.440537 windmill_api-1.87.0/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-04-11 19:13:11.512537 windmill_api-1.87.0/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-04-11 19:13:11.476537 windmill_api-1.87.0/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-04-11 19:13:11.516537 windmill_api-1.87.0/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-04-11 19:13:11.576538 windmill_api-1.87.0/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-04-11 19:13:11.544538 windmill_api-1.87.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-04-11 19:13:11.588538 windmill_api-1.87.0/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-04-11 19:13:11.612538 windmill_api-1.87.0/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-04-11 19:13:11.616538 windmill_api-1.87.0/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4633 2023-04-11 19:13:11.696539 windmill_api-1.87.0/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-04-11 19:13:11.644539 windmill_api-1.87.0/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3416 2023-04-11 19:13:11.708539 windmill_api-1.87.0/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-04-11 19:13:11.724539 windmill_api-1.87.0/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-04-11 19:13:11.828540 windmill_api-1.87.0/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-04-11 19:13:11.776540 windmill_api-1.87.0/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-04-11 19:13:11.812540 windmill_api-1.87.0/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-04-11 19:13:11.852541 windmill_api-1.87.0/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-04-11 19:13:11.864541 windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-04-11 19:12:59.880419 windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-04-11 19:13:11.900541 windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-04-11 19:12:59.884419 windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-04-11 19:13:11.936542 windmill_api-1.87.0/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-04-11 19:13:11.944542 windmill_api-1.87.0/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3080 2023-04-11 19:13:11.992542 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-04-11 19:13:12.036543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-11 19:13:12.032543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-11 19:12:59.804418 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-11 19:13:12.076543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-11 19:12:59.820418 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-04-11 19:13:00.584426 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-04-11 19:13:00.200422 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-04-11 19:13:12.088543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-04-11 19:13:12.128543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-11 19:13:12.128543 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-11 19:12:59.816419 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-11 19:13:12.164544 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-11 19:13:00.200422 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-04-11 19:13:00.104421 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-04-11 19:13:12.176544 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-04-11 19:13:12.216544 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-11 19:13:12.216544 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-11 19:13:00.828429 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-11 19:13:12.252545 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-11 19:13:00.992431 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-04-11 19:13:00.508426 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-04-11 19:13:12.288545 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-04-11 19:13:12.288545 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-04-11 19:12:59.892419 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-04-11 19:13:12.324545 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-04-11 19:13:00.944430 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-04-11 19:13:12.396546 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-04-11 19:13:12.376546 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-04-11 19:13:12.412546 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-04-11 19:13:12.472547 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-04-11 19:13:12.452547 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-11 19:13:00.080421 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-04-11 19:13:12.488547 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-11 19:13:00.736428 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-04-11 19:13:12.508547 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-04-11 19:13:12.552548 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-04-11 19:12:59.828419 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-04-11 19:13:12.560548 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-04-11 19:13:12.600548 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-04-11 19:13:12.676549 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-04-11 19:13:12.652549 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-04-11 19:13:12.692549 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-04-11 19:13:12.724550 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-04-11 19:13:12.728550 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-11 19:13:00.248423 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-04-11 19:13:12.760550 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-11 19:13:00.560426 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-04-11 19:13:12.768550 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-04-11 19:13:12.804551 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-04-11 19:13:12.872551 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-04-11 19:13:12.860551 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-04-11 19:13:12.900551 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-04-11 19:13:12.916552 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-04-11 19:13:12.980552 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-11 19:12:59.804418 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-04-11 19:13:12.952552 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-11 19:13:00.416425 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-04-11 19:13:13.032553 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-04-11 19:13:13.020553 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-04-11 19:13:00.740428 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-04-11 19:13:13.072553 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-04-11 19:13:13.080553 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-04-11 19:13:13.204554 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-04-11 19:13:13.132554 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-04-11 19:13:13.172554 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-04-11 19:13:13.216555 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-04-11 19:13:13.244555 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-11 19:13:00.952430 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-04-11 19:13:13.252555 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-11 19:13:00.140422 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-04-11 19:13:13.284555 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-04-11 19:13:13.292555 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-04-11 19:13:00.616427 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-04-11 19:13:13.324556 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-04-11 19:13:00.416425 windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-04-11 19:13:13.336556 windmill_api-1.87.0/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-04-11 19:13:13.356556 windmill_api-1.87.0/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-04-11 19:13:13.392557 windmill_api-1.87.0/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-04-11 19:13:13.512558 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-04-11 19:13:13.440557 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-04-11 19:13:13.480557 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-04-11 19:13:13.552558 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-04-11 19:13:13.556558 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-11 19:13:00.196422 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-04-11 19:13:13.588558 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-11 19:13:00.144422 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-04-11 19:13:13.604559 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-04-11 19:13:13.628559 windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-04-11 19:13:13.716560 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-04-11 19:13:13.680559 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-04-11 19:13:13.720560 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-04-11 19:13:13.764560 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-04-11 19:13:13.756560 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-04-11 19:13:00.740428 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-04-11 19:13:13.796561 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-04-11 19:13:00.204422 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-04-11 19:13:13.808561 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-04-11 19:13:13.836561 windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-04-11 19:13:13.840561 windmill_api-1.87.0/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-04-11 19:13:13.892562 windmill_api-1.87.0/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-04-11 19:13:13.960562 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-04-11 19:13:13.928562 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-04-11 19:13:13.964562 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-04-11 19:13:00.088421 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-04-11 19:13:14.032563 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-04-11 19:13:14.016563 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-04-11 19:12:59.804418 windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-04-11 19:13:14.176564 windmill_api-1.87.0/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-04-11 19:13:14.064563 windmill_api-1.87.0/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-04-11 19:13:14.104564 windmill_api-1.87.0/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-04-11 19:13:00.156422 windmill_api-1.87.0/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-04-11 19:13:14.140564 windmill_api-1.87.0/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-04-11 19:13:14.188564 windmill_api-1.87.0/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-04-11 19:13:00.748428 windmill_api-1.87.0/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-04-11 19:13:14.288565 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-04-11 19:13:14.224565 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-04-11 19:13:14.264565 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-04-11 19:12:59.924419 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-04-11 19:13:14.304566 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-04-11 19:13:14.336566 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-04-11 19:12:59.928420 windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-04-11 19:13:14.348566 windmill_api-1.87.0/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-04-11 19:13:14.388567 windmill_api-1.87.0/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-04-11 19:13:14.452567 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-04-11 19:13:14.440567 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-04-11 19:13:14.476567 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-04-11 19:13:14.496568 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-04-11 19:13:14.516568 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-04-11 19:12:59.940420 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-04-11 19:13:14.568568 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-04-11 19:13:00.128422 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-04-11 19:13:14.600569 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-04-11 19:13:14.604569 windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-04-11 19:13:14.712570 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-04-11 19:13:14.656569 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-04-11 19:13:14.696570 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-04-11 19:13:14.740570 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-04-11 19:13:14.760570 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-04-11 19:13:00.996430 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-04-11 19:13:14.784571 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-04-11 19:13:00.280423 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-04-11 19:13:14.800571 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-04-11 19:13:14.824571 windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-04-11 19:13:14.840571 windmill_api-1.87.0/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-04-11 19:13:14.852571 windmill_api-1.87.0/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-04-11 19:13:14.872572 windmill_api-1.87.0/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-04-11 19:13:14.920572 windmill_api-1.87.0/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-04-11 19:13:14.908572 windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-04-11 19:13:00.528426 windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-04-11 19:13:14.944572 windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-04-11 19:13:00.056421 windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-04-11 19:13:15.072574 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-04-11 19:13:14.996573 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-04-11 19:13:15.036573 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-04-11 19:13:15.116574 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-04-11 19:13:15.112574 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-04-11 19:13:00.612427 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-04-11 19:13:15.148574 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-04-11 19:12:59.820418 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-04-11 19:13:15.156574 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-04-11 19:13:15.188575 windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-04-11 19:12:59.720418 windmill_api-1.87.0/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-04-11 19:13:15.232575 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-04-11 19:13:00.416425 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-04-11 19:13:15.216575 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-04-11 19:13:15.288576 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-04-11 19:13:00.100421 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-04-11 19:13:15.264575 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-04-11 19:13:15.292576 windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-04-11 19:13:15.360576 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-04-11 19:13:00.800428 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-04-11 19:13:15.320576 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-04-11 19:13:15.384577 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-04-11 19:13:00.672427 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-04-11 19:13:15.396577 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-04-11 19:13:15.408577 windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-04-11 19:13:15.468577 windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-04-11 19:13:00.132422 windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-04-11 19:13:00.000420 windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-04-11 19:13:15.444577 windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    10876 2023-04-11 19:13:15.704580 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-04-11 19:13:15.492578 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-04-11 19:13:15.616579 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-04-11 19:13:15.740580 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-04-11 19:13:15.736580 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-04-11 19:13:15.784581 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-04-11 19:13:00.472425 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-04-11 19:13:15.780581 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-04-11 19:13:15.824581 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-04-11 19:13:00.180422 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-04-11 19:13:15.956582 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-04-11 19:13:15.864581 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-04-11 19:13:15.904582 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-04-11 19:13:00.424425 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-04-11 19:13:15.948582 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-04-11 19:13:16.000583 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-04-11 19:12:59.636417 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-04-11 19:13:16.000583 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-04-11 19:13:00.960430 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-04-11 19:13:00.784428 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-04-11 19:13:16.056584 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-04-11 19:13:16.160585 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-04-11 19:13:16.108584 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-04-11 19:13:16.148584 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-04-11 19:13:16.192585 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-04-11 19:13:16.204585 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-04-11 19:13:00.092421 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-04-11 19:13:16.276586 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-04-11 19:13:00.804428 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-04-11 19:13:16.244585 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-04-11 19:13:16.280586 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-04-11 19:13:16.388587 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-04-11 19:13:16.336586 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-04-11 19:13:16.372587 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-04-11 19:13:16.416587 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-04-11 19:13:16.428587 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-11 19:12:59.676417 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-04-11 19:13:16.456588 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-11 19:13:00.456425 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-04-11 19:13:16.476588 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-04-11 19:13:16.496588 windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5083 2023-04-11 19:13:16.568589 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-04-11 19:13:16.524588 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-04-11 19:13:16.548588 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-04-11 19:13:16.604589 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-04-11 19:13:16.680590 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-04-11 19:13:16.656590 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-04-11 19:13:16.692590 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-04-11 19:13:16.724590 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-04-11 19:13:16.792591 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-11 19:13:00.132422 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-04-11 19:13:16.828591 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-11 19:12:59.936420 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-04-11 19:13:16.832591 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-04-11 19:13:16.868592 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-04-11 19:13:16.940592 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-04-11 19:13:16.924592 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-04-11 19:13:16.964593 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-04-11 19:13:16.984593 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-04-11 19:13:17.008593 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-11 19:13:00.196422 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-04-11 19:13:17.024593 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-11 19:13:00.636427 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-04-11 19:13:17.048594 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-04-11 19:13:17.060594 windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2010 2023-04-11 19:13:17.096594 windmill_api-1.87.0/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-04-11 19:13:17.088594 windmill_api-1.87.0/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-04-11 19:13:17.136594 windmill_api-1.87.0/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      301 2023-04-11 19:12:59.956420 windmill_api-1.87.0/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-04-11 19:13:17.128594 windmill_api-1.87.0/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-04-11 19:13:17.192595 windmill_api-1.87.0/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-04-11 19:13:17.160595 windmill_api-1.87.0/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-04-11 19:13:17.192595 windmill_api-1.87.0/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-04-11 19:13:17.228595 windmill_api-1.87.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-04-11 19:13:17.236595 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-04-11 19:13:17.280596 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-04-11 19:13:17.320596 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-04-11 19:13:17.384597 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-04-11 19:13:17.432597 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-04-11 19:13:17.452598 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-04-11 19:13:17.472598 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-04-11 19:13:17.488598 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-04-11 19:13:17.512598 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-04-11 19:13:00.204422 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-04-11 19:13:17.528598 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-04-11 19:12:59.980420 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-04-11 19:13:17.552599 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-04-11 19:13:17.568599 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-04-11 19:13:17.664600 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-04-11 19:13:17.620599 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-04-11 19:13:17.660600 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-04-11 19:13:17.704600 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-04-11 19:13:17.700600 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-04-11 19:13:00.212422 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-04-11 19:13:17.740601 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-04-11 19:13:00.376424 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-04-11 19:13:17.752601 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-04-11 19:13:17.828601 windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-04-11 19:13:17.804601 windmill_api-1.87.0/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-04-11 19:12:59.776418 windmill_api-1.87.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1852 2023-04-11 19:13:17.844602 windmill_api-1.87.0/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-04-11 19:13:00.728428 windmill_api-1.87.0/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-04-11 19:13:17.876602 windmill_api-1.87.0/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-04-11 19:13:17.884602 windmill_api-1.87.0/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-04-11 19:13:17.944603 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-04-11 19:13:00.428425 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-04-11 19:13:17.908602 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-04-11 19:13:18.016603 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-04-11 19:12:59.824419 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-04-11 19:13:17.984603 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-04-11 19:13:18.008603 windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-04-11 19:13:18.076604 windmill_api-1.87.0/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-04-11 19:13:18.044604 windmill_api-1.87.0/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-04-11 19:13:18.100604 windmill_api-1.87.0/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-04-11 19:13:18.116604 windmill_api-1.87.0/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4325 2023-04-11 19:13:18.180605 windmill_api-1.87.0/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-04-11 19:13:18.140605 windmill_api-1.87.0/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-04-11 19:13:18.164605 windmill_api-1.87.0/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     6775 2023-04-11 19:13:18.272606 windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-04-11 19:13:18.204605 windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-11 19:13:00.428425 windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-04-11 19:12:59.812419 windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-04-11 19:13:18.232606 windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     6775 2023-04-11 19:13:18.332607 windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-04-11 19:13:18.340607 windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-11 19:13:00.196422 windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-04-11 19:13:00.804428 windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-04-11 19:13:18.360607 windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-04-11 19:13:18.376607 windmill_api-1.87.0/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-04-11 19:13:18.432608 windmill_api-1.87.0/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-04-11 19:13:18.420607 windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-04-11 19:13:18.452608 windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-04-11 19:13:18.472608 windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-04-11 19:12:59.812419 windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-04-11 19:13:18.592609 windmill_api-1.87.0/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-04-11 19:13:18.500608 windmill_api-1.87.0/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-04-11 19:13:18.548609 windmill_api-1.87.0/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-04-11 19:12:59.848419 windmill_api-1.87.0/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-04-11 19:13:18.584609 windmill_api-1.87.0/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-04-11 19:13:18.636610 windmill_api-1.87.0/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-04-11 19:12:59.760418 windmill_api-1.87.0/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-04-11 19:13:18.644610 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-04-11 19:13:18.724611 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-04-11 19:13:00.104421 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-04-11 19:13:18.680610 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-04-11 19:13:18.716611 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-04-11 19:13:18.760611 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-04-11 19:13:18.780611 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-04-11 19:13:00.572426 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-04-11 19:13:18.804611 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-04-11 19:13:18.880612 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-04-11 19:13:00.580426 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-04-11 19:13:18.840612 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-04-11 19:12:59.736418 windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-04-11 19:13:18.900612 windmill_api-1.87.0/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-04-11 19:13:18.908612 windmill_api-1.87.0/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-04-11 19:13:18.940613 windmill_api-1.87.0/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-04-11 19:13:00.540426 windmill_api-1.87.0/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     1820 2023-04-11 19:13:18.956613 windmill_api-1.87.0/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-04-11 19:13:00.396424 windmill_api-1.87.0/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-04-11 19:13:18.980613 windmill_api-1.87.0/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-04-11 19:13:00.276423 windmill_api-1.87.0/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-04-11 19:13:18.992613 windmill_api-1.87.0/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-04-11 19:13:19.020614 windmill_api-1.87.0/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-04-11 19:13:00.988430 windmill_api-1.87.0/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-04-11 19:13:19.032614 windmill_api-1.87.0/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-04-11 19:13:00.176422 windmill_api-1.87.0/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-04-11 19:13:19.128615 windmill_api-1.87.0/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-04-11 19:12:59.896419 windmill_api-1.87.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-04-11 19:13:19.068614 windmill_api-1.87.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-04-11 19:13:00.056421 windmill_api-1.87.0/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-04-11 19:13:19.136615 windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-04-11 19:13:00.616427 windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-04-11 19:13:00.608427 windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-04-11 19:13:19.160615 windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11088 2023-04-11 19:13:19.316617 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-04-11 19:13:19.188615 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-04-11 19:13:19.248616 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-04-11 19:13:19.412618 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-04-11 19:13:19.352617 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-04-11 19:13:19.392617 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-04-11 19:12:59.944420 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-04-11 19:13:19.432618 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-04-11 19:13:19.460618 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-04-11 19:13:00.108421 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-04-11 19:13:19.556619 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-04-11 19:13:19.492618 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-04-11 19:13:19.532619 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-04-11 19:13:00.448425 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-04-11 19:13:19.564619 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-04-11 19:13:19.604620 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-04-11 19:13:00.956430 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-04-11 19:13:19.604620 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-04-11 19:12:59.756418 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-04-11 19:13:00.112422 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-04-11 19:13:19.708621 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-04-11 19:13:19.712621 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-04-11 19:13:19.764621 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-04-11 19:13:19.744621 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-04-11 19:13:19.784621 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-04-11 19:13:19.804622 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-04-11 19:13:00.816429 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-04-11 19:13:19.820622 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-04-11 19:13:00.212422 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-04-11 19:13:19.840622 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-04-11 19:13:19.856622 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-04-11 19:13:19.956623 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-04-11 19:13:19.908623 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-04-11 19:13:19.992623 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-04-11 19:13:20.000624 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-04-11 19:13:20.028624 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-04-11 19:13:00.480425 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-04-11 19:13:20.036624 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-04-11 19:13:00.596426 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-04-11 19:13:20.072624 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-04-11 19:13:20.072624 windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-04-11 19:13:20.108625 windmill_api-1.87.0/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     5077 2023-04-11 19:13:20.196626 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-04-11 19:13:20.136625 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     1255 2023-04-11 19:13:20.164625 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_schema.py
--rw-r--r--   0        0        0     3297 2023-04-11 19:13:20.228626 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value.py
--rw-r--r--   0        0        0     7151 2023-04-11 19:13:20.308627 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py
--rw-r--r--   0        0        0     3318 2023-04-11 19:13:20.280626 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py
--rw-r--r--   0        0        0     1985 2023-04-11 19:13:20.316627 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2289 2023-04-11 19:13:20.364627 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2187 2023-04-11 19:13:20.356627 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-11 19:12:59.652417 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2054 2023-04-11 19:13:20.392628 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-11 19:13:00.012421 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1978 2023-04-11 19:13:20.408628 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2029 2023-04-11 19:13:20.428628 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7049 2023-04-11 19:13:20.508629 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py
--rw-r--r--   0        0        0     3284 2023-04-11 19:13:20.476628 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py
--rw-r--r--   0        0        0     1975 2023-04-11 19:13:20.512629 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-04-11 19:13:20.548629 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-04-11 19:13:20.592630 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-11 19:13:00.696427 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-04-11 19:13:20.584629 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-11 19:13:00.836429 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-04-11 19:13:20.664630 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-04-11 19:13:20.628630 windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2074 2023-04-11 19:13:20.664630 windmill_api-1.87.0/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-04-11 19:13:20.688630 windmill_api-1.87.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-04-11 19:13:20.724631 windmill_api-1.87.0/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-04-11 19:13:20.716631 windmill_api-1.87.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-04-11 19:13:20.760631 windmill_api-1.87.0/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-04-11 19:13:20.784632 windmill_api-1.87.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-04-11 19:13:20.812632 windmill_api-1.87.0/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-04-11 19:13:20.836632 windmill_api-1.87.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-04-11 19:13:20.856632 windmill_api-1.87.0/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-04-11 19:13:20.888633 windmill_api-1.87.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-04-11 19:13:00.376424 windmill_api-1.87.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     1922 2023-04-11 19:13:20.896633 windmill_api-1.87.0/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-04-11 19:12:59.908419 windmill_api-1.87.0/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-04-11 19:13:20.936633 windmill_api-1.87.0/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    11982 2023-04-11 19:13:21.104635 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-04-11 19:13:20.964633 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-04-11 19:13:21.024634 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-04-11 19:13:21.196636 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-04-11 19:13:21.188636 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-04-11 19:13:21.224636 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-04-11 19:13:00.728428 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-04-11 19:13:21.232636 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-04-11 19:13:21.276636 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-04-11 19:12:59.904420 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-04-11 19:13:21.340637 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-04-11 19:13:21.304637 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-04-11 19:13:21.340637 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-04-11 19:12:59.908419 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-04-11 19:13:21.384638 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-04-11 19:13:21.388638 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-04-11 19:13:00.740428 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-04-11 19:13:21.424638 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-04-11 19:12:59.640417 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-04-11 19:13:00.420425 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-04-11 19:13:21.448638 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-04-11 19:13:21.532639 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-04-11 19:13:21.500639 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-04-11 19:13:21.540639 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-04-11 19:13:21.572640 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-04-11 19:13:21.576640 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-11 19:13:00.376424 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-04-11 19:13:21.608640 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-11 19:13:00.660427 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-04-11 19:13:21.612640 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-04-11 19:13:21.700641 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-04-11 19:13:21.792642 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-04-11 19:13:21.748641 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-04-11 19:13:21.788642 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-04-11 19:13:21.828642 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-04-11 19:13:21.836642 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-11 19:12:59.640417 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-04-11 19:13:21.868642 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-11 19:13:00.168422 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-04-11 19:13:21.872643 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-04-11 19:13:21.904643 windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     4884 2023-04-11 19:13:21.960643 windmill_api-1.87.0/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-04-11 19:13:21.928643 windmill_api-1.87.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-04-11 19:13:21.976644 windmill_api-1.87.0/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4426 2023-04-11 19:13:22.052644 windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-04-11 19:13:22.004644 windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-04-11 19:13:22.032644 windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     6768 2023-04-11 19:13:22.148645 windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-04-11 19:13:22.080645 windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-11 19:13:00.580426 windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-04-11 19:12:59.848419 windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-04-11 19:13:22.108645 windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-04-11 19:13:22.164646 windmill_api-1.87.0/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-04-11 19:13:22.188646 windmill_api-1.87.0/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-04-11 19:13:22.264647 windmill_api-1.87.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-04-11 19:13:22.240646 windmill_api-1.87.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-04-11 19:13:00.240423 windmill_api-1.87.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4035 2023-04-11 19:13:22.360648 windmill_api-1.87.0/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-04-11 19:13:22.296647 windmill_api-1.87.0/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-04-11 19:13:22.372648 windmill_api-1.87.0/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-04-11 19:13:22.388648 windmill_api-1.87.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-04-11 19:13:22.416648 windmill_api-1.87.0/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-04-11 19:13:22.424648 windmill_api-1.87.0/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-04-11 19:13:22.456648 windmill_api-1.87.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-04-11 19:13:22.464649 windmill_api-1.87.0/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-04-11 19:13:22.516649 windmill_api-1.87.0/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-04-11 19:12:59.640417 windmill_api-1.87.0/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-04-11 19:13:22.488649 windmill_api-1.87.0/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-04-11 19:13:22.580650 windmill_api-1.87.0/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-04-11 19:13:22.536649 windmill_api-1.87.0/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-04-11 19:13:22.620650 windmill_api-1.87.0/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-04-11 19:13:22.604650 windmill_api-1.87.0/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-04-11 19:13:22.644650 windmill_api-1.87.0/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-04-11 19:13:22.664651 windmill_api-1.87.0/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-04-11 19:13:22.688651 windmill_api-1.87.0/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-04-11 19:13:22.720651 windmill_api-1.87.0/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-04-11 19:13:22.824652 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-04-11 19:13:00.860429 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-04-11 19:13:22.752652 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-04-11 19:13:22.844653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-04-11 19:13:22.860653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-04-11 19:13:22.896653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-04-11 19:12:59.724418 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-04-11 19:13:22.892653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-04-11 19:13:22.940653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-04-11 19:13:00.748428 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-04-11 19:13:22.928653 windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-04-11 19:13:00.904430 windmill_api-1.87.0/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2662 2023-04-11 19:13:22.984654 windmill_api-1.87.0/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-04-11 19:13:22.968654 windmill_api-1.87.0/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     2108 2023-04-11 19:13:23.016654 windmill_api-1.87.0/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     2473 2023-04-11 19:13:23.032654 windmill_api-1.87.0/windmill_api/models/new_token_impersonate.py
--rw-r--r--   0        0        0     1710 2023-04-11 19:13:23.052655 windmill_api-1.87.0/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-04-11 19:13:23.084655 windmill_api-1.87.0/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-04-11 19:13:23.084655 windmill_api-1.87.0/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-04-11 19:13:23.136655 windmill_api-1.87.0/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-04-11 19:13:23.192656 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-04-11 19:13:23.188656 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-04-11 19:13:23.228656 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-04-11 19:13:23.236657 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-04-11 19:13:23.268657 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-04-11 19:13:00.392424 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-04-11 19:13:23.272657 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-04-11 19:13:00.776428 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-04-11 19:13:23.304657 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-04-11 19:13:23.380658 windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-04-11 19:13:23.412658 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-04-11 19:13:23.440658 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-04-11 19:13:23.452659 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-04-11 19:13:23.484659 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-04-11 19:13:23.540660 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-04-11 19:13:00.088421 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-04-11 19:13:23.524659 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-04-11 19:13:00.952430 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-04-11 19:13:23.564660 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-04-11 19:13:23.576660 windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-04-11 19:13:23.624660 windmill_api-1.87.0/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-04-11 19:13:23.604660 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-04-11 19:13:23.656661 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-04-11 19:13:23.728661 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-04-11 19:13:23.708661 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-04-11 19:13:23.748662 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-04-11 19:13:23.776662 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-04-11 19:13:23.788662 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-04-11 19:13:00.444425 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-04-11 19:13:23.812662 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-04-11 19:12:59.952420 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-04-11 19:13:23.824662 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-04-11 19:13:23.852663 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-04-11 19:13:23.932664 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-04-11 19:13:23.976664 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-04-11 19:13:23.968664 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-04-11 19:13:24.012664 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-04-11 19:13:24.016664 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-11 19:13:00.784428 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-04-11 19:13:24.052665 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-11 19:12:59.696417 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-04-11 19:13:24.060665 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-04-11 19:13:24.100665 windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-04-11 19:13:24.100665 windmill_api-1.87.0/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-04-11 19:13:24.148666 windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-04-11 19:13:24.140666 windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-04-11 19:13:00.512426 windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-04-11 19:13:24.240667 windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-04-11 19:13:00.428425 windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-04-11 19:13:00.044421 windmill_api-1.87.0/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-04-11 19:13:24.200666 windmill_api-1.87.0/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-04-11 19:13:24.264667 windmill_api-1.87.0/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-04-11 19:13:24.280667 windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-04-11 19:13:00.008421 windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-04-11 19:13:24.304667 windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-04-11 19:12:59.812419 windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-04-11 19:13:00.100421 windmill_api-1.87.0/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-04-11 19:13:24.344668 windmill_api-1.87.0/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-04-11 19:13:00.168422 windmill_api-1.87.0/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-04-11 19:13:24.344668 windmill_api-1.87.0/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-04-11 19:13:24.368668 windmill_api-1.87.0/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2147 2023-04-11 19:13:24.388668 windmill_api-1.87.0/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-04-11 19:13:24.396668 windmill_api-1.87.0/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-04-11 19:12:59.928420 windmill_api-1.87.0/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1642 2023-04-11 19:13:24.428669 windmill_api-1.87.0/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-04-11 19:13:24.448669 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-04-11 19:13:24.512669 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-04-11 19:13:00.792428 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-04-11 19:13:24.488669 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-04-11 19:13:24.524670 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-04-11 19:13:24.556670 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-04-11 19:13:24.572670 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-04-11 19:12:59.996420 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-04-11 19:13:24.592670 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-04-11 19:13:24.620670 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-04-11 19:12:59.640417 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-04-11 19:13:24.628671 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-04-11 19:13:00.704428 windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11448 2023-04-11 19:13:24.892673 windmill_api-1.87.0/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-04-11 19:13:24.660671 windmill_api-1.87.0/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-04-11 19:13:24.724671 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-04-11 19:13:24.832673 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-04-11 19:13:24.932674 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-04-11 19:13:24.932674 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-04-11 19:13:00.164422 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-04-11 19:13:24.968674 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-04-11 19:13:24.980674 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-04-11 19:13:00.132422 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-04-11 19:13:25.076675 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-04-11 19:13:25.012674 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-04-11 19:13:25.052675 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-04-11 19:13:00.256423 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-04-11 19:13:25.088675 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-04-11 19:13:25.124676 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-04-11 19:13:00.180422 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-04-11 19:13:25.136676 windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-04-11 19:12:59.632417 windmill_api-1.87.0/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-04-11 19:13:00.772428 windmill_api-1.87.0/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-04-11 19:13:25.184676 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-04-11 19:13:25.320678 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-04-11 19:13:25.236677 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-04-11 19:13:25.272677 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-04-11 19:13:25.316677 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-04-11 19:13:25.356678 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-11 19:13:00.324424 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-04-11 19:13:25.356678 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-11 19:13:00.348424 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-04-11 19:13:25.396678 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-04-11 19:13:25.460679 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-04-11 19:13:25.504680 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-04-11 19:13:25.512679 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-04-11 19:13:25.544680 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-04-11 19:13:25.556680 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-04-11 19:13:25.584680 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-04-11 19:13:00.264423 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-04-11 19:13:25.592680 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-04-11 19:12:59.776418 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-04-11 19:13:25.628681 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-04-11 19:13:25.632681 windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-04-11 19:13:25.684681 windmill_api-1.87.0/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-04-11 19:13:25.676681 windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-04-11 19:13:25.712682 windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-04-11 19:12:59.732418 windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-04-11 19:13:25.720682 windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-04-11 19:13:00.956430 windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-04-11 19:12:59.888419 windmill_api-1.87.0/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-04-11 19:13:00.680427 windmill_api-1.87.0/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-04-11 19:13:25.748682 windmill_api-1.87.0/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-04-11 19:13:25.752682 windmill_api-1.87.0/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      304 2023-04-11 19:13:00.896429 windmill_api-1.87.0/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-04-11 19:13:25.784682 windmill_api-1.87.0/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-04-11 19:13:25.784682 windmill_api-1.87.0/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-04-11 19:13:25.848683 windmill_api-1.87.0/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-04-11 19:13:25.812682 windmill_api-1.87.0/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-04-11 19:13:25.864683 windmill_api-1.87.0/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-04-11 19:13:25.876683 windmill_api-1.87.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-04-11 19:13:25.892683 windmill_api-1.87.0/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-04-11 19:13:25.928684 windmill_api-1.87.0/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-04-11 19:13:25.932684 windmill_api-1.87.0/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-04-11 19:13:25.972684 windmill_api-1.87.0/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-04-11 19:13:25.960684 windmill_api-1.87.0/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-04-11 19:13:26.000685 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-04-11 19:13:26.000685 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-04-11 19:13:26.140686 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-04-11 19:13:26.224687 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-04-11 19:13:26.192686 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-04-11 19:13:26.232687 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-04-11 19:13:26.264687 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-04-11 19:13:26.276687 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-11 19:13:00.628427 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-04-11 19:13:26.304688 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-11 19:13:00.272423 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-04-11 19:13:26.316688 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-04-11 19:13:26.344688 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-04-11 19:13:26.424689 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-04-11 19:13:26.400689 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-04-11 19:13:26.436689 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-04-11 19:13:26.464689 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-04-11 19:13:26.468689 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-04-11 19:12:59.824419 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-04-11 19:13:26.500690 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-04-11 19:13:00.776428 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-04-11 19:13:26.508690 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-04-11 19:13:26.540690 windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-04-11 19:13:26.532690 windmill_api-1.87.0/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-04-11 19:13:26.560690 windmill_api-1.87.0/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2422 2023-04-11 19:13:26.584690 windmill_api-1.87.0/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-04-11 19:13:26.588690 windmill_api-1.87.0/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-04-11 19:13:00.104421 windmill_api-1.87.0/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-04-11 19:13:26.612691 windmill_api-1.87.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-04-11 19:13:26.612691 windmill_api-1.87.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0     4086 2023-04-11 19:13:26.776692 windmill_api-1.87.0/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-04-11 19:13:26.640691 windmill_api-1.87.0/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-04-11 19:13:26.668691 windmill_api-1.87.0/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     6220 2023-04-11 19:13:26.892694 windmill_api-1.87.0/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-04-11 19:13:26.812693 windmill_api-1.87.0/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-04-11 19:13:26.836693 windmill_api-1.87.0/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-04-11 19:12:59.820418 windmill_api-1.87.0/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-04-11 19:13:00.224423 windmill_api-1.87.0/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-04-11 19:13:26.868693 windmill_api-1.87.0/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-04-11 19:13:26.900694 windmill_api-1.87.0/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-04-11 19:13:26.924694 windmill_api-1.87.0/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-04-11 19:13:26.948694 windmill_api-1.87.0/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-04-11 19:13:26.956694 windmill_api-1.87.0/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-04-11 19:13:26.992694 windmill_api-1.87.0/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      185 2023-04-11 19:13:00.432425 windmill_api-1.87.0/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-04-11 19:13:26.996695 windmill_api-1.87.0/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-04-11 19:12:59.660417 windmill_api-1.87.0/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-04-11 19:13:27.048695 windmill_api-1.87.0/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-04-11 19:13:27.052695 windmill_api-1.87.0/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-04-11 19:13:27.092696 windmill_api-1.87.0/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      187 2023-04-11 19:13:00.056421 windmill_api-1.87.0/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-04-11 19:13:27.112696 windmill_api-1.87.0/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-04-11 19:13:27.156696 windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-04-11 19:13:00.144422 windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-04-11 19:13:27.148696 windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-04-11 19:13:27.176696 windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-04-11 19:13:27.212697 windmill_api-1.87.0/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-04-11 19:13:27.204697 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-04-11 19:13:27.260697 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-04-11 19:13:27.320698 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-04-11 19:13:27.316698 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-04-11 19:13:27.352698 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-04-11 19:13:27.364698 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-04-11 19:13:27.388699 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-04-11 19:13:00.960430 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-04-11 19:13:27.400699 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-04-11 19:13:00.468425 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-04-11 19:13:27.428699 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-04-11 19:13:27.508700 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-04-11 19:13:27.632701 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-04-11 19:13:27.564700 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-04-11 19:13:27.604701 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-04-11 19:13:27.648701 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-04-11 19:13:27.672701 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-04-11 19:13:00.240423 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-04-11 19:13:27.684702 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-04-11 19:12:59.704417 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-04-11 19:13:27.708702 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-04-11 19:13:27.720702 windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-04-11 19:13:27.752702 windmill_api-1.87.0/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-04-11 19:13:27.756702 windmill_api-1.87.0/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     2036 2023-04-11 19:13:27.800703 windmill_api-1.87.0/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-04-11 19:13:27.796703 windmill_api-1.87.0/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-04-11 19:13:27.828703 windmill_api-1.87.0/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1953 2023-04-11 19:13:27.840703 windmill_api-1.87.0/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-04-11 19:13:27.856703 windmill_api-1.87.0/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-04-11 19:13:27.892704 windmill_api-1.87.0/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-04-11 19:13:27.904704 windmill_api-1.87.0/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-04-11 19:13:27.924704 windmill_api-1.87.0/windmill_api/models/usage.py
--rw-r--r--   0        0        0     3799 2023-04-11 19:13:27.996705 windmill_api-1.87.0/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-04-11 19:13:27.968705 windmill_api-1.87.0/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-04-11 19:13:28.008705 windmill_api-1.87.0/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-04-11 19:13:28.032705 windmill_api-1.87.0/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     3950 2023-04-11 19:13:28.092706 windmill_api-1.87.0/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-04-11 19:13:28.068705 windmill_api-1.87.0/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     3939 2023-04-11 19:13:28.140706 windmill_api-1.87.0/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-04-11 19:13:28.124706 windmill_api-1.87.0/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-04-11 19:13:28.176707 windmill_api-1.87.0/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-04-11 19:13:28.184707 windmill_api-1.87.0/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-04-11 19:13:28.216707 windmill_api-1.87.0/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-04-11 19:12:48.844307 windmill_api-1.87.0/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-04-11 19:13:28.204707 windmill_api-1.87.0/windmill_api/types.py
--rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 windmill_api-1.87.0/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.87.0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-04-17 22:56:14.350781 windmill_api-1.88.0/LICENSE
+-rw-r--r--   0        0        0     2952 2023-04-17 22:56:14.354781 windmill_api-1.88.0/README.md
+-rw-r--r--   0        0        0      717 2023-04-17 22:56:14.354781 windmill_api-1.88.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-04-17 22:55:41.926713 windmill_api-1.88.0/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-17 22:55:42.398714 windmill_api-1.88.0/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.502714 windmill_api-1.88.0/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-04-17 22:55:53.074740 windmill_api-1.88.0/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-04-17 22:55:53.086740 windmill_api-1.88.0/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-04-17 22:55:53.106740 windmill_api-1.88.0/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-04-17 22:55:53.134740 windmill_api-1.88.0/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-04-17 22:55:53.146740 windmill_api-1.88.0/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3031 2023-04-17 22:55:53.178740 windmill_api-1.88.0/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-04-17 22:55:53.182740 windmill_api-1.88.0/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-04-17 22:55:53.234740 windmill_api-1.88.0/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-04-17 22:55:53.222740 windmill_api-1.88.0/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-04-17 22:55:53.314740 windmill_api-1.88.0/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-04-17 22:55:53.266740 windmill_api-1.88.0/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-04-17 22:55:53.298740 windmill_api-1.88.0/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.438714 windmill_api-1.88.0/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-04-17 22:55:53.342740 windmill_api-1.88.0/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-04-17 22:55:53.426741 windmill_api-1.88.0/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.550714 windmill_api-1.88.0/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-17 22:55:53.374740 windmill_api-1.88.0/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-04-17 22:55:53.406741 windmill_api-1.88.0/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-04-17 22:55:53.434741 windmill_api-1.88.0/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.554714 windmill_api-1.88.0/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-04-17 22:55:53.454741 windmill_api-1.88.0/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-04-17 22:55:53.466741 windmill_api-1.88.0/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.494714 windmill_api-1.88.0/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     2220 2023-04-17 22:55:53.486741 windmill_api-1.88.0/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-04-17 22:55:53.498741 windmill_api-1.88.0/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-04-17 22:55:53.514741 windmill_api-1.88.0/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-04-17 22:55:53.542741 windmill_api-1.88.0/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-04-17 22:55:53.578741 windmill_api-1.88.0/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     4827 2023-04-17 22:55:53.622741 windmill_api-1.88.0/windmill_api/api/flow/get_flow_input_history_by_path.py
+-rw-r--r--   0        0        0     2667 2023-04-17 22:55:53.614741 windmill_api-1.88.0/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-04-17 22:55:53.638741 windmill_api-1.88.0/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-04-17 22:55:53.726741 windmill_api-1.88.0/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-04-17 22:55:53.674741 windmill_api-1.88.0/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-04-17 22:55:53.702741 windmill_api-1.88.0/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.542714 windmill_api-1.88.0/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-04-17 22:55:53.734741 windmill_api-1.88.0/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-04-17 22:55:53.758741 windmill_api-1.88.0/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-04-17 22:55:53.762741 windmill_api-1.88.0/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-04-17 22:55:53.802741 windmill_api-1.88.0/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-04-17 22:55:53.802741 windmill_api-1.88.0/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-04-17 22:55:53.854742 windmill_api-1.88.0/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-04-17 22:55:53.862742 windmill_api-1.88.0/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-04-17 22:55:53.886742 windmill_api-1.88.0/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-04-17 22:55:53.894742 windmill_api-1.88.0/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.550714 windmill_api-1.88.0/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-04-17 22:55:53.922742 windmill_api-1.88.0/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-04-17 22:55:53.954742 windmill_api-1.88.0/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-04-17 22:55:53.966742 windmill_api-1.88.0/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.538714 windmill_api-1.88.0/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-04-17 22:55:53.986742 windmill_api-1.88.0/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-04-17 22:55:54.022742 windmill_api-1.88.0/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-04-17 22:55:54.014742 windmill_api-1.88.0/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-04-17 22:55:54.054742 windmill_api-1.88.0/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-04-17 22:55:54.074742 windmill_api-1.88.0/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-04-17 22:55:54.110742 windmill_api-1.88.0/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-04-17 22:55:54.106742 windmill_api-1.88.0/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-04-17 22:55:54.142742 windmill_api-1.88.0/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.554714 windmill_api-1.88.0/windmill_api/api/input_/__init__.py
+-rw-r--r--   0        0        0     3338 2023-04-17 22:55:54.154742 windmill_api-1.88.0/windmill_api/api/input_/create_input.py
+-rw-r--r--   0        0        0     1811 2023-04-17 22:55:54.170742 windmill_api-1.88.0/windmill_api/api/input_/delete_input.py
+-rw-r--r--   0        0        0     6187 2023-04-17 22:55:54.230743 windmill_api-1.88.0/windmill_api/api/input_/get_input_history.py
+-rw-r--r--   0        0        0     6010 2023-04-17 22:55:54.246743 windmill_api-1.88.0/windmill_api/api/input_/list_inputs.py
+-rw-r--r--   0        0        0     2025 2023-04-17 22:55:54.278743 windmill_api-1.88.0/windmill_api/api/input_/update_input.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.510714 windmill_api-1.88.0/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-04-17 22:55:54.282743 windmill_api-1.88.0/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-04-17 22:55:54.318743 windmill_api-1.88.0/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-04-17 22:55:54.326743 windmill_api-1.88.0/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-04-17 22:55:54.354743 windmill_api-1.88.0/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-04-17 22:55:54.390743 windmill_api-1.88.0/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-04-17 22:55:54.386743 windmill_api-1.88.0/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-04-17 22:55:54.426743 windmill_api-1.88.0/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-04-17 22:55:54.418743 windmill_api-1.88.0/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-04-17 22:55:54.462743 windmill_api-1.88.0/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-04-17 22:55:54.486743 windmill_api-1.88.0/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-04-17 22:55:54.518743 windmill_api-1.88.0/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-04-17 22:55:54.542743 windmill_api-1.88.0/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    12602 2023-04-17 22:55:54.686744 windmill_api-1.88.0/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    11829 2023-04-17 22:55:54.698744 windmill_api-1.88.0/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12367 2023-04-17 22:55:54.850744 windmill_api-1.88.0/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-04-17 22:55:54.730744 windmill_api-1.88.0/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-04-17 22:55:54.762744 windmill_api-1.88.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-04-17 22:55:54.806744 windmill_api-1.88.0/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-04-17 22:55:54.850744 windmill_api-1.88.0/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-04-17 22:55:54.910744 windmill_api-1.88.0/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-04-17 22:55:54.894744 windmill_api-1.88.0/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-04-17 22:55:54.954744 windmill_api-1.88.0/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-04-17 22:55:54.966744 windmill_api-1.88.0/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-04-17 22:55:55.018744 windmill_api-1.88.0/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-04-17 22:55:55.006744 windmill_api-1.88.0/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-04-17 22:55:55.054744 windmill_api-1.88.0/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-04-17 22:55:55.070744 windmill_api-1.88.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.470714 windmill_api-1.88.0/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-17 22:55:55.098744 windmill_api-1.88.0/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-04-17 22:55:55.098744 windmill_api-1.88.0/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-04-17 22:55:55.130745 windmill_api-1.88.0/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-04-17 22:55:55.158745 windmill_api-1.88.0/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-04-17 22:55:55.154745 windmill_api-1.88.0/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-04-17 22:55:55.178745 windmill_api-1.88.0/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-04-17 22:55:55.198745 windmill_api-1.88.0/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-04-17 22:55:55.210745 windmill_api-1.88.0/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.474714 windmill_api-1.88.0/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-17 22:55:55.230745 windmill_api-1.88.0/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-04-17 22:55:55.238745 windmill_api-1.88.0/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-04-17 22:55:55.258745 windmill_api-1.88.0/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-04-17 22:55:55.266745 windmill_api-1.88.0/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-04-17 22:55:55.302745 windmill_api-1.88.0/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-04-17 22:55:55.306745 windmill_api-1.88.0/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-04-17 22:55:55.346745 windmill_api-1.88.0/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-04-17 22:55:55.362745 windmill_api-1.88.0/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-04-17 22:55:55.374745 windmill_api-1.88.0/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-04-17 22:55:55.434745 windmill_api-1.88.0/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-04-17 22:55:55.418745 windmill_api-1.88.0/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-04-17 22:55:55.458745 windmill_api-1.88.0/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-04-17 22:55:55.466745 windmill_api-1.88.0/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-04-17 22:55:55.518746 windmill_api-1.88.0/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-04-17 22:55:55.498746 windmill_api-1.88.0/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.534714 windmill_api-1.88.0/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-17 22:55:55.530746 windmill_api-1.88.0/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-04-17 22:55:55.550746 windmill_api-1.88.0/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-04-17 22:55:55.570746 windmill_api-1.88.0/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-04-17 22:55:55.590746 windmill_api-1.88.0/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-04-17 22:55:55.630746 windmill_api-1.88.0/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-04-17 22:55:55.638746 windmill_api-1.88.0/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-04-17 22:55:55.658746 windmill_api-1.88.0/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-04-17 22:55:55.670746 windmill_api-1.88.0/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.482714 windmill_api-1.88.0/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-04-17 22:55:55.718746 windmill_api-1.88.0/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-04-17 22:55:55.702746 windmill_api-1.88.0/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-04-17 22:55:55.742746 windmill_api-1.88.0/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-04-17 22:55:55.746746 windmill_api-1.88.0/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-04-17 22:55:55.786746 windmill_api-1.88.0/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-04-17 22:55:55.790746 windmill_api-1.88.0/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-04-17 22:55:55.826746 windmill_api-1.88.0/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-04-17 22:55:55.830746 windmill_api-1.88.0/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-04-17 22:55:55.878746 windmill_api-1.88.0/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-04-17 22:55:55.858746 windmill_api-1.88.0/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-04-17 22:55:55.898746 windmill_api-1.88.0/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-04-17 22:55:55.922747 windmill_api-1.88.0/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3276 2023-04-17 22:55:55.938747 windmill_api-1.88.0/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-04-17 22:55:55.962746 windmill_api-1.88.0/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-04-17 22:55:55.970747 windmill_api-1.88.0/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-04-17 22:55:55.990747 windmill_api-1.88.0/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-04-17 22:55:56.122747 windmill_api-1.88.0/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-04-17 22:55:56.030747 windmill_api-1.88.0/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-04-17 22:55:56.058747 windmill_api-1.88.0/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-04-17 22:55:56.090747 windmill_api-1.88.0/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-04-17 22:55:56.122747 windmill_api-1.88.0/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.410714 windmill_api-1.88.0/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-17 22:55:56.146747 windmill_api-1.88.0/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-04-17 22:55:56.150747 windmill_api-1.88.0/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.442714 windmill_api-1.88.0/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-04-17 22:55:56.170747 windmill_api-1.88.0/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-04-17 22:55:56.178747 windmill_api-1.88.0/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-04-17 22:55:56.198747 windmill_api-1.88.0/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-04-17 22:55:56.210747 windmill_api-1.88.0/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-04-17 22:55:56.226747 windmill_api-1.88.0/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-04-17 22:55:56.254747 windmill_api-1.88.0/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-04-17 22:55:56.254747 windmill_api-1.88.0/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-04-17 22:55:56.282747 windmill_api-1.88.0/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-04-17 22:55:56.278747 windmill_api-1.88.0/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-04-17 22:55:56.306747 windmill_api-1.88.0/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-04-17 22:55:56.306747 windmill_api-1.88.0/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-04-17 22:55:56.338747 windmill_api-1.88.0/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-04-17 22:55:56.342748 windmill_api-1.88.0/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-04-17 22:55:56.378748 windmill_api-1.88.0/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-04-17 22:55:56.370747 windmill_api-1.88.0/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-04-17 22:55:56.430748 windmill_api-1.88.0/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-04-17 22:55:56.414748 windmill_api-1.88.0/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-04-17 22:55:56.458748 windmill_api-1.88.0/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-04-17 22:55:56.486748 windmill_api-1.88.0/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-04-17 22:55:56.494748 windmill_api-1.88.0/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-04-17 22:55:56.514748 windmill_api-1.88.0/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-04-17 22:55:56.522748 windmill_api-1.88.0/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-04-17 22:55:56.542748 windmill_api-1.88.0/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-04-17 22:55:56.550748 windmill_api-1.88.0/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-04-17 22:55:56.574748 windmill_api-1.88.0/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-04-17 22:55:56.602748 windmill_api-1.88.0/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-04-17 22:55:56.618748 windmill_api-1.88.0/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.462714 windmill_api-1.88.0/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-04-17 22:55:56.638748 windmill_api-1.88.0/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-04-17 22:55:56.658748 windmill_api-1.88.0/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-04-17 22:55:56.678748 windmill_api-1.88.0/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-04-17 22:55:56.710748 windmill_api-1.88.0/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-04-17 22:55:56.718748 windmill_api-1.88.0/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-04-17 22:55:56.754748 windmill_api-1.88.0/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-04-17 22:55:56.758748 windmill_api-1.88.0/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.550714 windmill_api-1.88.0/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     3896 2023-04-17 22:55:56.826749 windmill_api-1.88.0/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:55:42.454714 windmill_api-1.88.0/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-04-17 22:55:56.790748 windmill_api-1.88.0/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-04-17 22:55:56.814749 windmill_api-1.88.0/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-04-17 22:55:56.842749 windmill_api-1.88.0/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-04-17 22:55:56.858749 windmill_api-1.88.0/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-04-17 22:55:56.866749 windmill_api-1.88.0/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-04-17 22:55:56.890749 windmill_api-1.88.0/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-04-17 22:55:56.898749 windmill_api-1.88.0/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-04-17 22:55:56.918749 windmill_api-1.88.0/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-04-17 22:55:56.938749 windmill_api-1.88.0/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-04-17 22:55:56.950749 windmill_api-1.88.0/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-04-17 22:55:56.978749 windmill_api-1.88.0/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-04-17 22:55:56.986749 windmill_api-1.88.0/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-04-17 22:55:57.006749 windmill_api-1.88.0/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-04-17 22:55:57.022749 windmill_api-1.88.0/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-04-17 22:55:57.046749 windmill_api-1.88.0/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-04-17 22:55:57.058749 windmill_api-1.88.0/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-04-17 22:55:57.082749 windmill_api-1.88.0/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-04-17 22:55:57.118749 windmill_api-1.88.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-04-17 22:55:57.110749 windmill_api-1.88.0/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-04-17 22:55:57.138749 windmill_api-1.88.0/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-04-17 22:56:14.346781 windmill_api-1.88.0/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-04-17 22:55:57.166749 windmill_api-1.88.0/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-04-17 22:55:57.194749 windmill_api-1.88.0/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      301 2023-04-17 22:55:52.190738 windmill_api-1.88.0/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-04-17 22:55:57.218750 windmill_api-1.88.0/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-04-17 22:55:57.250750 windmill_api-1.88.0/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-04-17 22:55:57.290750 windmill_api-1.88.0/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-04-17 22:55:57.306750 windmill_api-1.88.0/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-04-17 22:55:52.110737 windmill_api-1.88.0/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-04-17 22:55:57.314750 windmill_api-1.88.0/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-04-17 22:55:57.358750 windmill_api-1.88.0/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-04-17 22:55:51.578736 windmill_api-1.88.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-04-17 22:55:57.342750 windmill_api-1.88.0/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-04-17 22:55:57.366750 windmill_api-1.88.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1569 2023-04-17 22:55:57.382750 windmill_api-1.88.0/windmill_api/models/archive_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     6879 2023-04-17 22:55:57.454750 windmill_api-1.88.0/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-04-17 22:55:57.402750 windmill_api-1.88.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-04-17 22:55:51.774737 windmill_api-1.88.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-04-17 22:55:52.226738 windmill_api-1.88.0/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-04-17 22:55:57.430750 windmill_api-1.88.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-04-17 22:55:57.514750 windmill_api-1.88.0/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-04-17 22:55:51.698737 windmill_api-1.88.0/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-04-17 22:55:51.606736 windmill_api-1.88.0/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-04-17 22:55:57.482750 windmill_api-1.88.0/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-04-17 22:55:57.522750 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-04-17 22:55:57.578750 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-04-17 22:55:51.666736 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-04-17 22:55:57.550750 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-04-17 22:55:57.578750 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-04-17 22:55:57.606750 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-04-17 22:55:57.618750 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-04-17 22:55:51.470736 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-04-17 22:55:57.634750 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-04-17 22:55:57.678751 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-04-17 22:55:52.146737 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-04-17 22:55:57.662751 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-17 22:55:51.438736 windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-04-17 22:55:57.714751 windmill_api-1.88.0/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-04-17 22:55:57.714751 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-04-17 22:55:57.798751 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-04-17 22:55:57.754751 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-17 22:55:57.782751 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-17 22:55:57.818751 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-17 22:55:57.830751 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-17 22:55:51.782737 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-17 22:55:57.846751 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-17 22:55:51.882737 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-17 22:55:57.862751 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-17 22:55:57.878751 windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-04-17 22:55:52.442738 windmill_api-1.88.0/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-04-17 22:55:57.926751 windmill_api-1.88.0/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-04-17 22:55:57.914751 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-04-17 22:55:57.994751 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-04-17 22:55:57.966751 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-17 22:55:57.998751 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-17 22:55:58.026751 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-17 22:55:58.030751 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-17 22:55:51.698737 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-17 22:55:58.070752 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-17 22:55:52.318738 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-17 22:55:58.062751 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-17 22:55:58.094751 windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-04-17 22:55:58.154752 windmill_api-1.88.0/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-04-17 22:55:58.138752 windmill_api-1.88.0/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-04-17 22:55:58.170752 windmill_api-1.88.0/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-04-17 22:55:58.186752 windmill_api-1.88.0/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-04-17 22:55:58.198752 windmill_api-1.88.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-04-17 22:55:52.038737 windmill_api-1.88.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-04-17 22:55:58.218752 windmill_api-1.88.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-17 22:55:51.566736 windmill_api-1.88.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-04-17 22:55:58.230752 windmill_api-1.88.0/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-04-17 22:55:58.250752 windmill_api-1.88.0/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-04-17 22:55:51.966737 windmill_api-1.88.0/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-04-17 22:55:58.258752 windmill_api-1.88.0/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-04-17 22:55:58.270752 windmill_api-1.88.0/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10376 2023-04-17 22:55:58.414752 windmill_api-1.88.0/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-04-17 22:55:58.290752 windmill_api-1.88.0/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-04-17 22:55:58.334752 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-04-17 22:55:58.446752 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-04-17 22:55:58.438752 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-04-17 22:55:58.470752 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-04-17 22:55:52.162737 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-04-17 22:55:58.474752 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-04-17 22:55:58.510753 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-04-17 22:55:51.766737 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-04-17 22:55:58.554752 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-04-17 22:55:58.538752 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-04-17 22:55:58.570752 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-04-17 22:55:52.210738 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-04-17 22:55:58.582753 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-04-17 22:55:58.610753 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-04-17 22:55:51.774737 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-04-17 22:55:58.618753 windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-04-17 22:55:51.722736 windmill_api-1.88.0/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-04-17 22:55:51.810737 windmill_api-1.88.0/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-04-17 22:55:58.658753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-04-17 22:55:58.706753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-04-17 22:55:58.726753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-17 22:55:58.742753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-17 22:55:58.762753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-17 22:55:58.770753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-17 22:55:51.962737 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-17 22:55:58.802753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-17 22:55:52.442738 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-17 22:55:58.818753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-17 22:55:58.834753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-04-17 22:55:58.902753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-04-17 22:55:58.874753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-04-17 22:55:58.906753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-04-17 22:55:58.934753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-04-17 22:55:58.938753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-04-17 22:55:52.422738 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-04-17 22:55:58.962753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-04-17 22:55:51.602736 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-04-17 22:55:58.970754 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-04-17 22:55:58.994753 windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-04-17 22:55:58.998753 windmill_api-1.88.0/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-04-17 22:55:59.030753 windmill_api-1.88.0/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-04-17 22:55:59.022754 windmill_api-1.88.0/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-04-17 22:55:59.054754 windmill_api-1.88.0/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-04-17 22:55:59.062754 windmill_api-1.88.0/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2035 2023-04-17 22:55:59.106754 windmill_api-1.88.0/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-04-17 22:55:59.110754 windmill_api-1.88.0/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-04-17 22:55:51.862737 windmill_api-1.88.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-04-17 22:55:59.138754 windmill_api-1.88.0/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-04-17 22:55:59.130754 windmill_api-1.88.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-04-17 22:55:59.194754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-04-17 22:55:59.158754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-04-17 22:55:59.202754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-04-17 22:55:59.278754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-04-17 22:55:59.242754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-04-17 22:55:59.274754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-04-17 22:55:59.310754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-04-17 22:55:59.310754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-17 22:55:51.894737 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-04-17 22:55:59.334754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-17 22:55:52.414738 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-04-17 22:55:59.342754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-04-17 22:55:59.366754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-04-17 22:55:59.426754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-04-17 22:55:59.406754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-04-17 22:55:59.434754 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-04-17 22:55:59.462755 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-04-17 22:55:59.466755 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-04-17 22:55:51.986737 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-04-17 22:55:59.490755 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-04-17 22:55:52.094737 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-04-17 22:55:59.514755 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-04-17 22:55:59.522755 windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2126 2023-04-17 22:55:59.550755 windmill_api-1.88.0/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-04-17 22:55:59.570755 windmill_api-1.88.0/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     1613 2023-04-17 22:55:59.578755 windmill_api-1.88.0/windmill_api/models/create_input.py
+-rw-r--r--   0        0        0     1171 2023-04-17 22:55:59.590755 windmill_api-1.88.0/windmill_api/models/create_input_args.py
+-rw-r--r--   0        0        0     1701 2023-04-17 22:55:59.606755 windmill_api-1.88.0/windmill_api/models/create_input_json_body.py
+-rw-r--r--   0        0        0     1217 2023-04-17 22:55:59.610755 windmill_api-1.88.0/windmill_api/models/create_input_json_body_args.py
+-rw-r--r--   0        0        0      214 2023-04-17 22:55:51.894737 windmill_api-1.88.0/windmill_api/models/create_input_runnable_type.py
+-rw-r--r--   0        0        0     2094 2023-04-17 22:55:59.642755 windmill_api-1.88.0/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-04-17 22:55:59.646755 windmill_api-1.88.0/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-04-17 22:55:59.678755 windmill_api-1.88.0/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-04-17 22:55:59.686755 windmill_api-1.88.0/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-04-17 22:55:59.698755 windmill_api-1.88.0/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     4616 2023-04-17 22:55:59.758755 windmill_api-1.88.0/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-04-17 22:55:51.962737 windmill_api-1.88.0/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-04-17 22:55:51.710736 windmill_api-1.88.0/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-04-17 22:55:59.722755 windmill_api-1.88.0/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-04-17 22:55:59.758755 windmill_api-1.88.0/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-04-17 22:55:59.794755 windmill_api-1.88.0/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-04-17 22:55:59.794755 windmill_api-1.88.0/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-04-17 22:55:59.830755 windmill_api-1.88.0/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-04-17 22:55:59.834755 windmill_api-1.88.0/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-04-17 22:55:59.878755 windmill_api-1.88.0/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-04-17 22:55:59.862755 windmill_api-1.88.0/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-04-17 22:55:59.894755 windmill_api-1.88.0/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-04-17 22:55:59.922756 windmill_api-1.88.0/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    10978 2023-04-17 22:56:00.050756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-04-17 22:55:59.946756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-04-17 22:55:59.990756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-04-17 22:56:00.082756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-04-17 22:56:00.074756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-04-17 22:56:00.106756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-04-17 22:55:51.578736 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-04-17 22:56:00.110756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-04-17 22:56:00.142756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-04-17 22:55:52.306738 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-04-17 22:56:00.202756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-04-17 22:56:00.170756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-04-17 22:56:00.198756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-04-17 22:55:52.262738 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-04-17 22:56:00.226756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-04-17 22:56:00.238756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-04-17 22:55:52.466738 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-04-17 22:56:00.262756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-04-17 22:55:52.426738 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-04-17 22:55:52.454738 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-04-17 22:56:00.314756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-04-17 22:56:00.374756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-04-17 22:56:00.354756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-04-17 22:56:00.386757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-04-17 22:56:00.406756 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-04-17 22:56:00.422757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-17 22:55:51.526736 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-17 22:56:00.438757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-17 22:55:52.158738 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-04-17 22:56:00.450757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-04-17 22:56:00.470757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-04-17 22:56:00.538757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-04-17 22:56:00.510757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-04-17 22:56:00.542757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-04-17 22:56:00.570757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-04-17 22:56:00.574757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-04-17 22:55:51.606736 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-04-17 22:56:00.602757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-04-17 22:55:52.066737 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-04-17 22:56:00.606757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-04-17 22:56:00.630757 windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-04-17 22:56:00.634757 windmill_api-1.88.0/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     6853 2023-04-17 22:56:00.750757 windmill_api-1.88.0/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-04-17 22:56:00.658757 windmill_api-1.88.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-04-17 22:55:52.118738 windmill_api-1.88.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-04-17 22:55:52.378738 windmill_api-1.88.0/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-04-17 22:56:00.682757 windmill_api-1.88.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-04-17 22:56:00.746757 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-04-17 22:56:00.810757 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-04-17 22:55:51.842737 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-04-17 22:56:00.778757 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-04-17 22:56:00.806758 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-04-17 22:56:00.834757 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-04-17 22:56:00.850757 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-04-17 22:55:51.562736 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-04-17 22:56:00.862758 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-04-17 22:56:00.886758 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-04-17 22:55:51.906737 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-04-17 22:56:00.894758 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-17 22:55:52.010737 windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-04-17 22:56:00.914758 windmill_api-1.88.0/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-04-17 22:56:00.926758 windmill_api-1.88.0/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-04-17 22:56:00.942758 windmill_api-1.88.0/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-04-17 22:56:00.958758 windmill_api-1.88.0/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-04-17 22:56:00.962758 windmill_api-1.88.0/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-04-17 22:56:00.986758 windmill_api-1.88.0/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-04-17 22:56:01.002758 windmill_api-1.88.0/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-04-17 22:56:01.014758 windmill_api-1.88.0/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-04-17 22:56:01.034758 windmill_api-1.88.0/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-04-17 22:56:01.062758 windmill_api-1.88.0/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-04-17 22:56:01.054758 windmill_api-1.88.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-04-17 22:56:01.086758 windmill_api-1.88.0/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-04-17 22:56:01.114758 windmill_api-1.88.0/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-04-17 22:56:01.110758 windmill_api-1.88.0/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4633 2023-04-17 22:56:01.206758 windmill_api-1.88.0/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-04-17 22:56:01.134758 windmill_api-1.88.0/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3416 2023-04-17 22:56:01.182758 windmill_api-1.88.0/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-04-17 22:56:01.202758 windmill_api-1.88.0/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-04-17 22:56:01.286759 windmill_api-1.88.0/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-04-17 22:56:01.246759 windmill_api-1.88.0/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-04-17 22:56:01.274758 windmill_api-1.88.0/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-04-17 22:56:01.310759 windmill_api-1.88.0/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-04-17 22:56:01.318759 windmill_api-1.88.0/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-04-17 22:55:51.618736 windmill_api-1.88.0/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-04-17 22:56:01.338759 windmill_api-1.88.0/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-04-17 22:55:51.618736 windmill_api-1.88.0/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-04-17 22:56:01.354759 windmill_api-1.88.0/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-04-17 22:56:01.370759 windmill_api-1.88.0/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3080 2023-04-17 22:56:01.398759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-04-17 22:56:01.406759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-17 22:56:01.430759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-17 22:55:51.558736 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-17 22:56:01.438759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-17 22:55:51.570736 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-04-17 22:55:52.166738 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-04-17 22:55:51.862737 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-04-17 22:56:01.470759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-04-17 22:56:01.478759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-17 22:56:01.530759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-17 22:55:51.566736 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-17 22:56:01.542759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-17 22:55:51.862737 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-04-17 22:55:51.790737 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-04-17 22:56:01.566759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-04-17 22:56:01.582759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-17 22:56:01.598759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-17 22:55:52.358738 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-17 22:56:01.610759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-17 22:55:52.482738 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-04-17 22:55:52.106737 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-04-17 22:56:01.662759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-04-17 22:56:01.642759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-04-17 22:55:51.630736 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-04-17 22:56:01.670759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-04-17 22:55:52.450738 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-04-17 22:56:01.750759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-04-17 22:56:01.710759 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-04-17 22:56:01.742760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-04-17 22:56:01.774760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-04-17 22:56:01.786760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-17 22:55:51.774737 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-04-17 22:56:01.806760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-17 22:55:52.286738 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-04-17 22:56:01.818760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-04-17 22:56:01.838760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-04-17 22:55:51.574736 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-04-17 22:56:01.862760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-04-17 22:56:01.874760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-04-17 22:56:01.978760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-04-17 22:56:01.914760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-04-17 22:56:01.966760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-04-17 22:56:02.002760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-04-17 22:56:02.010760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-17 22:55:51.902737 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-04-17 22:56:02.030760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-17 22:55:52.146737 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-04-17 22:56:02.042760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-04-17 22:56:02.062760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-04-17 22:56:02.126760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-04-17 22:56:02.102760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-04-17 22:56:02.134760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-04-17 22:56:02.166761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-04-17 22:56:02.162760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-17 22:55:51.554736 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-04-17 22:56:02.194760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-17 22:55:52.034737 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-04-17 22:56:02.194760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-04-17 22:56:02.226760 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-04-17 22:55:52.286738 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-04-17 22:56:02.234761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-04-17 22:56:02.266761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-04-17 22:56:02.346761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-04-17 22:56:02.310761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-04-17 22:56:02.370761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-04-17 22:56:02.378761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-04-17 22:56:02.402761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-17 22:55:52.454738 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-04-17 22:56:02.406761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-17 22:55:51.818737 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-04-17 22:56:02.434761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-04-17 22:56:02.438761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-04-17 22:55:52.190738 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-04-17 22:56:02.466761 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-04-17 22:55:52.038737 windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-04-17 22:56:02.474761 windmill_api-1.88.0/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-04-17 22:56:02.490761 windmill_api-1.88.0/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-04-17 22:56:02.518761 windmill_api-1.88.0/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-04-17 22:56:02.574761 windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-04-17 22:56:02.558761 windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-04-17 22:56:02.586761 windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-04-17 22:56:02.610762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-04-17 22:56:02.618761 windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-17 22:55:51.858737 windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-04-17 22:56:02.642762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-17 22:55:51.822737 windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-04-17 22:56:02.646762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-04-17 22:56:02.674762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-04-17 22:56:02.762762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-04-17 22:56:02.714762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-04-17 22:56:02.778762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-04-17 22:56:02.798762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-04-17 22:56:02.810762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-04-17 22:55:52.290738 windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-04-17 22:56:02.826762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-04-17 22:55:51.866737 windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-04-17 22:56:02.842762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-04-17 22:56:02.858762 windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-04-17 22:56:02.866762 windmill_api-1.88.0/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-04-17 22:56:02.902762 windmill_api-1.88.0/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-04-17 22:56:02.954762 windmill_api-1.88.0/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-04-17 22:56:02.926762 windmill_api-1.88.0/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-04-17 22:56:02.958762 windmill_api-1.88.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-04-17 22:55:51.778737 windmill_api-1.88.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-04-17 22:56:02.982762 windmill_api-1.88.0/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-04-17 22:56:02.994762 windmill_api-1.88.0/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-04-17 22:55:51.558736 windmill_api-1.88.0/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-04-17 22:56:03.070762 windmill_api-1.88.0/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-04-17 22:56:03.022762 windmill_api-1.88.0/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-04-17 22:56:03.050763 windmill_api-1.88.0/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-04-17 22:55:51.830737 windmill_api-1.88.0/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-04-17 22:56:03.082763 windmill_api-1.88.0/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-04-17 22:56:03.106763 windmill_api-1.88.0/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-04-17 22:55:52.294738 windmill_api-1.88.0/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-04-17 22:56:03.210763 windmill_api-1.88.0/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-04-17 22:56:03.170763 windmill_api-1.88.0/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-04-17 22:56:03.198763 windmill_api-1.88.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-04-17 22:55:51.650736 windmill_api-1.88.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-04-17 22:56:03.226763 windmill_api-1.88.0/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-04-17 22:56:03.246763 windmill_api-1.88.0/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-04-17 22:55:51.654736 windmill_api-1.88.0/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-04-17 22:56:03.266763 windmill_api-1.88.0/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-04-17 22:56:03.290763 windmill_api-1.88.0/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-04-17 22:56:03.350763 windmill_api-1.88.0/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-04-17 22:56:03.330763 windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-04-17 22:56:03.358763 windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-04-17 22:56:03.382763 windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-04-17 22:56:03.390763 windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-04-17 22:55:51.666736 windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-04-17 22:56:03.414763 windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-04-17 22:55:51.810737 windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-04-17 22:56:03.422763 windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-04-17 22:56:03.446763 windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-04-17 22:56:03.502763 windmill_api-1.88.0/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-04-17 22:56:03.486763 windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-04-17 22:56:03.518763 windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-04-17 22:56:03.570763 windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-04-17 22:56:03.582764 windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-04-17 22:55:52.490738 windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-04-17 22:56:03.602764 windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-17 22:55:51.926737 windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-04-17 22:56:03.614764 windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-04-17 22:56:03.630764 windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-04-17 22:56:03.646764 windmill_api-1.88.0/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-04-17 22:56:03.654764 windmill_api-1.88.0/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-04-17 22:56:03.674764 windmill_api-1.88.0/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-04-17 22:56:03.702764 windmill_api-1.88.0/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-04-17 22:56:03.702764 windmill_api-1.88.0/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-04-17 22:55:52.126737 windmill_api-1.88.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-04-17 22:56:03.734764 windmill_api-1.88.0/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-04-17 22:55:51.754737 windmill_api-1.88.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-04-17 22:56:03.798764 windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-04-17 22:56:03.778764 windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-04-17 22:56:03.806764 windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-04-17 22:56:03.834764 windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-04-17 22:56:03.834764 windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-04-17 22:55:52.186738 windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-04-17 22:56:03.862764 windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-04-17 22:55:51.570736 windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-04-17 22:56:03.866764 windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-04-17 22:56:03.890764 windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-04-17 22:55:51.494736 windmill_api-1.88.0/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-04-17 22:56:03.922764 windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-04-17 22:55:52.034737 windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-04-17 22:56:03.914764 windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-04-17 22:56:03.994764 windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-04-17 22:55:51.786737 windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-04-17 22:56:03.986765 windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-04-17 22:56:04.006765 windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-04-17 22:56:04.050765 windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-04-17 22:55:52.334738 windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-04-17 22:56:04.030765 windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-04-17 22:56:04.078765 windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-04-17 22:55:52.238738 windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-04-17 22:56:04.074765 windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-04-17 22:56:04.098765 windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-04-17 22:56:04.134765 windmill_api-1.88.0/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-04-17 22:55:51.810737 windmill_api-1.88.0/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-04-17 22:55:51.710736 windmill_api-1.88.0/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-04-17 22:56:04.122765 windmill_api-1.88.0/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    10876 2023-04-17 22:56:04.258765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-04-17 22:56:04.154765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-04-17 22:56:04.198765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-04-17 22:56:04.290765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-04-17 22:56:04.282765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-04-17 22:56:04.314765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-04-17 22:55:52.078737 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-04-17 22:56:04.318765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-04-17 22:56:04.386765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-04-17 22:55:51.846737 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-04-17 22:56:04.446766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-04-17 22:56:04.414765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-04-17 22:56:04.442766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-04-17 22:55:52.042737 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-04-17 22:56:04.470765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-04-17 22:56:04.486765 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-04-17 22:55:51.426736 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-04-17 22:56:04.502766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-04-17 22:55:52.462738 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-04-17 22:55:52.326738 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-04-17 22:56:04.534766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-04-17 22:56:04.586766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-04-17 22:56:04.578766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-04-17 22:56:04.610766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-04-17 22:56:04.618766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-04-17 22:56:04.642766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-04-17 22:55:51.782737 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-04-17 22:56:04.646766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-04-17 22:55:52.338738 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-04-17 22:56:04.674766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-04-17 22:56:04.678766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-04-17 22:56:04.806766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-04-17 22:56:04.718766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-04-17 22:56:04.782766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-04-17 22:56:04.814766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-04-17 22:56:04.838766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-17 22:55:51.458736 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-04-17 22:56:04.842766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-17 22:55:52.066737 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-04-17 22:56:04.870766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-04-17 22:56:04.874766 windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5083 2023-04-17 22:56:04.942767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-04-17 22:56:04.894766 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-04-17 22:56:04.914766 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-04-17 22:56:04.954767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-04-17 22:56:05.026767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-04-17 22:56:04.998767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-04-17 22:56:05.026767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-04-17 22:56:05.058767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-04-17 22:56:05.058767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-17 22:55:51.810737 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-04-17 22:56:05.086767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-17 22:55:51.658736 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-04-17 22:56:05.090767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-04-17 22:56:05.114767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-04-17 22:56:05.222767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-04-17 22:56:05.186767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-04-17 22:56:05.214767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-04-17 22:56:05.246767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-04-17 22:56:05.254767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-17 22:55:51.858737 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-04-17 22:56:05.278767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-17 22:55:52.206738 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-04-17 22:56:05.286767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-04-17 22:56:05.306767 windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2756 2023-04-17 22:56:05.326767 windmill_api-1.88.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
+-rw-r--r--   0        0        0     1337 2023-04-17 22:56:05.330767 windmill_api-1.88.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
+-rw-r--r--   0        0        0     2010 2023-04-17 22:56:05.354767 windmill_api-1.88.0/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-04-17 22:56:05.346768 windmill_api-1.88.0/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-04-17 22:56:05.386767 windmill_api-1.88.0/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      301 2023-04-17 22:55:51.678736 windmill_api-1.88.0/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-04-17 22:56:05.378768 windmill_api-1.88.0/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-04-17 22:56:05.426768 windmill_api-1.88.0/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-04-17 22:56:05.406768 windmill_api-1.88.0/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-04-17 22:56:05.430768 windmill_api-1.88.0/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-04-17 22:56:05.450768 windmill_api-1.88.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-04-17 22:56:05.466768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-04-17 22:56:05.494768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-04-17 22:56:05.486768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-04-17 22:56:05.530768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-04-17 22:56:05.622768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-04-17 22:56:05.602768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-04-17 22:56:05.634768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-04-17 22:56:05.654768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-04-17 22:56:05.666768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-04-17 22:55:51.866737 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-04-17 22:56:05.682768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-04-17 22:55:51.694736 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-04-17 22:56:05.694768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-04-17 22:56:05.714768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-04-17 22:56:05.782768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-04-17 22:56:05.754768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-04-17 22:56:05.786768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-04-17 22:56:05.818768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-04-17 22:56:05.814768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-04-17 22:55:51.874737 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-04-17 22:56:05.846768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-04-17 22:55:52.006737 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-04-17 22:56:05.850768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-04-17 22:56:05.874768 windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-04-17 22:56:05.890768 windmill_api-1.88.0/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-04-17 22:55:51.534736 windmill_api-1.88.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     2644 2023-04-17 22:56:05.914768 windmill_api-1.88.0/windmill_api/models/get_input_history_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-04-17 22:56:05.914768 windmill_api-1.88.0/windmill_api/models/get_input_history_response_200_item_args.py
+-rw-r--r--   0        0        0      218 2023-04-17 22:55:52.202738 windmill_api-1.88.0/windmill_api/models/get_input_history_runnable_type.py
+-rw-r--r--   0        0        0     1852 2023-04-17 22:56:05.978768 windmill_api-1.88.0/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-04-17 22:55:52.278738 windmill_api-1.88.0/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-04-17 22:56:05.954769 windmill_api-1.88.0/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-04-17 22:56:05.986769 windmill_api-1.88.0/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-04-17 22:56:06.026769 windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-04-17 22:55:52.042737 windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-04-17 22:56:06.006769 windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-04-17 22:56:06.106769 windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-04-17 22:55:51.574736 windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-04-17 22:56:06.054769 windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-04-17 22:56:06.074769 windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-04-17 22:56:06.126769 windmill_api-1.88.0/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-04-17 22:56:06.130769 windmill_api-1.88.0/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-04-17 22:56:06.162769 windmill_api-1.88.0/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-04-17 22:56:06.158769 windmill_api-1.88.0/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-04-17 22:56:06.222769 windmill_api-1.88.0/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-04-17 22:56:06.182769 windmill_api-1.88.0/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-04-17 22:56:06.202769 windmill_api-1.88.0/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     6775 2023-04-17 22:56:06.286769 windmill_api-1.88.0/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-04-17 22:56:06.242769 windmill_api-1.88.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-17 22:55:52.046737 windmill_api-1.88.0/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-04-17 22:55:51.562736 windmill_api-1.88.0/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-04-17 22:56:06.270769 windmill_api-1.88.0/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     6775 2023-04-17 22:56:06.358769 windmill_api-1.88.0/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-04-17 22:56:06.306769 windmill_api-1.88.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-17 22:55:51.862737 windmill_api-1.88.0/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-04-17 22:55:52.338738 windmill_api-1.88.0/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-04-17 22:56:06.362769 windmill_api-1.88.0/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-04-17 22:56:06.386769 windmill_api-1.88.0/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-04-17 22:56:06.418769 windmill_api-1.88.0/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-04-17 22:56:06.422769 windmill_api-1.88.0/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-04-17 22:56:06.442769 windmill_api-1.88.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-04-17 22:56:06.454769 windmill_api-1.88.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-04-17 22:55:51.562736 windmill_api-1.88.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-04-17 22:56:06.506769 windmill_api-1.88.0/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-04-17 22:56:06.474769 windmill_api-1.88.0/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-04-17 22:56:06.566769 windmill_api-1.88.0/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-04-17 22:55:51.590736 windmill_api-1.88.0/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-04-17 22:56:06.530769 windmill_api-1.88.0/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-04-17 22:56:06.570769 windmill_api-1.88.0/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-04-17 22:55:51.522736 windmill_api-1.88.0/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-04-17 22:56:06.610769 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-04-17 22:56:06.630769 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-04-17 22:55:51.790737 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-04-17 22:56:06.634770 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-04-17 22:56:06.658769 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-04-17 22:56:06.666770 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-04-17 22:56:06.694769 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-04-17 22:55:52.154738 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-04-17 22:56:06.694769 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-04-17 22:56:06.734770 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-04-17 22:55:52.166738 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-04-17 22:56:06.754770 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-17 22:55:51.506736 windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-04-17 22:56:06.782770 windmill_api-1.88.0/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-04-17 22:56:06.774770 windmill_api-1.88.0/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-04-17 22:56:06.802770 windmill_api-1.88.0/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-04-17 22:55:52.134738 windmill_api-1.88.0/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     2377 2023-04-17 22:56:06.822770 windmill_api-1.88.0/windmill_api/models/input_.py
+-rw-r--r--   0        0        0     1138 2023-04-17 22:56:06.822770 windmill_api-1.88.0/windmill_api/models/input_args.py
+-rw-r--r--   0        0        0     1820 2023-04-17 22:56:06.854770 windmill_api-1.88.0/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-04-17 22:55:52.022737 windmill_api-1.88.0/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-04-17 22:56:06.854770 windmill_api-1.88.0/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-04-17 22:55:51.922737 windmill_api-1.88.0/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-04-17 22:56:06.886770 windmill_api-1.88.0/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-04-17 22:56:06.882770 windmill_api-1.88.0/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-04-17 22:55:52.478738 windmill_api-1.88.0/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-04-17 22:56:06.910770 windmill_api-1.88.0/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-04-17 22:55:51.842737 windmill_api-1.88.0/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-04-17 22:56:06.934770 windmill_api-1.88.0/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-04-17 22:55:51.630736 windmill_api-1.88.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-04-17 22:56:06.934770 windmill_api-1.88.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-04-17 22:55:51.754737 windmill_api-1.88.0/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-04-17 22:56:06.986770 windmill_api-1.88.0/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-04-17 22:55:52.190738 windmill_api-1.88.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-04-17 22:55:52.182738 windmill_api-1.88.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-04-17 22:56:06.962770 windmill_api-1.88.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11088 2023-04-17 22:56:07.146770 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-04-17 22:56:07.006770 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-04-17 22:56:07.050770 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-04-17 22:56:07.170770 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-04-17 22:56:07.174770 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-04-17 22:56:07.198770 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-04-17 22:55:51.666736 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-04-17 22:56:07.206770 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-04-17 22:56:07.234770 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-04-17 22:55:51.790737 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-04-17 22:56:07.290770 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-04-17 22:56:07.262771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-04-17 22:56:07.290770 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-04-17 22:55:52.058737 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-04-17 22:56:07.318771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-04-17 22:56:07.330771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-04-17 22:55:52.458738 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-04-17 22:56:07.354771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-04-17 22:55:51.518736 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-04-17 22:55:51.798737 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-04-17 22:56:07.378771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-04-17 22:56:07.438771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-04-17 22:56:07.478771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-04-17 22:56:07.470771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-04-17 22:56:07.546771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-04-17 22:56:07.510771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-04-17 22:55:52.350738 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-04-17 22:56:07.538771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-04-17 22:55:51.874737 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-04-17 22:56:07.570771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-04-17 22:56:07.574771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-04-17 22:56:07.658771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-04-17 22:56:07.614771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-04-17 22:56:07.646771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-04-17 22:56:07.678771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-04-17 22:56:07.690771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-04-17 22:55:52.086737 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-04-17 22:56:07.710771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-04-17 22:55:52.178737 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-04-17 22:56:07.722771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-04-17 22:56:07.738771 windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-04-17 22:56:07.750771 windmill_api-1.88.0/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     5077 2023-04-17 22:56:07.810771 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-04-17 22:56:07.770771 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     1255 2023-04-17 22:56:07.790771 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_schema.py
+-rw-r--r--   0        0        0     3297 2023-04-17 22:56:07.882771 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value.py
+-rw-r--r--   0        0        0     7151 2023-04-17 22:56:07.890771 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py
+-rw-r--r--   0        0        0     3318 2023-04-17 22:56:07.926771 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1985 2023-04-17 22:56:07.962772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2289 2023-04-17 22:56:07.962772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2187 2023-04-17 22:56:07.994772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-17 22:55:51.442736 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2054 2023-04-17 22:56:07.994772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-17 22:55:51.718737 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1978 2023-04-17 22:56:08.022771 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2029 2023-04-17 22:56:08.022771 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7049 2023-04-17 22:56:08.110772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py
+-rw-r--r--   0        0        0     3284 2023-04-17 22:56:08.066772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1975 2023-04-17 22:56:08.094772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-04-17 22:56:08.130772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-04-17 22:56:08.142772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-17 22:55:52.254738 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-04-17 22:56:08.158772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-17 22:55:52.366738 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-04-17 22:56:08.170772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-04-17 22:56:08.190772 windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2074 2023-04-17 22:56:08.202772 windmill_api-1.88.0/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-04-17 22:56:08.210772 windmill_api-1.88.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-04-17 22:56:08.246772 windmill_api-1.88.0/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-04-17 22:56:08.234772 windmill_api-1.88.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-04-17 22:56:08.266772 windmill_api-1.88.0/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-04-17 22:56:08.286772 windmill_api-1.88.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-04-17 22:56:08.298772 windmill_api-1.88.0/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-04-17 22:56:08.366772 windmill_api-1.88.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-04-17 22:56:08.334772 windmill_api-1.88.0/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-04-17 22:56:08.374772 windmill_api-1.88.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-04-17 22:55:52.006737 windmill_api-1.88.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     2590 2023-04-17 22:56:08.406772 windmill_api-1.88.0/windmill_api/models/list_inputs_response_200_item.py
+-rw-r--r--   0        0        0     1250 2023-04-17 22:56:08.442772 windmill_api-1.88.0/windmill_api/models/list_inputs_response_200_item_args.py
+-rw-r--r--   0        0        0      213 2023-04-17 22:55:51.574736 windmill_api-1.88.0/windmill_api/models/list_inputs_runnable_type.py
+-rw-r--r--   0        0        0     1922 2023-04-17 22:56:08.438772 windmill_api-1.88.0/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-04-17 22:55:51.638736 windmill_api-1.88.0/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-04-17 22:56:08.474772 windmill_api-1.88.0/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    11982 2023-04-17 22:56:08.598772 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-04-17 22:56:08.490772 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-04-17 22:56:08.538772 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-04-17 22:56:08.622773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-04-17 22:56:08.626772 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-04-17 22:56:08.654773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-04-17 22:55:52.278738 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-04-17 22:56:08.654773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-04-17 22:56:08.690773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-04-17 22:55:51.638736 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-04-17 22:56:08.742773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-04-17 22:56:08.766773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-04-17 22:56:08.774773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-04-17 22:55:51.642736 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-04-17 22:56:08.794773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-04-17 22:56:08.870773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-04-17 22:55:52.290738 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-04-17 22:56:08.826773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-04-17 22:55:51.430736 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-04-17 22:55:52.038737 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-04-17 22:56:08.874773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-04-17 22:56:08.954773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-04-17 22:56:08.914773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-04-17 22:56:08.942773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-04-17 22:56:08.974773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-04-17 22:56:08.986773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-17 22:55:52.006737 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-04-17 22:56:09.006773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-17 22:55:52.226738 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-04-17 22:56:09.018773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-04-17 22:56:09.034773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-04-17 22:56:09.102773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-04-17 22:56:09.074773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-04-17 22:56:09.106773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-04-17 22:56:09.138773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-04-17 22:56:09.134773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-17 22:55:51.430736 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-04-17 22:56:09.166773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-17 22:55:51.838737 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-04-17 22:56:09.166773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-04-17 22:56:09.198773 windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     4884 2023-04-17 22:56:09.286774 windmill_api-1.88.0/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-04-17 22:56:09.274773 windmill_api-1.88.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-04-17 22:56:09.310773 windmill_api-1.88.0/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-04-17 22:56:09.346773 windmill_api-1.88.0/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-04-17 22:56:09.334774 windmill_api-1.88.0/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-04-17 22:56:09.354774 windmill_api-1.88.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     6768 2023-04-17 22:56:09.430774 windmill_api-1.88.0/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-04-17 22:56:09.374774 windmill_api-1.88.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-17 22:55:52.162737 windmill_api-1.88.0/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-04-17 22:55:51.594736 windmill_api-1.88.0/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-04-17 22:56:09.398774 windmill_api-1.88.0/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-04-17 22:56:09.446774 windmill_api-1.88.0/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-04-17 22:56:09.462774 windmill_api-1.88.0/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-04-17 22:56:09.474774 windmill_api-1.88.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-04-17 22:56:09.498774 windmill_api-1.88.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-04-17 22:55:51.894737 windmill_api-1.88.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4307 2023-04-17 22:56:09.538774 windmill_api-1.88.0/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-04-17 22:56:09.526774 windmill_api-1.88.0/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-04-17 22:56:09.586774 windmill_api-1.88.0/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-04-17 22:56:09.558774 windmill_api-1.88.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-04-17 22:56:09.598774 windmill_api-1.88.0/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-04-17 22:56:09.662774 windmill_api-1.88.0/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-04-17 22:56:09.630774 windmill_api-1.88.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-04-17 22:56:09.666774 windmill_api-1.88.0/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-04-17 22:56:09.710774 windmill_api-1.88.0/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-04-17 22:55:51.430736 windmill_api-1.88.0/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-04-17 22:56:09.690774 windmill_api-1.88.0/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-04-17 22:56:09.814774 windmill_api-1.88.0/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-04-17 22:56:09.730774 windmill_api-1.88.0/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-04-17 22:56:09.794774 windmill_api-1.88.0/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-04-17 22:56:09.814774 windmill_api-1.88.0/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-04-17 22:56:09.842774 windmill_api-1.88.0/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-04-17 22:56:09.842774 windmill_api-1.88.0/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-04-17 22:56:09.870774 windmill_api-1.88.0/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-04-17 22:56:09.886774 windmill_api-1.88.0/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-04-17 22:56:09.930775 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-04-17 22:55:52.386738 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-04-17 22:56:09.914775 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-04-17 22:56:09.938774 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-04-17 22:56:09.958774 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-04-17 22:56:09.978775 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-04-17 22:55:51.494736 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-04-17 22:56:09.986775 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-04-17 22:56:10.018775 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-04-17 22:55:52.294738 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-04-17 22:56:10.010774 windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-17 22:55:52.418738 windmill_api-1.88.0/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-04-17 22:56:10.054775 windmill_api-1.88.0/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-04-17 22:56:10.038775 windmill_api-1.88.0/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     2108 2023-04-17 22:56:10.074775 windmill_api-1.88.0/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-04-17 22:56:10.142775 windmill_api-1.88.0/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-04-17 22:56:10.102775 windmill_api-1.88.0/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-04-17 22:56:10.150775 windmill_api-1.88.0/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-04-17 22:56:10.162775 windmill_api-1.88.0/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-04-17 22:56:10.194775 windmill_api-1.88.0/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-04-17 22:56:10.246775 windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-04-17 22:56:10.238775 windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-04-17 22:56:10.266775 windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-04-17 22:56:10.278775 windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-04-17 22:56:10.362775 windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-04-17 22:55:52.018737 windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-04-17 22:56:10.306775 windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-04-17 22:55:52.318738 windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-04-17 22:56:10.338775 windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-04-17 22:56:10.366775 windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-04-17 22:56:10.450775 windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-04-17 22:56:10.406775 windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-04-17 22:56:10.438775 windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-04-17 22:56:10.470775 windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-04-17 22:56:10.478775 windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-04-17 22:55:51.778737 windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-04-17 22:56:10.554775 windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-04-17 22:55:52.454738 windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-04-17 22:56:10.510775 windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-04-17 22:56:10.542775 windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-04-17 22:56:10.586775 windmill_api-1.88.0/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-04-17 22:56:10.574775 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-04-17 22:56:10.618775 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-04-17 22:56:10.670776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-04-17 22:56:10.658776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-04-17 22:56:10.686776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-04-17 22:56:10.702776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-04-17 22:56:10.718776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-04-17 22:55:52.058737 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-04-17 22:56:10.806776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-17 22:55:51.670736 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-04-17 22:56:10.746776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-04-17 22:56:10.778776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-04-17 22:56:10.862776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-04-17 22:56:10.846776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-04-17 22:56:10.878776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-04-17 22:56:10.894776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-04-17 22:56:10.910776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-17 22:55:52.322738 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-04-17 22:56:10.978776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-17 22:55:51.474736 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-04-17 22:56:10.942776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-04-17 22:56:10.970776 windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-04-17 22:56:11.002776 windmill_api-1.88.0/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-04-17 22:56:11.014776 windmill_api-1.88.0/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-04-17 22:56:11.034776 windmill_api-1.88.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-17 22:55:52.110737 windmill_api-1.88.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-04-17 22:56:11.042776 windmill_api-1.88.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-17 22:55:52.046737 windmill_api-1.88.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-04-17 22:55:51.742736 windmill_api-1.88.0/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-04-17 22:56:11.074776 windmill_api-1.88.0/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-04-17 22:56:11.078776 windmill_api-1.88.0/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-04-17 22:56:11.106776 windmill_api-1.88.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-04-17 22:55:51.718737 windmill_api-1.88.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-04-17 22:56:11.110776 windmill_api-1.88.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-04-17 22:55:51.562736 windmill_api-1.88.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-04-17 22:55:51.786737 windmill_api-1.88.0/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-04-17 22:56:11.158776 windmill_api-1.88.0/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-04-17 22:55:51.838737 windmill_api-1.88.0/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-04-17 22:56:11.138776 windmill_api-1.88.0/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-04-17 22:56:11.158776 windmill_api-1.88.0/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2147 2023-04-17 22:56:11.194776 windmill_api-1.88.0/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-04-17 22:56:11.178776 windmill_api-1.88.0/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-04-17 22:55:51.654736 windmill_api-1.88.0/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-04-17 22:56:11.210776 windmill_api-1.88.0/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-04-17 22:56:11.234776 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-04-17 22:56:11.274777 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-04-17 22:55:52.330738 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-04-17 22:56:11.258777 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-04-17 22:56:11.286776 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-04-17 22:56:11.302776 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-04-17 22:56:11.326777 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-04-17 22:55:51.706736 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-04-17 22:56:11.330777 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-04-17 22:56:11.362777 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-04-17 22:55:51.430736 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-04-17 22:56:11.426777 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-04-17 22:55:52.258738 windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11448 2023-04-17 22:56:11.570777 windmill_api-1.88.0/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-04-17 22:56:11.446777 windmill_api-1.88.0/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-04-17 22:56:11.490777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-04-17 22:56:11.578777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-04-17 22:56:11.598777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-04-17 22:56:11.610777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-04-17 22:55:51.834737 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-04-17 22:56:11.626777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-04-17 22:56:11.646777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-04-17 22:55:51.810737 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-04-17 22:56:11.706777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-04-17 22:56:11.670777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-04-17 22:56:11.702777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-04-17 22:55:51.910737 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-04-17 22:56:11.730777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-04-17 22:56:11.742777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-04-17 22:55:51.846737 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-04-17 22:56:11.766777 windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-04-17 22:55:51.426736 windmill_api-1.88.0/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-04-17 22:55:52.314738 windmill_api-1.88.0/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-04-17 22:56:11.790777 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-04-17 22:56:11.914777 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-04-17 22:56:11.898777 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-04-17 22:56:11.926777 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-04-17 22:56:11.946777 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-04-17 22:56:11.954778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-17 22:55:51.966737 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-04-17 22:56:11.978778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-17 22:55:51.986737 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-04-17 22:56:11.986778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-04-17 22:56:12.006778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-04-17 22:56:12.066778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-04-17 22:56:12.050778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-04-17 22:56:12.078778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-04-17 22:56:12.098778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-04-17 22:56:12.110778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-04-17 22:55:51.914737 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-04-17 22:56:12.126778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-04-17 22:55:51.534736 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-04-17 22:56:12.138778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-04-17 22:56:12.154778 windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-04-17 22:56:12.182778 windmill_api-1.88.0/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-04-17 22:56:12.190778 windmill_api-1.88.0/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-04-17 22:56:12.214778 windmill_api-1.88.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-04-17 22:55:51.502736 windmill_api-1.88.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-04-17 22:56:12.218778 windmill_api-1.88.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-04-17 22:55:52.458738 windmill_api-1.88.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-04-17 22:55:51.626736 windmill_api-1.88.0/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-04-17 22:55:52.242738 windmill_api-1.88.0/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-04-17 22:56:12.242778 windmill_api-1.88.0/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-04-17 22:56:12.290778 windmill_api-1.88.0/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      304 2023-04-17 22:55:52.414738 windmill_api-1.88.0/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-04-17 22:56:12.266778 windmill_api-1.88.0/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-04-17 22:56:12.294778 windmill_api-1.88.0/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-04-17 22:56:12.342778 windmill_api-1.88.0/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-04-17 22:56:12.314778 windmill_api-1.88.0/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-04-17 22:56:12.354778 windmill_api-1.88.0/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-04-17 22:56:12.362778 windmill_api-1.88.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-04-17 22:56:12.374778 windmill_api-1.88.0/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-04-17 22:56:12.402778 windmill_api-1.88.0/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-04-17 22:56:12.402778 windmill_api-1.88.0/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-04-17 22:56:12.434778 windmill_api-1.88.0/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-04-17 22:56:12.426778 windmill_api-1.88.0/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-04-17 22:56:12.458778 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-04-17 22:56:12.458778 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-04-17 22:56:12.498778 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-04-17 22:56:12.614779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-04-17 22:56:12.538778 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-04-17 22:56:12.570778 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-04-17 22:56:12.602779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-04-17 22:56:12.630779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-17 22:55:52.202738 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-04-17 22:56:12.642778 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-17 22:55:51.922737 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-04-17 22:56:12.662779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-04-17 22:56:12.674779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-04-17 22:56:12.818779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-04-17 22:56:12.714779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-04-17 22:56:12.742779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-04-17 22:56:12.778779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-04-17 22:56:12.810779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-04-17 22:55:51.574736 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-04-17 22:56:12.838779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-04-17 22:55:52.314738 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-04-17 22:56:12.846779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-04-17 22:56:12.870779 windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-04-17 22:56:12.866779 windmill_api-1.88.0/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-04-17 22:56:12.886779 windmill_api-1.88.0/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2422 2023-04-17 22:56:12.906779 windmill_api-1.88.0/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-04-17 22:56:12.906779 windmill_api-1.88.0/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-04-17 22:55:51.790737 windmill_api-1.88.0/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-04-17 22:56:12.926779 windmill_api-1.88.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-04-17 22:56:12.926779 windmill_api-1.88.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0      203 2023-04-17 22:55:51.622736 windmill_api-1.88.0/windmill_api/models/runnable_type.py
+-rw-r--r--   0        0        0     4086 2023-04-17 22:56:12.990779 windmill_api-1.88.0/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-04-17 22:56:12.950779 windmill_api-1.88.0/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-04-17 22:56:12.970779 windmill_api-1.88.0/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     6220 2023-04-17 22:56:13.054779 windmill_api-1.88.0/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-04-17 22:56:13.010779 windmill_api-1.88.0/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-04-17 22:56:13.030779 windmill_api-1.88.0/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-04-17 22:55:51.570736 windmill_api-1.88.0/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-04-17 22:55:51.882737 windmill_api-1.88.0/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-04-17 22:56:13.054779 windmill_api-1.88.0/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-04-17 22:56:13.078779 windmill_api-1.88.0/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-04-17 22:56:13.078779 windmill_api-1.88.0/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-04-17 22:56:13.106779 windmill_api-1.88.0/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-04-17 22:56:13.102779 windmill_api-1.88.0/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-04-17 22:56:13.142779 windmill_api-1.88.0/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      185 2023-04-17 22:55:52.046737 windmill_api-1.88.0/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-04-17 22:56:13.138779 windmill_api-1.88.0/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-04-17 22:55:51.446736 windmill_api-1.88.0/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-04-17 22:56:13.178779 windmill_api-1.88.0/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-04-17 22:56:13.186779 windmill_api-1.88.0/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-04-17 22:56:13.214779 windmill_api-1.88.0/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      187 2023-04-17 22:55:51.754737 windmill_api-1.88.0/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-04-17 22:56:13.254779 windmill_api-1.88.0/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-04-17 22:56:13.302780 windmill_api-1.88.0/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-04-17 22:55:51.822737 windmill_api-1.88.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-04-17 22:56:13.286779 windmill_api-1.88.0/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-04-17 22:56:13.306779 windmill_api-1.88.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-04-17 22:56:13.410780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-04-17 22:56:13.326780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-04-17 22:56:13.370780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-04-17 22:56:13.458780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-04-17 22:56:13.466780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-04-17 22:56:13.486780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-04-17 22:56:13.502780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-04-17 22:56:13.518780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-17 22:55:52.458738 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-04-17 22:56:13.530780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-17 22:55:52.078737 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-04-17 22:56:13.550780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-04-17 22:56:13.562780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-04-17 22:56:13.634780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-04-17 22:56:13.602780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-04-17 22:56:13.630780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-04-17 22:56:13.666780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-04-17 22:56:13.770780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-04-17 22:55:51.894737 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-04-17 22:56:13.694780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-04-17 22:55:51.482736 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-04-17 22:56:13.722780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-04-17 22:56:13.754780 windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-04-17 22:56:13.798780 windmill_api-1.88.0/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-04-17 22:56:13.810780 windmill_api-1.88.0/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     1670 2023-04-17 22:56:13.830780 windmill_api-1.88.0/windmill_api/models/update_input.py
+-rw-r--r--   0        0        0     1716 2023-04-17 22:56:13.838780 windmill_api-1.88.0/windmill_api/models/update_input_json_body.py
+-rw-r--r--   0        0        0     2036 2023-04-17 22:56:13.862780 windmill_api-1.88.0/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-04-17 22:56:13.870780 windmill_api-1.88.0/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-04-17 22:56:13.890780 windmill_api-1.88.0/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-04-17 22:56:13.902780 windmill_api-1.88.0/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-04-17 22:56:13.910780 windmill_api-1.88.0/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-04-17 22:56:13.934780 windmill_api-1.88.0/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-04-17 22:56:13.946780 windmill_api-1.88.0/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-04-17 22:56:13.962780 windmill_api-1.88.0/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     4071 2023-04-17 22:56:14.010780 windmill_api-1.88.0/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-04-17 22:56:13.986780 windmill_api-1.88.0/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-04-17 22:56:14.018780 windmill_api-1.88.0/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-04-17 22:56:14.038780 windmill_api-1.88.0/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     4222 2023-04-17 22:56:14.082780 windmill_api-1.88.0/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-04-17 22:56:14.134781 windmill_api-1.88.0/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     4211 2023-04-17 22:56:14.142780 windmill_api-1.88.0/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-04-17 22:56:14.158780 windmill_api-1.88.0/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-04-17 22:56:14.182780 windmill_api-1.88.0/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-04-17 22:56:14.190780 windmill_api-1.88.0/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-04-17 22:56:14.214780 windmill_api-1.88.0/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-04-17 22:55:41.926713 windmill_api-1.88.0/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-04-17 22:56:14.206781 windmill_api-1.88.0/windmill_api/types.py
+-rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 windmill_api-1.88.0/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.88.0/PKG-INFO
```

### Comparing `windmill_api-1.87.0/LICENSE` & `windmill_api-1.88.0/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/README.md` & `windmill_api-1.88.0/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/pyproject.toml` & `windmill_api-1.88.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windmill-api"
-version = "1.87.0"
+version = "1.88.0"
 description = "A client library for accessing Windmill API"
 license = "Apache-2.0"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
 readme = "README.md"
 packages = [
```

### Comparing `windmill_api-1.87.0/windmill_api/api/app/create_app.py` & `windmill_api-1.88.0/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/delete_app.py` & `windmill_api-1.88.0/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/execute_component.py` & `windmill_api-1.88.0/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/exists_app.py` & `windmill_api-1.88.0/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.88.0/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.88.0/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.88.0/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.88.0/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.88.0/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/list_apps.py` & `windmill_api-1.88.0/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.88.0/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/app/update_app.py` & `windmill_api-1.88.0/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.88.0/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.88.0/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/capture/create_capture.py` & `windmill_api-1.88.0/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/capture/get_capture.py` & `windmill_api-1.88.0/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/capture/update_capture.py` & `windmill_api-1.88.0/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/favorite/star.py` & `windmill_api-1.88.0/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/favorite/unstar.py` & `windmill_api-1.88.0/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.88.0/windmill_api/api/resource/delete_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 def _get_kwargs(
     workspace: str,
     path: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/w/{workspace}/flows/archive/{path}".format(client.base_url, workspace=workspace, path=path)
+    url = "{}/w/{workspace}/resources/delete/{path}".format(client.base_url, workspace=workspace, path=path)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "post",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
@@ -37,15 +37,15 @@
 
 def sync_detailed(
     workspace: str,
     path: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """archive flow by path
+    """delete resource
 
     Args:
         workspace (str):
         path (str):
 
     Returns:
         Response[Any]
@@ -67,15 +67,15 @@
 
 async def asyncio_detailed(
     workspace: str,
     path: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """archive flow by path
+    """delete resource
 
     Args:
         workspace (str):
         path (str):
 
     Returns:
         Response[Any]
```

### Comparing `windmill_api-1.87.0/windmill_api/api/flow/create_flow.py` & `windmill_api-1.88.0/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.88.0/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.88.0/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.88.0/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.88.0/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.88.0/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/flow/list_flows.py` & `windmill_api-1.88.0/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.88.0/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/flow/update_flow.py` & `windmill_api-1.88.0/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.88.0/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/folder/create_folder.py` & `windmill_api-1.88.0/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.88.0/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/folder/get_folder.py` & `windmill_api-1.88.0/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.88.0/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.88.0/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/folder/list_folders.py` & `windmill_api-1.88.0/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.88.0/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/folder/update_folder.py` & `windmill_api-1.88.0/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.88.0/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.88.0/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.88.0/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.88.0/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/group/create_group.py` & `windmill_api-1.88.0/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/group/delete_group.py` & `windmill_api-1.88.0/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/group/get_group.py` & `windmill_api-1.88.0/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/group/list_group_names.py` & `windmill_api-1.88.0/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/group/list_groups.py` & `windmill_api-1.88.0/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.88.0/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/group/update_group.py` & `windmill_api-1.88.0/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.88.0/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.88.0/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.88.0/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.88.0/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.88.0/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.88.0/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.88.0/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.88.0/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/get_job.py` & `windmill_api-1.88.0/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.88.0/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.88.0/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.88.0/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.88.0/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/list_jobs.py` & `windmill_api-1.88.0/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/list_queue.py` & `windmill_api-1.88.0/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/result_by_id.py` & `windmill_api-1.88.0/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.88.0/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.88.0/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.88.0/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.88.0/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.88.0/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.88.0/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.88.0/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.88.0/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/run_wait_result_flow_by_path.py` & `windmill_api-1.88.0/windmill_api/api/job/run_wait_result_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.88.0/windmill_api/api/job/run_wait_result_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/job/run_wait_result_script_by_path_get.py` & `windmill_api-1.88.0/windmill_api/api/job/run_wait_result_script_by_path_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.88.0/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.88.0/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/oauth/create_account.py` & `windmill_api-1.88.0/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.88.0/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.88.0/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.88.0/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.88.0/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.88.0/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/create_resource.py` & `windmill_api-1.88.0/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.88.0/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.88.0/windmill_api/api/resource/get_resource_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 def _get_kwargs(
     workspace: str,
     path: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/w/{workspace}/resources/delete/{path}".format(client.base_url, workspace=workspace, path=path)
+    url = "{}/w/{workspace}/resources/get_value/{path}".format(client.base_url, workspace=workspace, path=path)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "delete",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
@@ -37,15 +37,15 @@
 
 def sync_detailed(
     workspace: str,
     path: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """delete resource
+    """get resource value
 
     Args:
         workspace (str):
         path (str):
 
     Returns:
         Response[Any]
@@ -67,15 +67,15 @@
 
 async def asyncio_detailed(
     workspace: str,
     path: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """delete resource
+    """get resource value
 
     Args:
         workspace (str):
         path (str):
 
     Returns:
         Response[Any]
```

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.88.0/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.88.0/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.88.0/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/get_resource.py` & `windmill_api-1.88.0/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.88.0/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.88.0/windmill_api/api/user/get_usage.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 import httpx
 
 from ...client import Client
 from ...types import Response
 
 
 def _get_kwargs(
-    workspace: str,
-    path: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/w/{workspace}/resources/get_value/{path}".format(client.base_url, workspace=workspace, path=path)
+    url = "{}/users/usage".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
@@ -32,62 +30,46 @@
         content=response.content,
         headers=response.headers,
         parsed=None,
     )
 
 
 def sync_detailed(
-    workspace: str,
-    path: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """get resource value
-
-    Args:
-        workspace (str):
-        path (str):
+    """get current usage outside of premium workspaces
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
-        workspace=workspace,
-        path=path,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 async def asyncio_detailed(
-    workspace: str,
-    path: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """get resource value
-
-    Args:
-        workspace (str):
-        path (str):
+    """get current usage outside of premium workspaces
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
-        workspace=workspace,
-        path=path,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
```

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/list_resource.py` & `windmill_api-1.88.0/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.88.0/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.88.0/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/update_resource.py` & `windmill_api-1.88.0/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.88.0/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.88.0/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.88.0/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.88.0/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.88.0/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.88.0/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.88.0/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.88.0/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.88.0/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.88.0/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.88.0/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.88.0/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.88.0/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/create_script.py` & `windmill_api-1.88.0/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.88.0/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.88.0/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.88.0/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.88.0/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.88.0/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.88.0/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.88.0/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.88.0/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.88.0/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.88.0/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.88.0/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.88.0/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/list_scripts.py` & `windmill_api-1.88.0/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.88.0/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.88.0/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.88.0/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/script/raw_script_by_path_tokened.py` & `windmill_api-1.88.0/windmill_api/api/script/raw_script_by_path_tokened.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/settings/backend_version.py` & `windmill_api-1.88.0/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.88.0/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/accept_invite.py` & `windmill_api-1.88.0/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/create_token.py` & `windmill_api-1.88.0/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/create_token_impersonate.py` & `windmill_api-1.88.0/windmill_api/api/user/create_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/create_user.py` & `windmill_api-1.88.0/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.88.0/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/decline_invite.py` & `windmill_api-1.88.0/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/delete_token.py` & `windmill_api-1.88.0/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/delete_user.py` & `windmill_api-1.88.0/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/get_current_email.py` & `windmill_api-1.88.0/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/get_usage.py` & `windmill_api-1.88.0/windmill_api/api/user/logout.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/users/usage".format(client.base_url)
+    url = "{}/auth/logout".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "get",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
@@ -33,15 +33,15 @@
     )
 
 
 def sync_detailed(
     *,
     client: Client,
 ) -> Response[Any]:
-    """get current usage outside of premium workspaces
+    """logout
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
         client=client,
@@ -55,15 +55,15 @@
     return _build_response(response=response)
 
 
 async def asyncio_detailed(
     *,
     client: Client,
 ) -> Response[Any]:
-    """get current usage outside of premium workspaces
+    """logout
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
         client=client,
```

### Comparing `windmill_api-1.87.0/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.88.0/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/global_user_update.py` & `windmill_api-1.88.0/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/global_whoami.py` & `windmill_api-1.88.0/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.88.0/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.88.0/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/list_tokens.py` & `windmill_api-1.88.0/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/list_usernames.py` & `windmill_api-1.88.0/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/list_users.py` & `windmill_api-1.88.0/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.88.0/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.88.0/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/login.py` & `windmill_api-1.88.0/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.88.0/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/logout.py` & `windmill_api-1.88.0/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,114 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, cast
 
 import httpx
 
 from ...client import Client
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/auth/logout".format(client.base_url)
+    url = "{}/workspaces/allowed_domain_auto_invite".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _parse_response(*, response: httpx.Response) -> Optional[bool]:
+    if response.status_code == 200:
+        response_200 = cast(bool, response.json())
+        return response_200
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[bool]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Any]:
-    """logout
+) -> Response[bool]:
+    """is domain allowed for auto invi
 
     Returns:
-        Response[Any]
+        Response[bool]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
+def sync(
+    *,
+    client: Client,
+) -> Optional[bool]:
+    """is domain allowed for auto invi
+
+    Returns:
+        Response[bool]
+    """
+
+    return sync_detailed(
+        client=client,
+    ).parsed
+
+
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Any]:
-    """logout
+) -> Response[bool]:
+    """is domain allowed for auto invi
 
     Returns:
-        Response[Any]
+        Response[bool]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
+
+
+async def asyncio(
+    *,
+    client: Client,
+) -> Optional[bool]:
+    """is domain allowed for auto invi
+
+    Returns:
+        Response[bool]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `windmill_api-1.87.0/windmill_api/api/user/set_password.py` & `windmill_api-1.88.0/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/update_user.py` & `windmill_api-1.88.0/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/whoami.py` & `windmill_api-1.88.0/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/user/whois.py` & `windmill_api-1.88.0/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/variable/create_variable.py` & `windmill_api-1.88.0/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.88.0/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.88.0/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/variable/get_variable.py` & `windmill_api-1.88.0/windmill_api/api/variable/get_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.88.0/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/variable/list_variable.py` & `windmill_api-1.88.0/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/variable/update_variable.py` & `windmill_api-1.88.0/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/worker/list_workers.py` & `windmill_api-1.88.0/windmill_api/api/worker/list_workers.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/add_user.py` & `windmill_api-1.88.0/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.88.0/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.88.0/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.88.0/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.88.0/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.88.0/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.88.0/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.88.0/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.88.0/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.88.0/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.88.0/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.88.0/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.88.0/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.88.0/windmill_api/api/workspace/list_workspaces.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,64 @@
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, List, Optional
 
 import httpx
 
 from ...client import Client
+from ...models.list_workspaces_response_200_item import ListWorkspacesResponse200Item
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/workspaces/allowed_domain_auto_invite".format(client.base_url)
+    url = "{}/workspaces/list".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[bool]:
+def _parse_response(*, response: httpx.Response) -> Optional[List[ListWorkspacesResponse200Item]]:
     if response.status_code == 200:
-        response_200 = cast(bool, response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = ListWorkspacesResponse200Item.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
+
         return response_200
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[bool]:
+def _build_response(*, response: httpx.Response) -> Response[List[ListWorkspacesResponse200Item]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[bool]:
-    """is domain allowed for auto invi
+) -> Response[List[ListWorkspacesResponse200Item]]:
+    """list all workspaces visible to me
 
     Returns:
-        Response[bool]
+        Response[List[ListWorkspacesResponse200Item]]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
@@ -61,34 +68,34 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[bool]:
-    """is domain allowed for auto invi
+) -> Optional[List[ListWorkspacesResponse200Item]]:
+    """list all workspaces visible to me
 
     Returns:
-        Response[bool]
+        Response[List[ListWorkspacesResponse200Item]]
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[bool]:
-    """is domain allowed for auto invi
+) -> Response[List[ListWorkspacesResponse200Item]]:
+    """list all workspaces visible to me
 
     Returns:
-        Response[bool]
+        Response[List[ListWorkspacesResponse200Item]]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -96,19 +103,19 @@
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[bool]:
-    """is domain allowed for auto invi
+) -> Optional[List[ListWorkspacesResponse200Item]]:
+    """list all workspaces visible to me
 
     Returns:
-        Response[bool]
+        Response[List[ListWorkspacesResponse200Item]]
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.88.0/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.88.0/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py` & `windmill_api-1.88.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.88.0/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/client.py` & `windmill_api-1.88.0/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.88.0/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.88.0/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.88.0/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/add_user_json_body.py` & `windmill_api-1.88.0/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.88.0/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/app_with_last_version.py` & `windmill_api-1.88.0/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.88.0/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.88.0/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.88.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.88.0/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.88.0/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/audit_log.py` & `windmill_api-1.88.0/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/audit_log_operation.py` & `windmill_api-1.88.0/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.88.0/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.88.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_all.py` & `windmill_api-1.88.0/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.88.0/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one.py` & `windmill_api-1.88.0/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.88.0/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.88.0/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job.py` & `windmill_api-1.88.0/windmill_api/models/completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_args.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.88.0/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.88.0/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.88.0/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/contextual_variable.py` & `windmill_api-1.88.0/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_account_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_app_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.88.0/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.88.0/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.88.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_schema.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_group_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_resource.py` & `windmill_api-1.88.0/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.88.0/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_script_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_script_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.88.0/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_token_impersonate_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_token_impersonate_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_token_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_user_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_variable.py` & `windmill_api-1.88.0/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_workspace.py` & `windmill_api-1.88.0/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.88.0/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.88.0/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.88.0/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.88.0/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.88.0/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.88.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.88.0/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/edit_resource.py` & `windmill_api-1.88.0/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/edit_resource_type.py` & `windmill_api-1.88.0/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/edit_schedule.py` & `windmill_api-1.88.0/windmill_api/models/edit_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.88.0/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.88.0/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/edit_variable.py` & `windmill_api-1.88.0/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.88.0/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.88.0/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.88.0/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.88.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.88.0/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.88.0/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.88.0/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow.py` & `windmill_api-1.88.0/windmill_api/models/flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_metadata.py` & `windmill_api-1.88.0/windmill_api/models/flow_metadata.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module.py` & `windmill_api-1.88.0/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.88.0/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_args.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_schema.py` & `windmill_api-1.88.0/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status.py` & `windmill_api-1.88.0/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_module.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_status_retry.py` & `windmill_api-1.88.0/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value.py` & `windmill_api-1.88.0/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/folder.py` & `windmill_api-1.88.0/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.88.0/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.88.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.88.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.88.0/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.88.0/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_group_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_job_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.88.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_schedule_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.88.0/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.88.0/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.88.0/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.88.0/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.88.0/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/global_user_info.py` & `windmill_api-1.88.0/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.88.0/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.88.0/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.88.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/group.py` & `windmill_api-1.88.0/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/group_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/identity.py` & `windmill_api-1.88.0/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.88.0/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.88.0/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.88.0/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/javascript_transform.py` & `windmill_api-1.88.0/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/job.py` & `windmill_api-1.88.0/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.88.0/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.88.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_schema.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.88.0/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.88.0/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.88.0/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.88.0/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.88.0/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.88.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_schedules_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.88.0/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_scripts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.88.0/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.88.0/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.88.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/whoami_response_200.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.list_users_response_200_item_usage import ListUsersResponse200ItemUsage
+from ..models.whoami_response_200_usage import WhoamiResponse200Usage
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListUsersResponse200Item")
+T = TypeVar("T", bound="WhoamiResponse200")
 
 
 @attr.s(auto_attribs=True)
-class ListUsersResponse200Item:
+class WhoamiResponse200:
     """
     Attributes:
         email (str):
         username (str):
         is_admin (bool):
         is_super_admin (bool):
         created_at (datetime.datetime):
         operator (bool):
         disabled (bool):
         folders (List[str]):
+        folders_owners (List[str]):
         groups (Union[Unset, List[str]]):
-        usage (Union[Unset, ListUsersResponse200ItemUsage]):
+        usage (Union[Unset, WhoamiResponse200Usage]):
     """
 
     email: str
     username: str
     is_admin: bool
     is_super_admin: bool
     created_at: datetime.datetime
     operator: bool
     disabled: bool
     folders: List[str]
+    folders_owners: List[str]
     groups: Union[Unset, List[str]] = UNSET
-    usage: Union[Unset, ListUsersResponse200ItemUsage] = UNSET
+    usage: Union[Unset, WhoamiResponse200Usage] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         email = self.email
         username = self.username
         is_admin = self.is_admin
         is_super_admin = self.is_super_admin
         created_at = self.created_at.isoformat()
 
         operator = self.operator
         disabled = self.disabled
         folders = self.folders
 
+        folders_owners = self.folders_owners
+
         groups: Union[Unset, List[str]] = UNSET
         if not isinstance(self.groups, Unset):
             groups = self.groups
 
         usage: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.usage, Unset):
             usage = self.usage.to_dict()
@@ -65,14 +69,15 @@
                 "username": username,
                 "is_admin": is_admin,
                 "is_super_admin": is_super_admin,
                 "created_at": created_at,
                 "operator": operator,
                 "disabled": disabled,
                 "folders": folders,
+                "folders_owners": folders_owners,
             }
         )
         if groups is not UNSET:
             field_dict["groups"] = groups
         if usage is not UNSET:
             field_dict["usage"] = usage
 
@@ -93,38 +98,41 @@
 
         operator = d.pop("operator")
 
         disabled = d.pop("disabled")
 
         folders = cast(List[str], d.pop("folders"))
 
+        folders_owners = cast(List[str], d.pop("folders_owners"))
+
         groups = cast(List[str], d.pop("groups", UNSET))
 
         _usage = d.pop("usage", UNSET)
-        usage: Union[Unset, ListUsersResponse200ItemUsage]
+        usage: Union[Unset, WhoamiResponse200Usage]
         if isinstance(_usage, Unset):
             usage = UNSET
         else:
-            usage = ListUsersResponse200ItemUsage.from_dict(_usage)
+            usage = WhoamiResponse200Usage.from_dict(_usage)
 
-        list_users_response_200_item = cls(
+        whoami_response_200 = cls(
             email=email,
             username=username,
             is_admin=is_admin,
             is_super_admin=is_super_admin,
             created_at=created_at,
             operator=operator,
             disabled=disabled,
             folders=folders,
+            folders_owners=folders_owners,
             groups=groups,
             usage=usage,
         )
 
-        list_users_response_200_item.additional_properties = d
-        return list_users_response_200_item
+        whoami_response_200.additional_properties = d
+        return whoami_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.87.0/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.88.0/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.88.0/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/listable_app.py` & `windmill_api-1.88.0/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/listable_resource.py` & `windmill_api-1.88.0/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/listable_variable.py` & `windmill_api-1.88.0/windmill_api/models/listable_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/login.py` & `windmill_api-1.88.0/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/login_json_body.py` & `windmill_api-1.88.0/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.88.0/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/main_arg_signature.py` & `windmill_api-1.88.0/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.88.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/new_schedule.py` & `windmill_api-1.88.0/windmill_api/models/new_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/new_schedule_args.py` & `windmill_api-1.88.0/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/new_token.py` & `windmill_api-1.88.0/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/new_token_impersonate.py` & `windmill_api-1.88.0/windmill_api/models/new_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/new_user.py` & `windmill_api-1.88.0/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow.py` & `windmill_api-1.88.0/windmill_api/models/open_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_schema.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/path_flow.py` & `windmill_api-1.88.0/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.88.0/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.88.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.88.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/path_script.py` & `windmill_api-1.88.0/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.88.0/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.88.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.88.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/policy.py` & `windmill_api-1.88.0/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/policy_triggerables.py` & `windmill_api-1.88.0/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.88.0/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/preview.py` & `windmill_api-1.88.0/windmill_api/models/preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/preview_args.py` & `windmill_api-1.88.0/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.88.0/windmill_api/models/preview_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.88.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job.py` & `windmill_api-1.88.0/windmill_api/models/queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_args.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/raw_script.py` & `windmill_api-1.88.0/windmill_api/models/raw_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.88.0/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.88.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.88.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.88.0/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.88.0/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.88.0/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.88.0/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/resource.py` & `windmill_api-1.88.0/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/resource_type.py` & `windmill_api-1.88.0/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.88.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.88.0/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/retry.py` & `windmill_api-1.88.0/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.88.0/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.88.0/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.88.0/windmill_api/models/run_script_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.88.0/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.88.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.88.0/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/schedule.py` & `windmill_api-1.88.0/windmill_api/models/schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/schedule_args.py` & `windmill_api-1.88.0/windmill_api/models/schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/schedule_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/script.py` & `windmill_api-1.88.0/windmill_api/models/script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/script_args.py` & `windmill_api-1.88.0/windmill_api/models/script_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/script_extra_perms.py` & `windmill_api-1.88.0/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/script_schema.py` & `windmill_api-1.88.0/windmill_api/models/script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/set_password_json_body.py` & `windmill_api-1.88.0/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.88.0/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/slack_token.py` & `windmill_api-1.88.0/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/slack_token_bot.py` & `windmill_api-1.88.0/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/star_json_body.py` & `windmill_api-1.88.0/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/static_transform.py` & `windmill_api-1.88.0/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/token_response.py` & `windmill_api-1.88.0/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/truncated_token.py` & `windmill_api-1.88.0/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/unstar_json_body.py` & `windmill_api-1.88.0/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_app_json_body.py` & `windmill_api-1.88.0/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.88.0/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.88.0/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.88.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.88.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.88.0/windmill_api/models/update_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_group_json_body.py` & `windmill_api-1.88.0/windmill_api/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.88.0/windmill_api/models/update_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_resource_type_json_body.py` & `windmill_api-1.88.0/windmill_api/models/update_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.88.0/windmill_api/models/update_resource_value_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_schedule_json_body.py` & `windmill_api-1.88.0/windmill_api/models/update_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.88.0/windmill_api/models/update_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_user_json_body.py` & `windmill_api-1.88.0/windmill_api/models/update_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/update_variable_json_body.py` & `windmill_api-1.88.0/windmill_api/models/update_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/usage.py` & `windmill_api-1.88.0/windmill_api/models/usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/user.py` & `windmill_api-1.88.0/windmill_api/models/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,26 +18,28 @@
         username (str):
         is_admin (bool):
         is_super_admin (bool):
         created_at (datetime.datetime):
         operator (bool):
         disabled (bool):
         folders (List[str]):
+        folders_owners (List[str]):
         groups (Union[Unset, List[str]]):
         usage (Union[Unset, UserUsage]):
     """
 
     email: str
     username: str
     is_admin: bool
     is_super_admin: bool
     created_at: datetime.datetime
     operator: bool
     disabled: bool
     folders: List[str]
+    folders_owners: List[str]
     groups: Union[Unset, List[str]] = UNSET
     usage: Union[Unset, UserUsage] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         email = self.email
         username = self.username
@@ -45,14 +47,16 @@
         is_super_admin = self.is_super_admin
         created_at = self.created_at.isoformat()
 
         operator = self.operator
         disabled = self.disabled
         folders = self.folders
 
+        folders_owners = self.folders_owners
+
         groups: Union[Unset, List[str]] = UNSET
         if not isinstance(self.groups, Unset):
             groups = self.groups
 
         usage: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.usage, Unset):
             usage = self.usage.to_dict()
@@ -65,14 +69,15 @@
                 "username": username,
                 "is_admin": is_admin,
                 "is_super_admin": is_super_admin,
                 "created_at": created_at,
                 "operator": operator,
                 "disabled": disabled,
                 "folders": folders,
+                "folders_owners": folders_owners,
             }
         )
         if groups is not UNSET:
             field_dict["groups"] = groups
         if usage is not UNSET:
             field_dict["usage"] = usage
 
@@ -93,14 +98,16 @@
 
         operator = d.pop("operator")
 
         disabled = d.pop("disabled")
 
         folders = cast(List[str], d.pop("folders"))
 
+        folders_owners = cast(List[str], d.pop("folders_owners"))
+
         groups = cast(List[str], d.pop("groups", UNSET))
 
         _usage = d.pop("usage", UNSET)
         usage: Union[Unset, UserUsage]
         if isinstance(_usage, Unset):
             usage = UNSET
         else:
@@ -111,14 +118,15 @@
             username=username,
             is_admin=is_admin,
             is_super_admin=is_super_admin,
             created_at=created_at,
             operator=operator,
             disabled=disabled,
             folders=folders,
+            folders_owners=folders_owners,
             groups=groups,
             usage=usage,
         )
 
         user.additional_properties = d
         return user
```

### Comparing `windmill_api-1.87.0/windmill_api/models/user_usage.py` & `windmill_api-1.88.0/windmill_api/models/user_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/user_workspace_list.py` & `windmill_api-1.88.0/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.88.0/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/whoami_response_200.py` & `windmill_api-1.88.0/windmill_api/models/whois_response_200.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.whoami_response_200_usage import WhoamiResponse200Usage
+from ..models.whois_response_200_usage import WhoisResponse200Usage
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="WhoamiResponse200")
+T = TypeVar("T", bound="WhoisResponse200")
 
 
 @attr.s(auto_attribs=True)
-class WhoamiResponse200:
+class WhoisResponse200:
     """
     Attributes:
         email (str):
         username (str):
         is_admin (bool):
         is_super_admin (bool):
         created_at (datetime.datetime):
         operator (bool):
         disabled (bool):
         folders (List[str]):
+        folders_owners (List[str]):
         groups (Union[Unset, List[str]]):
-        usage (Union[Unset, WhoamiResponse200Usage]):
+        usage (Union[Unset, WhoisResponse200Usage]):
     """
 
     email: str
     username: str
     is_admin: bool
     is_super_admin: bool
     created_at: datetime.datetime
     operator: bool
     disabled: bool
     folders: List[str]
+    folders_owners: List[str]
     groups: Union[Unset, List[str]] = UNSET
-    usage: Union[Unset, WhoamiResponse200Usage] = UNSET
+    usage: Union[Unset, WhoisResponse200Usage] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         email = self.email
         username = self.username
         is_admin = self.is_admin
         is_super_admin = self.is_super_admin
         created_at = self.created_at.isoformat()
 
         operator = self.operator
         disabled = self.disabled
         folders = self.folders
 
+        folders_owners = self.folders_owners
+
         groups: Union[Unset, List[str]] = UNSET
         if not isinstance(self.groups, Unset):
             groups = self.groups
 
         usage: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.usage, Unset):
             usage = self.usage.to_dict()
@@ -65,14 +69,15 @@
                 "username": username,
                 "is_admin": is_admin,
                 "is_super_admin": is_super_admin,
                 "created_at": created_at,
                 "operator": operator,
                 "disabled": disabled,
                 "folders": folders,
+                "folders_owners": folders_owners,
             }
         )
         if groups is not UNSET:
             field_dict["groups"] = groups
         if usage is not UNSET:
             field_dict["usage"] = usage
 
@@ -93,38 +98,41 @@
 
         operator = d.pop("operator")
 
         disabled = d.pop("disabled")
 
         folders = cast(List[str], d.pop("folders"))
 
+        folders_owners = cast(List[str], d.pop("folders_owners"))
+
         groups = cast(List[str], d.pop("groups", UNSET))
 
         _usage = d.pop("usage", UNSET)
-        usage: Union[Unset, WhoamiResponse200Usage]
+        usage: Union[Unset, WhoisResponse200Usage]
         if isinstance(_usage, Unset):
             usage = UNSET
         else:
-            usage = WhoamiResponse200Usage.from_dict(_usage)
+            usage = WhoisResponse200Usage.from_dict(_usage)
 
-        whoami_response_200 = cls(
+        whois_response_200 = cls(
             email=email,
             username=username,
             is_admin=is_admin,
             is_super_admin=is_super_admin,
             created_at=created_at,
             operator=operator,
             disabled=disabled,
             folders=folders,
+            folders_owners=folders_owners,
             groups=groups,
             usage=usage,
         )
 
-        whoami_response_200.additional_properties = d
-        return whoami_response_200
+        whois_response_200.additional_properties = d
+        return whois_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.87.0/windmill_api/models/whoami_response_200_usage.py` & `windmill_api-1.88.0/windmill_api/models/whoami_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/whois_response_200.py` & `windmill_api-1.88.0/windmill_api/models/list_users_response_200_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.whois_response_200_usage import WhoisResponse200Usage
+from ..models.list_users_response_200_item_usage import ListUsersResponse200ItemUsage
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="WhoisResponse200")
+T = TypeVar("T", bound="ListUsersResponse200Item")
 
 
 @attr.s(auto_attribs=True)
-class WhoisResponse200:
+class ListUsersResponse200Item:
     """
     Attributes:
         email (str):
         username (str):
         is_admin (bool):
         is_super_admin (bool):
         created_at (datetime.datetime):
         operator (bool):
         disabled (bool):
         folders (List[str]):
+        folders_owners (List[str]):
         groups (Union[Unset, List[str]]):
-        usage (Union[Unset, WhoisResponse200Usage]):
+        usage (Union[Unset, ListUsersResponse200ItemUsage]):
     """
 
     email: str
     username: str
     is_admin: bool
     is_super_admin: bool
     created_at: datetime.datetime
     operator: bool
     disabled: bool
     folders: List[str]
+    folders_owners: List[str]
     groups: Union[Unset, List[str]] = UNSET
-    usage: Union[Unset, WhoisResponse200Usage] = UNSET
+    usage: Union[Unset, ListUsersResponse200ItemUsage] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         email = self.email
         username = self.username
         is_admin = self.is_admin
         is_super_admin = self.is_super_admin
         created_at = self.created_at.isoformat()
 
         operator = self.operator
         disabled = self.disabled
         folders = self.folders
 
+        folders_owners = self.folders_owners
+
         groups: Union[Unset, List[str]] = UNSET
         if not isinstance(self.groups, Unset):
             groups = self.groups
 
         usage: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.usage, Unset):
             usage = self.usage.to_dict()
@@ -65,14 +69,15 @@
                 "username": username,
                 "is_admin": is_admin,
                 "is_super_admin": is_super_admin,
                 "created_at": created_at,
                 "operator": operator,
                 "disabled": disabled,
                 "folders": folders,
+                "folders_owners": folders_owners,
             }
         )
         if groups is not UNSET:
             field_dict["groups"] = groups
         if usage is not UNSET:
             field_dict["usage"] = usage
 
@@ -93,38 +98,41 @@
 
         operator = d.pop("operator")
 
         disabled = d.pop("disabled")
 
         folders = cast(List[str], d.pop("folders"))
 
+        folders_owners = cast(List[str], d.pop("folders_owners"))
+
         groups = cast(List[str], d.pop("groups", UNSET))
 
         _usage = d.pop("usage", UNSET)
-        usage: Union[Unset, WhoisResponse200Usage]
+        usage: Union[Unset, ListUsersResponse200ItemUsage]
         if isinstance(_usage, Unset):
             usage = UNSET
         else:
-            usage = WhoisResponse200Usage.from_dict(_usage)
+            usage = ListUsersResponse200ItemUsage.from_dict(_usage)
 
-        whois_response_200 = cls(
+        list_users_response_200_item = cls(
             email=email,
             username=username,
             is_admin=is_admin,
             is_super_admin=is_super_admin,
             created_at=created_at,
             operator=operator,
             disabled=disabled,
             folders=folders,
+            folders_owners=folders_owners,
             groups=groups,
             usage=usage,
         )
 
-        whois_response_200.additional_properties = d
-        return whois_response_200
+        list_users_response_200_item.additional_properties = d
+        return list_users_response_200_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.87.0/windmill_api/models/whois_response_200_usage.py` & `windmill_api-1.88.0/windmill_api/models/whois_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/worker_ping.py` & `windmill_api-1.88.0/windmill_api/models/worker_ping.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/workspace.py` & `windmill_api-1.88.0/windmill_api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/models/workspace_invite.py` & `windmill_api-1.88.0/windmill_api/models/workspace_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/windmill_api/types.py` & `windmill_api-1.88.0/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.87.0/setup.py` & `windmill_api-1.88.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
  'windmill_api.api.audit',
  'windmill_api.api.capture',
  'windmill_api.api.favorite',
  'windmill_api.api.flow',
  'windmill_api.api.folder',
  'windmill_api.api.granular_acl',
  'windmill_api.api.group',
+ 'windmill_api.api.input_',
  'windmill_api.api.job',
  'windmill_api.api.oauth',
  'windmill_api.api.resource',
  'windmill_api.api.schedule',
  'windmill_api.api.script',
  'windmill_api.api.settings',
  'windmill_api.api.user',
@@ -28,15 +29,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.87.0',
+    'version': '1.88.0',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.87.0/PKG-INFO` & `windmill_api-1.88.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.87.0
+Version: 1.88.0
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

