# Comparing `tmp/tmlt_analytics-0.6.1.tar.gz` & `tmp/tmlt_analytics-0.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmlt_analytics-0.6.1.tar", max compression
+gzip compressed data, was "tmlt_analytics-0.7.0rc1.tar", max compression
```

## Comparing `tmlt_analytics-0.6.1.tar` & `tmlt_analytics-0.7.0rc1.tar`

### file list

```diff
@@ -1,115 +1,159 @@
--rw-r--r--   0        0        0    10749 2022-12-07 22:19:17.160494 tmlt_analytics-0.6.1/CHANGELOG.rst
--rw-r--r--   0        0        0    11358 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/LICENSE
--rw-r--r--   0        0        0    20138 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/LICENSE.docs
--rw-r--r--   0        0        0      121 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/NOTICE
--rw-r--r--   0        0        0     1611 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/README.md
--rw-r--r--   0        0        0      951 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/_static/css/custom.css
--rw-r--r--   0        0        0    12470 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/_static/favicon.ico
--rw-r--r--   0        0        0     1001 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/_static/js/version-banner.js
--rw-r--r--   0        0        0    30903 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/_static/logo.png
--rw-r--r--   0        0        0       50 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/_templates/build-info.html
--rw-r--r--   0        0        0      408 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/_templates/layout.html
--rw-r--r--   0        0        0       23 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/_templates/package-name.html
--rw-r--r--   0        0        0      192 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/additional-resources/index.rst
--rw-r--r--   0        0        0      670 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/additional-resources/license.rst
--rw-r--r--   0        0        0     3159 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/additional-resources/privacy_policy.rst
--rw-r--r--   0        0        0     6764 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/conf.py
--rw-r--r--   0        0        0   118378 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/images/api_diagram.svg
--rw-r--r--   0        0        0    85925 2022-12-07 20:43:07.622239 tmlt_analytics-0.6.1/doc/images/chart_age_at_joining.png
--rw-r--r--   0        0        0    27267 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_attacker_certainty.png
--rw-r--r--   0        0        0    41645 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_average_age_by_edu.png
--rw-r--r--   0        0        0   104926 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_counts_age_gender.png
--rw-r--r--   0        0        0    34006 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_counts_different_eps.png
--rw-r--r--   0        0        0    25097 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_counts_edu+sex.png
--rw-r--r--   0        0        0    13993 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_counts_education.png
--rw-r--r--   0        0        0    41034 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_error_vs_partition_age_edu.png
--rw-r--r--   0        0        0    65291 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_favorite_genres.png
--rw-r--r--   0        0        0    14310 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_filters_education.png
--rw-r--r--   0        0        0    14782 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_quantiles_education.png
--rw-r--r--   0        0        0    20853 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_senior_counts_1.png
--rw-r--r--   0        0        0    21067 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_senior_counts_2.png
--rw-r--r--   0        0        0    29335 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_teen_edu_counts.png
--rw-r--r--   0        0        0    20226 2022-12-07 20:43:07.626240 tmlt_analytics-0.6.1/doc/images/chart_younger_age_counts.png
--rw-r--r--   0        0        0    29155 2022-12-07 20:43:07.630240 tmlt_analytics-0.6.1/doc/images/clamping_bounds_averages.png
--rw-r--r--   0        0        0     9416 2022-12-07 20:43:07.630240 tmlt_analytics-0.6.1/doc/images/clamping_bounds_schema.png
--rw-r--r--   0        0        0    14685 2022-12-07 20:43:07.630240 tmlt_analytics-0.6.1/doc/images/histogram_books_borrowed.png
--rw-r--r--   0        0        0     1844 2022-12-07 20:43:07.630240 tmlt_analytics-0.6.1/doc/images/index_api.svg
--rw-r--r--   0        0        0     1196 2022-12-07 20:43:07.630240 tmlt_analytics-0.6.1/doc/images/index_more.svg
--rw-r--r--   0        0        0      604 2022-12-07 20:43:07.630240 tmlt_analytics-0.6.1/doc/images/index_topic_guides.svg
--rw-r--r--   0        0        0     1371 2022-12-07 20:43:07.630240 tmlt_analytics-0.6.1/doc/images/index_tutorials.svg
--rw-r--r--   0        0        0    30903 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/images/logo.png
--rw-r--r--   0        0        0     3871 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/index.rst
--rw-r--r--   0        0        0     4960 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/installation.rst
--rw-r--r--   0        0        0      662 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/intersphinx_mapping.json
--rw-r--r--   0        0        0     2029 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/templates/python/class.rst
--rw-r--r--   0        0        0     3440 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/templates/python/module.rst
--rw-r--r--   0        0        0      366 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/topic-guides/index.rst
--rw-r--r--   0        0        0    11697 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/topic-guides/nulls-nans-infinities.rst
--rw-r--r--   0        0        0     8608 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/topic-guides/privacy-budgets.rst
--rw-r--r--   0        0        0     5577 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/topic-guides/privacy-promise.rst
--rw-r--r--   0        0        0     6317 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/topic-guides/spark.rst
--rw-r--r--   0        0        0     8462 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/topic-guides/working-with-sessions.rst
--rw-r--r--   0        0        0     9124 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/tutorials/clamping-bounds.rst
--rw-r--r--   0        0        0     7246 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/tutorials/first-steps.rst
--rw-r--r--   0        0        0    18802 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/tutorials/groupby-queries.rst
--rw-r--r--   0        0        0      384 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/tutorials/index.rst
--rw-r--r--   0        0        0     7732 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/tutorials/privacy-budget-basics.rst
--rw-r--r--   0        0        0    16105 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/doc/tutorials/simple-transformations.rst
--rw-r--r--   0        0        0     4792 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/examples/interactive_evaluation.ipynb
--rw-r--r--   0        0        0     5459 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/examples/private_join.ipynb
--rw-r--r--   0        0        0     6570 2022-12-07 20:43:07.634240 tmlt_analytics-0.6.1/examples/zcdp_puredp_switching.ipynb
--rw-r--r--   0        0        0     4399 2022-12-07 22:19:58.825202 tmlt_analytics-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      108 2022-12-07 20:43:07.638241 tmlt_analytics-0.6.1/test/__init__.py
--rw-r--r--   0        0        0     6976 2022-12-07 20:43:07.638241 tmlt_analytics-0.6.1/test/conftest.py
--rw-r--r--   0        0        0      115 2022-12-07 20:43:07.638241 tmlt_analytics-0.6.1/test/system/__init__.py
--rw-r--r--   0        0        0    83597 2022-12-07 20:43:07.638241 tmlt_analytics-0.6.1/test/system/test_session.py
--rw-r--r--   0        0        0      108 2022-12-07 20:43:07.638241 tmlt_analytics-0.6.1/test/unit/__init__.py
--rw-r--r--   0        0        0      298 2022-12-07 20:43:07.638241 tmlt_analytics-0.6.1/test/unit/query_expr_compiler/__init__.py
--rw-r--r--   0        0        0    85945 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/query_expr_compiler/test_measurement_visitor.py
--rw-r--r--   0        0        0    55570 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/query_expr_compiler/test_output_schema_visitor.py
--rw-r--r--   0        0        0    43862 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/query_expr_compiler/test_transformation_visitor.py
--rw-r--r--   0        0        0    14133 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_binning_spec.py
--rw-r--r--   0        0        0     3335 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_catalog.py
--rw-r--r--   0        0        0      657 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_cleanup.py
--rw-r--r--   0        0        0    21155 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_keyset.py
--rw-r--r--   0        0        0     8974 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_neighboring_relations.py
--rw-r--r--   0        0        0     3058 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_noise_info.py
--rw-r--r--   0        0        0     2999 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_privacy_budget.py
--rw-r--r--   0        0        0     5420 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0     2331 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_protected_change.py
--rw-r--r--   0        0        0    39666 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_query_builder.py
--rw-r--r--   0        0        0    61013 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_query_expr_compiler.py
--rw-r--r--   0        0        0    16212 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_query_expression.py
--rw-r--r--   0        0        0     4660 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_query_expression_visitor.py
--rw-r--r--   0        0        0     2172 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_schema.py
--rw-r--r--   0        0        0    13538 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_schema_conversion.py
--rw-r--r--   0        0        0    59968 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_session.py
--rw-r--r--   0        0        0      792 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_truncation_strategy.py
--rw-r--r--   0        0        0      518 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test/unit/test_utils.py
--rw-r--r--   0        0        0       37 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/test_requirements.txt
--rw-r--r--   0        0        0      222 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/__init__.py
--rw-r--r--   0        0        0     6082 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_catalog.py
--rw-r--r--   0        0        0     3555 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_coerce_spark_schema.py
--rw-r--r--   0        0        0     5513 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_neighboring_relation_visitor.py
--rw-r--r--   0        0        0    11381 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_neighboring_relations.py
--rw-r--r--   0        0        0     5428 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_noise_info.py
--rw-r--r--   0        0        0     2289 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0      184 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_query_expr_compiler/__init__.py
--rw-r--r--   0        0        0     8548 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_query_expr_compiler/_compiler.py
--rw-r--r--   0        0        0    30088 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
--rw-r--r--   0        0        0    40227 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
--rw-r--r--   0        0        0    37560 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
--rw-r--r--   0        0        0    11590 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/_schema.py
--rw-r--r--   0        0        0    11663 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/binning_spec.py
--rw-r--r--   0        0        0      306 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/cleanup.py
--rw-r--r--   0        0        0    11844 2022-12-07 20:43:07.642241 tmlt_analytics-0.6.1/tmlt/analytics/keyset.py
--rw-r--r--   0        0        0     4222 2022-12-07 20:43:07.646242 tmlt_analytics-0.6.1/tmlt/analytics/privacy_budget.py
--rw-r--r--   0        0        0     3847 2022-12-07 20:43:07.646242 tmlt_analytics-0.6.1/tmlt/analytics/protected_change.py
--rw-r--r--   0        0        0        0 2022-12-07 20:43:07.646242 tmlt_analytics-0.6.1/tmlt/analytics/py.typed
--rw-r--r--   0        0        0   124569 2022-12-07 20:43:07.646242 tmlt_analytics-0.6.1/tmlt/analytics/query_builder.py
--rw-r--r--   0        0        0    40426 2022-12-07 20:43:07.646242 tmlt_analytics-0.6.1/tmlt/analytics/query_expr.py
--rw-r--r--   0        0        0    54586 2022-12-07 20:43:07.646242 tmlt_analytics-0.6.1/tmlt/analytics/session.py
--rw-r--r--   0        0        0     3031 2022-12-07 20:43:07.646242 tmlt_analytics-0.6.1/tmlt/analytics/truncation_strategy.py
--rw-r--r--   0        0        0     4772 2022-12-07 20:43:07.646242 tmlt_analytics-0.6.1/tmlt/analytics/utils.py
--rw-r--r--   0        0        0     2486 1970-01-01 00:00:00.000000 tmlt_analytics-0.6.1/setup.py
--rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 tmlt_analytics-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    13178 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/CHANGELOG.rst
+-rw-r--r--   0        0        0    11358 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/LICENSE
+-rw-r--r--   0        0        0    20138 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/LICENSE.docs
+-rw-r--r--   0        0        0      121 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/NOTICE
+-rw-r--r--   0        0        0     2597 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/README.md
+-rw-r--r--   0        0        0      951 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/css/custom.css
+-rw-r--r--   0        0        0    12470 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     1001 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/js/version-banner.js
+-rw-r--r--   0        0        0    30903 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_static/logo.png
+-rw-r--r--   0        0        0       50 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_templates/build-info.html
+-rw-r--r--   0        0        0      408 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_templates/layout.html
+-rw-r--r--   0        0        0       23 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/_templates/package-name.html
+-rw-r--r--   0        0        0     1108 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/citing.rst
+-rw-r--r--   0        0        0      201 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/index.rst
+-rw-r--r--   0        0        0      670 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/license.rst
+-rw-r--r--   0        0        0     3159 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/additional-resources/privacy_policy.rst
+-rw-r--r--   0        0        0     6764 2023-04-17 23:55:36.890097 tmlt_analytics-0.7.0rc1/doc/conf.py
+-rw-r--r--   0        0        0   118378 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/api_diagram.svg
+-rw-r--r--   0        0        0    85925 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_age_at_joining.png
+-rw-r--r--   0        0        0    27267 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_attacker_certainty.png
+-rw-r--r--   0        0        0    41645 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_average_age_by_edu.png
+-rw-r--r--   0        0        0    34101 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_books_by_unique_members.png
+-rw-r--r--   0        0        0   104926 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_age_gender.png
+-rw-r--r--   0        0        0    34006 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_different_eps.png
+-rw-r--r--   0        0        0    25097 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_edu+sex.png
+-rw-r--r--   0        0        0    13993 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_counts_education.png
+-rw-r--r--   0        0        0    41034 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_error_vs_partition_age_edu.png
+-rw-r--r--   0        0        0    59042 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_favorite_genres.png
+-rw-r--r--   0        0        0    14310 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_filters_education.png
+-rw-r--r--   0        0        0    30330 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_genres_by_age.png
+-rw-r--r--   0        0        0    14782 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_quantiles_education.png
+-rw-r--r--   0        0        0    20853 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_1.png
+-rw-r--r--   0        0        0    21067 2023-04-17 23:55:36.894096 tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_2.png
+-rw-r--r--   0        0        0    29335 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/chart_teen_edu_counts.png
+-rw-r--r--   0        0        0    20226 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/chart_younger_age_counts.png
+-rw-r--r--   0        0        0    29155 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_averages.png
+-rw-r--r--   0        0        0     9416 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_schema.png
+-rw-r--r--   0        0        0    23590 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/flow_chart_truncation.svg
+-rw-r--r--   0        0        0    14685 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/histogram_books_borrowed.png
+-rw-r--r--   0        0        0     1844 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_api.svg
+-rw-r--r--   0        0        0     1196 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_more.svg
+-rw-r--r--   0        0        0      604 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_topic_guides.svg
+-rw-r--r--   0        0        0     1371 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/index_tutorials.svg
+-rw-r--r--   0        0        0    30903 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/images/logo.png
+-rw-r--r--   0        0        0     3971 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/index.rst
+-rw-r--r--   0        0        0     4960 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/installation.rst
+-rw-r--r--   0        0        0      662 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/intersphinx_mapping.json
+-rw-r--r--   0        0        0     2024 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/templates/python/class.rst
+-rw-r--r--   0        0        0     3440 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/templates/python/module.rst
+-rw-r--r--   0        0        0     1602 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/bigquery-setup.rst
+-rw-r--r--   0        0        0     3022 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/docker-image.rst
+-rw-r--r--   0        0        0     1237 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/index.rst
+-rw-r--r--   0        0        0     6303 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/inputs-outputs.rst
+-rw-r--r--   0        0        0     5770 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/parameters.rst
+-rw-r--r--   0        0        0     4763 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/running-the-program.rst
+-rw-r--r--   0        0        0     1716 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/bigquery/setup.rst
+-rw-r--r--   0        0        0      405 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/index.rst
+-rw-r--r--   0        0        0    11697 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/nulls-nans-infinities.rst
+-rw-r--r--   0        0        0     8608 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-budgets.rst
+-rw-r--r--   0        0        0     6595 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-promise.rst
+-rw-r--r--   0        0        0     7726 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/spark.rst
+-rw-r--r--   0        0        0     2735 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/troubleshooting.rst
+-rw-r--r--   0        0        0     8462 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/topic-guides/working-with-sessions.rst
+-rw-r--r--   0        0        0     9124 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/clamping-bounds.rst
+-rw-r--r--   0        0        0     7246 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/first-steps.rst
+-rw-r--r--   0        0        0    18802 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/groupby-queries.rst
+-rw-r--r--   0        0        0      430 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/index.rst
+-rw-r--r--   0        0        0    11634 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/more-with-privacy-ids.rst
+-rw-r--r--   0        0        0     7732 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-budget-basics.rst
+-rw-r--r--   0        0        0    11302 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-id-basics.rst
+-rw-r--r--   0        0        0    16226 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/doc/tutorials/simple-transformations.rst
+-rw-r--r--   0        0        0     4789 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/examples/interactive_evaluation.ipynb
+-rw-r--r--   0        0        0     5459 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/examples/private_join.ipynb
+-rw-r--r--   0        0        0     6570 2023-04-17 23:55:36.898096 tmlt_analytics-0.7.0rc1/examples/zcdp_puredp_switching.ipynb
+-rw-r--r--   0        0        0     4469 2023-04-17 23:55:55.706036 tmlt_analytics-0.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/__init__.py
+-rw-r--r--   0        0        0     6976 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/conftest.py
+-rw-r--r--   0        0        0      115 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/__init__.py
+-rw-r--r--   0        0        0     4265 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/conftest.py
+-rw-r--r--   0        0        0      151 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/__init__.py
+-rw-r--r--   0        0        0    15227 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_constraint_propagation.py
+-rw-r--r--   0        0        0    21707 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_l0_linf_truncation.py
+-rw-r--r--   0        0        0    14517 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_l1_truncation.py
+-rw-r--r--   0        0        0     4011 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/ids/test_partition.py
+-rw-r--r--   0        0        0      143 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/mixed/__init__.py
+-rw-r--r--   0        0        0     5087 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/mixed/test_mixed_session.py
+-rw-r--r--   0        0        0      152 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/__init__.py
+-rw-r--r--   0        0        0    25557 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/conftest.py
+-rw-r--r--   0        0        0    38557 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows.py
+-rw-r--r--   0        0        0     6134 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows_in_max_groups.py
+-rw-r--r--   0        0        0    13790 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_add_max_rows_infs_nulls.py
+-rw-r--r--   0        0        0     7754 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/rows/test_invalid.py
+-rw-r--r--   0        0        0     2212 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/system/session/test_invalid_constraints.py
+-rw-r--r--   0        0        0      108 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/__init__.py
+-rw-r--r--   0        0        0      298 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    75163 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_measurement_visitor.py
+-rw-r--r--   0        0        0    54429 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_output_schema_visitor.py
+-rw-r--r--   0        0        0      107 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/__init__.py
+-rw-r--r--   0        0        0    17843 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/conftest.py
+-rw-r--r--   0        0        0    24159 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
+-rw-r--r--   0        0        0    36757 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
+-rw-r--r--   0        0        0     7610 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
+-rw-r--r--   0        0        0    14086 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_binning_spec.py
+-rw-r--r--   0        0        0     2301 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_catalog.py
+-rw-r--r--   0        0        0      657 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_cleanup.py
+-rw-r--r--   0        0        0     5285 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_constraints.py
+-rw-r--r--   0        0        0    21191 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_keyset.py
+-rw-r--r--   0        0        0    13993 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_neighboring_relations.py
+-rw-r--r--   0        0        0     3058 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_noise_info.py
+-rw-r--r--   0        0        0     5865 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget.py
+-rw-r--r--   0        0        0     5420 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0     3011 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_protected_change.py
+-rw-r--r--   0        0        0    40864 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_builder.py
+-rw-r--r--   0        0        0    63485 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_expr_compiler.py
+-rw-r--r--   0        0        0    16715 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_expression.py
+-rw-r--r--   0        0        0     4904 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_query_expression_visitor.py
+-rw-r--r--   0        0        0     2172 2023-04-17 23:55:36.902096 tmlt_analytics-0.7.0rc1/test/unit/test_schema.py
+-rw-r--r--   0        0        0    13538 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_schema_conversion.py
+-rw-r--r--   0        0        0    84468 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_session.py
+-rw-r--r--   0        0        0     1604 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_table_identifiers.py
+-rw-r--r--   0        0        0     5371 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_transformation_utils.py
+-rw-r--r--   0        0        0      792 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_truncation_strategy.py
+-rw-r--r--   0        0        0      518 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test/unit/test_utils.py
+-rw-r--r--   0        0        0       37 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/test_requirements.txt
+-rw-r--r--   0        0        0      222 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/__init__.py
+-rw-r--r--   0        0        0     3666 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_catalog.py
+-rw-r--r--   0        0        0     3555 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_coerce_spark_schema.py
+-rw-r--r--   0        0        0    16188 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation.py
+-rw-r--r--   0        0        0     6110 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation_visitor.py
+-rw-r--r--   0        0        0     5428 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_noise_info.py
+-rw-r--r--   0        0        0     2289 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0      184 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0     9786 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_compiler.py
+-rw-r--r--   0        0        0     7694 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
+-rw-r--r--   0        0        0    34784 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
+-rw-r--r--   0        0        0    46272 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
+-rw-r--r--   0        0        0    59768 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
+-rw-r--r--   0        0        0    12656 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_schema.py
+-rw-r--r--   0        0        0     1250 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_table_identifier.py
+-rw-r--r--   0        0        0     3979 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_table_reference.py
+-rw-r--r--   0        0        0    10147 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/_transformation_utils.py
+-rw-r--r--   0        0        0    11663 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/binning_spec.py
+-rw-r--r--   0        0        0      306 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/cleanup.py
+-rw-r--r--   0        0        0      288 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_base.py
+-rw-r--r--   0        0        0      735 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_simplify.py
+-rw-r--r--   0        0        0    12819 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/constraints/_truncation.py
+-rw-r--r--   0        0        0    11850 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/keyset.py
+-rw-r--r--   0        0        0     7155 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/privacy_budget.py
+-rw-r--r--   0        0        0     5471 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/protected_change.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/py.typed
+-rw-r--r--   0        0        0   126388 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/query_builder.py
+-rw-r--r--   0        0        0    41097 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/query_expr.py
+-rw-r--r--   0        0        0    72500 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/session.py
+-rw-r--r--   0        0        0     3031 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/truncation_strategy.py
+-rw-r--r--   0        0        0     4772 2023-04-17 23:55:36.906096 tmlt_analytics-0.7.0rc1/tmlt/analytics/utils.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.0rc1/setup.py
+-rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.0rc1/PKG-INFO
```

### Comparing `tmlt_analytics-0.6.1/CHANGELOG.rst` & `tmlt_analytics-0.7.0rc1/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,42 @@
 .. _analytics-changelog:
 
 Changelog
 =========
 
+Unreleased
+----------
+
+Added
+~~~~~
+- Added MaxRowsPerGroupPerID contraint, which limits the number of rows each unique (ID, grouping column value) pair may appear in.
+- Added MaxGroupsPerID constraint, which limits the number of unique grouping column values associated with each unique ID.
+- Added a new :class:`tmlt.analytics.protected_change.AddRowsWithID` class, which protects the addition or removal of all rows with the same value in a specified column.
+  When creating a session with AddRowsWithID for multiple tables, you must use the new :meth:`Session.Builder.with_id_space <tmlt.analytics.session.Session.Builder.with_id_space>` method to specify the identifier space(s) of the tables.
+  See the documentation for :class:`tmlt.analytics.protected_change.AddRowsWithID` for more information.
+- Added a new method, :meth:`tmlt.analytics.session.Session.describe`, which describes a session, query, or table.
+
+
+Changed
+~~~~~~~
+- Argument ``max_num_rows`` of ``QueryBuilder.flat_map`` is now optional for tables with a :class:`tmlt.analytics.protected_change.AddRowsWithID` protected change.
+- *Backwards-incompatible*: Argument ``max_num_rows`` is now the last parameter specified for ``QueryBuilder.flat_map``.
+- *Backwards-incompatible*: Analytics no longer allows users to set lower bounds equal to upper bounds for quantile, sum, average, variance, and standard deviation queries. Now, the lower bound must be strictly less than the upper bound.
+- *Backwards-incompatible*: Renamed ``QueryBuilder.filter`` argument from "predicate" to "condition".
+- *Backwards-incompatible*: Renamed ``query_expr.Filter`` property from "predicate" to "condition".
+- *Backwards-incompatible*: Renamed ``KeySet.filter`` argument from "expr" to "condition".
+- ``QueryBuilder.join_private`` now accepts a string as a ``right_operand``. ``QueryBuilder("table").join_private("foo")`` is equivalent to ``QueryBuilder("table").join_private(QueryBuilder("foo"))``.
+- *Backwards-incompatible*: Removed the ``attr_name`` argument from ``Session.partition_and_create``.
+
+Fixed
+~~~~~
+
+- ``Session.add_public_datafame`` used to allow creation of a public table with the same name as an existing private table, even though doing so is disallowed elsewhere and is not fully supported by some ``Session`` methods.
+  It now raises a ``ValueError`` when this happens, like it already did when there was a name conflict with an existing public table.
+
 0.6.1 - 2022-12-07
 ------------------
 
 This is a maintenance release which introduces a number of documentation improvements, but has no publicly-visible API changes.
 
 0.6.0 - 2022-12-06
 ------------------
```

### Comparing `tmlt_analytics-0.6.1/LICENSE` & `tmlt_analytics-0.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/LICENSE.docs` & `tmlt_analytics-0.7.0rc1/LICENSE.docs`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/README.md` & `tmlt_analytics-0.7.0rc1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 automatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).
 
 ## Installation
 
 See the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)
 for information about setting up prerequisites such as Spark.
 
-Once the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project.pip).
+Once the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project/pip).
 
 ```bash
 pip install tmlt.analytics
 ```
 
 ## Documentation
 
@@ -25,14 +25,39 @@
 
 ## Contributing
 
 We are not yet accepting external contributions, but please let us know if you are interested in contributing [via Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.
 
+## Citing Tumult Analytics
+
+If you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.
+
+```
+@software{tumultanalyticssoftware,
+    author = {Tumult Labs},
+    title = {Tumult {{Analytics}}},
+    month = dec,
+    year = 2022,
+    version = {latest},
+    url = {https://tmlt.dev}
+}
+```
+
+```
+@article{tumultanalyticswhitepaper,
+  title={Tumult {{Analytics}}: a robust, easy-to-use, scalable, and expressive framework for differential privacy},
+  author={Berghel, Skye and Bohannon, Philip and Desfontaines, Damien and Estes, Charles and Haney, Sam and Hartman, Luke and Hay, Michael and Machanavajjhala, Ashwin and Magerlein, Tom and Miklau, Gerome and Pai, Amritha and Sexton, William and Shrestha, Ruchit},
+  journal={arXiv preprint arXiv:2212.04133},
+  month = dec,
+  year={2022}
+}
+```
+
 ## License
 
-Copyright Tumult Labs 2022
+Copyright Tumult Labs 2023
 
 The Tumult Platform source code is licensed under the Apache License, version 2.0 (Apache-2.0).
 The Tumult Platform documentation is licensed under
 Creative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).
```

### Comparing `tmlt_analytics-0.6.1/doc/_static/css/custom.css` & `tmlt_analytics-0.7.0rc1/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/_static/favicon.ico` & `tmlt_analytics-0.7.0rc1/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/_static/js/version-banner.js` & `tmlt_analytics-0.7.0rc1/doc/_static/js/version-banner.js`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/_static/logo.png` & `tmlt_analytics-0.7.0rc1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/additional-resources/license.rst` & `tmlt_analytics-0.7.0rc1/doc/additional-resources/license.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _License:
 
 License
 =======
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
-Copyright Tumult Labs 2022
+Copyright Tumult Labs 2023
 
 The Tumult Analytics source code is licensed under the Apache License, version 2.0 (`Apache-2.0 <https://gitlab.com/tumult-labs/core/-/blob/dev/LICENSE>`_).
 
 The Tumult Analytics documentation is licensed under Creative Commons Attribution-ShareAlike 4.0 International (`CC-BY-SA-4.0 <https://gitlab.com/tumult-labs/core/-/blob/dev/LICENSE.docs>`_).
 To view a copy of this license, visit this `webpage <http://creativecommons.org/licenses/by-sa/4.0/>`_ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
```

### Comparing `tmlt_analytics-0.6.1/doc/additional-resources/privacy_policy.rst` & `tmlt_analytics-0.7.0rc1/doc/additional-resources/privacy_policy.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/conf.py` & `tmlt_analytics-0.7.0rc1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pylint: skip-file
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 import logging
 import os
 import sys
 import datetime
 
 _logger = logging.getLogger(__name__)
 
 # Project information
 
 project = "Tumult Analytics"
 author = "Tumult Labs"
-copyright = "Tumult Labs 2022"
+copyright = "Tumult Labs 2023"
 
 package_name = "tmlt.analytics"
 
 # TODO(#1256): Fix import failure in nested class; `tmlt.core` and remove suppress_warnings setting
 suppress_warnings = ["autoapi.python_import_resolution", "autodoc.import_object"]
```

### Comparing `tmlt_analytics-0.6.1/doc/images/api_diagram.svg` & `tmlt_analytics-0.7.0rc1/doc/images/api_diagram.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_age_at_joining.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_age_at_joining.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_attacker_certainty.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_attacker_certainty.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_average_age_by_edu.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_average_age_by_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_counts_age_gender.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_age_gender.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_counts_different_eps.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_different_eps.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_counts_edu+sex.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_edu+sex.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_counts_education.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_counts_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_error_vs_partition_age_edu.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_error_vs_partition_age_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_filters_education.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_filters_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_quantiles_education.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_quantiles_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_senior_counts_1.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_1.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_senior_counts_2.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_senior_counts_2.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_teen_edu_counts.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_teen_edu_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/chart_younger_age_counts.png` & `tmlt_analytics-0.7.0rc1/doc/images/chart_younger_age_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/clamping_bounds_averages.png` & `tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_averages.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/clamping_bounds_schema.png` & `tmlt_analytics-0.7.0rc1/doc/images/clamping_bounds_schema.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/histogram_books_borrowed.png` & `tmlt_analytics-0.7.0rc1/doc/images/histogram_books_borrowed.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/index_api.svg` & `tmlt_analytics-0.7.0rc1/doc/images/index_api.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/index_more.svg` & `tmlt_analytics-0.7.0rc1/doc/images/index_more.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/index_topic_guides.svg` & `tmlt_analytics-0.7.0rc1/doc/images/index_topic_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/index_tutorials.svg` & `tmlt_analytics-0.7.0rc1/doc/images/index_tutorials.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/images/logo.png` & `tmlt_analytics-0.7.0rc1/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/index.rst` & `tmlt_analytics-0.7.0rc1/doc/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -84,16 +84,18 @@
    ---
    :img-top: images/index_more.svg
 
 
    **Additional resources**
    ^^^^^^^^^^^^^^^^^^^^^^^^
 
-   Additional resources include the :ref:`changelog <analytics-changelog>`, which
-   describes notable changes to the library, as well as
+   Additional resources include the :ref:`changelog <analytics-changelog>`,
+   our :ref:`troubleshooting guide <troubleshooting>`,
+   :ref:`citation instructions <citing>`
+   if you use Tumult Analytics for a scientific publication, and 
    :ref:`license information <License>`.
 
 Contact Information
 ^^^^^^^^^^^^^^^^^^^
 The best place to ask questions, file feature requests, or give feedback about Tumult Analytics
 is our `Slack server <https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#>`__.
 We also use it for announcements of new releases and feature additions.
```

### Comparing `tmlt_analytics-0.6.1/doc/installation.rst` & `tmlt_analytics-0.7.0rc1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/intersphinx_mapping.json` & `tmlt_analytics-0.7.0rc1/doc/intersphinx_mapping.json`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/templates/python/class.rst` & `tmlt_analytics-0.7.0rc1/doc/templates/python/class.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
       {% endfor %}
 
    {% endif %}
    {% if visible_attributes %}
    .. list-table:: Attributes
 
       {% for attribute in visible_attributes %}
-      * - :attribute:`.{{ attribute.short_name }}`
+      * - :attr:`.{{ attribute.short_name }}`
         - {{ attribute.summary }}
       {% endfor %}
 
    {% endif %}
    {% if visible_methods %}
    .. list-table:: Methods
```

### Comparing `tmlt_analytics-0.6.1/doc/templates/python/module.rst` & `tmlt_analytics-0.7.0rc1/doc/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/doc/topic-guides/nulls-nans-infinities.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/nulls-nans-infinities.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Nulls, NaNs, and infinite values:
 
 Nulls, NaNs, and infinite values
 ================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 This topic guide details how 
 `null values <https://en.wikipedia.org/wiki/Null_(SQL)>`__,
 `NaN values <https://en.wikipedia.org/wiki/NaN>`__, and 
 `infinite values <https://en.wikipedia.org/wiki/IEEE_754-1985#Positive_and_negative_infinity>`__
 (positive and negative infinity) are handled in Tumult Analytics.
```

### Comparing `tmlt_analytics-0.6.1/doc/topic-guides/privacy-budgets.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-budgets.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 Privacy budget fundamentals
 ===========================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 This topic guide goes into more depth on the concept of *privacy budgets* that
 we discussed in :ref:`tutorial two <Working with privacy budgets>`. At a high
 level, a privacy budget associates one or more numeric *privacy parameters* with
 a *privacy definition*. Together, this information determines the privacy
 guarantees provided by each query, and by the Session as a whole.
```

### Comparing `tmlt_analytics-0.6.1/doc/topic-guides/privacy-promise.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/privacy-promise.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,106 @@
 .. _Privacy promise:
 
 Tumult Analytics' privacy promise
 =================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 This topic guide outlines the "privacy promise" provided by Tumult Analytics,
 along with its caveats. This guarantee is based on one of the core abstractions
-of Tumult Analytics: :class:`Sessions<tmlt.analytics.session.Session>`.
+of Tumult Analytics: :class:`Sessions <tmlt.analytics.session.Session>`.
 
 At a high level, a Session allows you to evaluate queries on private data in a
 way that satisfies differential privacy. When creating a Session, private data
-must first be loaded into it, along with a
-:ref:`privacy budget<Privacy budget fundamentals>`. You can then evaluate
+must first be loaded into it, along with
+a :mod:`protected change<tmlt.analytics.protected_change>` for each
+table, and a Session-wide :ref:`privacy budget<Privacy budget fundamentals>`. You
+can then evaluate
 queries on your private data, consuming at most the privacy budget provided at
 initialization time.
 
 The privacy promise in more detail
 ----------------------------------
 
 A :class:`~tmlt.analytics.session.Session` is initialized with:
 
-* one or more private data sources (data you wish to query in a differentially
-  private way);
-* one or more public data sources (data that does not require privacy
+* one or more private tables (containing data you wish to query in a differentially
+  private way), each associated to a :mod:`protected change<tmlt.analytics.protected_change>`;
+* zero or more public tables (containing data that does not require privacy
   protection, but may be used as auxiliary input to your computation);
 * a privacy definition along with its associated privacy parameters (e.g.
   tutorials use `PureDBBudget`, corresponding to pure differential privacy, and
   Tumult Analytics also supports zero-concentrated differential privacy).
 
 After initialization, the Session guarantees that the answers returned by
 calling :meth:`~tmlt.analytics.session.Session.evaluate` to evaluate queries
 satisfy the corresponding privacy definition with respect to the private data,
 using the specified parameters. For example, a Session initialized with
 :code:`PureDPBudget(1)` provides :math:`{\varepsilon}`-differential privacy with
 :math:`{\varepsilon}=1`.
 
 .. _privacy-promise#unit-of-protection:
 
-Subtlety 1: unit of protection
-------------------------------
+Understanding the protected change
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-In the simplest case, the privacy guarantee from a :class:`~tmlt.analytics.session.Session` prevents an attacker from learning whether *one individual row* was added or removed in each private dataset -- the :class:`~tmlt.analytics.protected_change.AddOneRow` protected change.
-If the data of a single individual can span multiple rows in the same private dataset, then this individual is not covered by the privacy promise, only individual rows are.
+Each table's differential privacy guarantee hides a *protected change* in
+data, preventing an attacker from learning whether a table was changed 
+in some specified way. When you add a private table to a session, you must
+specify what kind of protected change to use for this table.
+
+* In the simplest case, the privacy guarantee from a
+  :class:`~tmlt.analytics.session.Session` prevents an attacker from learning 
+  whether *one individual row* was added or removed in each private table -- the 
+  :class:`~tmlt.analytics.protected_change.AddOneRow` protected change.
+  If the data of a single individual can span multiple rows in the same private
+  table, then this individual is not covered by the privacy promise, only
+  individual rows are.
+
+* If you know that a single individual can appear in at most *k* rows in a private 
+  table, you can load that table into a Session using a different value for the
+  ``protected_change`` parameter.
+  For example, using ``AddMaxRows(k)`` will cause Tumult Analytics to hide the
+  addition or removal of up to *k* rows at once from the corresponding private table.
+
+* If you want to protect the addition or removal of *arbitrarily many* rows that
+  all share the same *identifier* (in some column), you can use the 
+  :class:`~tmlt.analytics.protected_change.AddRowsWithID` protected change.
+  If you add multiple tables that all use ``AddRowsWithID``, the
+  :attr:`~tmlt.analytics.protected_change.AddRowsWithID.id_space` property
+  determines which ID space each table belongs to.
+
+Other possible protected changes are also available, though they are typically
+only needed for advanced use cases.
+See our :mod:`~tmlt.analytics.protected_change` documentation for more information.
+
+Because the privacy of individuals depends on how often they appear in a table,
+you should be careful of what kind of pre-processing is done to the private data
+before loading it into a Session.
+For example, if you start from a table where each individual appears in a single
+record, but this property stops being true before the data is loaded into a Session,
+then using ``AddOneRow`` as a protected change might not reflect the privacy guarantee that you want to achieve.
 
-If you know that a single individual can appear in at most *k* rows in an input dataset, you can load that dataset into a Session using a different value for the ``protected_change`` parameter.
-For example, using ``AddMaxRows(k)`` will cause Tumult Analytics to hide the addition or removal of up to *k* rows at once from the corresponding private dataset, providing individual-level protection.
-Other possible protected changes are also available, though they are typically only needed for advanced use cases.
-
-Because the privacy of individuals depends on how often they appear in a dataset, you should be careful of what kind of pre-processing is done to the private data before loading it into a Session.
-If you start from a DataFrame where each individual appears in a single record, but this property stops being true before the data is loaded into a Session, then you might not get the expected privacy guarantees.
-
-Subtlety 2: covered inputs & outputs
+Subtlety 1: covered inputs & outputs
 ------------------------------------
 
-A Session only provides guarantees on the private datasets, and this guarantee
+A Session only provides guarantees on the private tables, and this guarantee
 only covers data returned by ``evaluate`` calls. Use of the private data in any
 other way is not protected by the Session.
 
 This means that **you should not directly use private data**; instead, you
 should only access it indirectly by executing
 :meth:`~tmlt.analytics.session.Session.evaluate` on well-specified queries. In
 particular, public sources and parameters like ``groupby`` information or
 clamping bounds are not protected. They can reveal private information if the
 private data is used directly to determine them.
 
-Subtlety 3: adversarial model
+Subtlety 2: adversarial model
 -----------------------------
 
 Tumult Analytics, and in particular the Session interface, is designed to make
 it easy to obtain expected differential privacy guarantees, and difficult to
 accidentally break these guarantees. However, this library was *not* designed to
 defend against actively malicious users. In particular:
```

### Comparing `tmlt_analytics-0.6.1/doc/topic-guides/spark.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/spark.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Spark:
 
 Spark
 =====
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 Tumult Analytics uses Spark as its underlying data processing
 framework. This topic guide covers relevant information about Spark
 for users of the Analytics library.
 
 Configuring Spark sessions
 --------------------------
@@ -151,7 +151,49 @@
 
 Performance and profiling
 -------------------------
 
 All queries made with Analytics are executed by Spark. If you are having
 performance problems, you will probably want to look at
 `Spark performance-tuning options <https://spark.apache.org/docs/latest/sql-performance-tuning.html>`_.
+
+RAM usage
+^^^^^^^^^
+
+By default, Spark allocates itself 1GB of RAM 
+(see `Spark's configuration documentation <https://spark.apache.org/docs/latest/configuration.html#application-properties>`_).
+Analytics programs often need more RAM than this.
+Usually, a program needs more RAM because:
+
+* the input data is large (10M rows or more)
+* a keyset used for a grouping operation is large (10k rows or more)
+* the output data is large (10M rows or more)
+
+You can adjust the amount of memory available to Spark when creating your
+Spark session. For example, to configure Spark with 8 gigabytes of RAM, you
+can run this code:
+
+.. code-block::
+
+    spark = SparkSession.builder.config('spark.driver.memory', '8gb').getOrCreate()
+
+This only applies when running Spark on a single, local node; see Spark's
+documentation for how to configure Spark to use more RAM across a cluster.
+
+Saving results (to CSV or other formats)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Converting large Spark dataframes (10M rows or more) to Pandas dataframes can
+be very resource-intensive. We recommend using 
+:meth:`pyspark.sql.DataFrame.write` to save results
+to file, instead of using 
+:meth:`pyspark.sql.DataFrame.toPandas` and then saving the Pandas
+dataframe.
+
+For example, to save a dataframe as CSV, you can do this:
+
+.. code-block::
+
+    import os
+    import tempfile
+
+    df.write.csv(os.path.join(tempfile.mkdtemp(), 'data'))
```

### Comparing `tmlt_analytics-0.6.1/doc/topic-guides/working-with-sessions.rst` & `tmlt_analytics-0.7.0rc1/doc/topic-guides/working-with-sessions.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Working with Sessions:
 
 Working with Sessions
 =====================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 This topic guide covers how to work with one of the core abstractions of Tumult
 Analytics: :class:`Session <tmlt.analytics.session.Session>`. In particular, we
 will demonstrate the different ways that a Session can be initialized and
 examined. For a simple end-to-end usage example of a Session, a better place to
 start is the :ref:`privacy budget tutorial <Working with privacy budgets>`.
 
@@ -198,15 +198,15 @@
 .. testcode::
 
     print(session.private_sources)
     print(session.public_sources)
 
 .. testoutput::
 
-    ['my_private_data', 'my_other_private_data']
+    ['my_other_private_data', 'my_private_data']
     ['my_public_data']
 
 These IDs will typically be used when constructing queries, to specify which data
 source a query refers to. They can also be used to access schema information about
 individual data sources, through
 :meth:`~tmlt.analytics.session.Session.get_schema`.
```

### Comparing `tmlt_analytics-0.6.1/doc/tutorials/clamping-bounds.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/clamping-bounds.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Clamping bounds:
 
 Tutorial 3: Introduction to clamping bounds
 ===========================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 Counting queries, which we saw in tutorials :ref:`one <First steps>` and
 :ref:`two <Working with privacy budgets>`, are very useful, but we often need a
 little more: sums, averages, medians… In this tutorial, we'll see how to compute
 this larger class of aggregations with Tumult Analytics. These operations
 require us to learn and use a new concept: *clamping bounds*. In this tutorial,
 we'll tell you what these are, how they work, and how to specify them in
```

### Comparing `tmlt_analytics-0.6.1/doc/tutorials/first-steps.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/first-steps.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _First steps:
 
 Tutorial 1: First steps with Tumult Analytics
 =============================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 In this first tutorial, we will demonstrate how to load data, run a simple
 aggregation query, and get our first differentially private results. You can run
 this tutorial (as well as the next ones) as you go: simply follow the
 :ref:`installation instructions <Installation instructions>`, and use the copy/paste button of each code
 block to reproduce it.
```

### Comparing `tmlt_analytics-0.6.1/doc/tutorials/groupby-queries.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/groupby-queries.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Group-by queries:
 
 Tutorial 4: Group-by queries
 ============================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 In all previous tutorials, all aggregations we saw were global aggregations,
 returning a single statistic for all the data. But many common data analysis
 operations are *group-by queries*: they partition the data into groups, and
 compute one aggregation per group. In this tutorial, we will demonstrate how to
 express such queries using Tumult Analytics.
```

### Comparing `tmlt_analytics-0.6.1/doc/tutorials/privacy-budget-basics.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/privacy-budget-basics.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Working with privacy budgets:
 
 Tutorial 2: Working with privacy budgets
 ========================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 
 In our :ref:`first tutorial<First steps>`, we saw how to run a simple aggregation
 query on private data. When loading the private data into a Session, we had to
 specify a *privacy budget*. This raises two kinds of questions.
 
 1. What is a privacy budget, what formal guarantee does it provide, and how can
```

### Comparing `tmlt_analytics-0.6.1/doc/tutorials/simple-transformations.rst` & `tmlt_analytics-0.7.0rc1/doc/tutorials/simple-transformations.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _Simple transformations:
 
 Tutorial 5: Simple transformations
 ==================================
 
 ..
     SPDX-License-Identifier: CC-BY-SA-4.0
-    Copyright Tumult Labs 2022
+    Copyright Tumult Labs 2023
 
 So far we have learned how to perform aggregations on our data, but sometimes we need
 to transform our data before they are ready to be aggregated. In this tutorial, we'll
 demonstrate a few ways that we can transform our data using filters, maps, flat maps,
 binning, and public joins.
 
 Setup
@@ -131,27 +131,33 @@
         "favorite_genres": "Romance;Classics/Literature;Current affairs",
         "date_joined": "2021-12-22",
     }
 
     print(age_joined(example_row))
 
 .. testoutput::
+   :hide:
+   :options: +NORMALIZE_WHITESPACE
 
-    {'age_joined': 50}
+    {'age_joined': ...}
+
+.. code-block::
+
+    {'age_joined': 49}
 
 Now that we have our mapping function, we can use it in a query.
 
-To add the map to our query, we also need to provide the `new_column_types`. It should
+To add the map to our query, we also need to provide the ``new_column_types``. It should
 be a dictionary containing the names and types for each of the columns created by the
-map. In this case, the type is `INTEGER`.
+map. In this case, the type is ``INTEGER``.
 
-We also set `augment=True`. This tells the query to keep the original columns in
-addition to the columns created by the map. If we used `augment=False`, the `gender`
+We also set ``augment=True``. This tells the query to keep the original columns in
+addition to the columns created by the map. If we used ``augment=False``, the ``gender``
 column would no longer be available: the only column in the transformed data would be
-`age_joined`.
+``age_joined``.
 
 .. testcode::
 
     from tmlt.analytics.query_builder import ColumnType
 
     ages = list(range(0, 100))  # [0, 6, ..., 99]
     age_keys = KeySet.from_dict({"age_joined": ages})
@@ -222,24 +228,24 @@
     }
     print(expand_genre(example_row))
 
 .. testoutput::
 
     [{'genre': 'Romance'}, {'genre': 'Classics/Literature'}, {'genre': 'Current affairs'}]
 
-Like `map`, `flat_map` has the `new_column_types` and `augment` options. In this
-example, we leave `augment` with its default value of `False`.
+Like ``map``, ``flat_map`` has the ``new_column_types`` and ``augment`` options.
+In this example, we leave ``augment`` with its default value of ``False``.
 
-Unlike `map`, `flat_map` has an argument `max_num_rows`. It clamps the maximum number
+Unlike ``map``, ``flat_map`` has an argument ``max_num_rows``. It clamps the maximum number
 of new rows that can be created for each input row. This serves a similar function as
 the clamping bounds on aggregations we used in :ref:`tutorial 3 <Clamping bounds>`, and
-also has the analogous trade-offs: higher values for `max_num_rows` will result in more
+also has the analogous trade-offs: higher values for ``max_num_rows`` will result in more
 noise in the final results, while lower values may cause more rows to be silently
 dropped. In this case, the choice is easy: no members have more than three favorites and
-there are many members with three, so we set `max_num_rows=3`.
+there are many members with three, so we set ``max_num_rows=3``.
 
 .. testcode::
 
     genre_keys = KeySet.from_dict(
         {
             "genre": [
                 "Mystery/thriller/crime",
@@ -263,16 +269,16 @@
             ],
         }
     )
     genre_count_query = (
         QueryBuilder("members")
         .flat_map(
             expand_genre,
-            max_num_rows=3,
             new_column_types={"genre": ColumnType.VARCHAR},
+            max_num_rows=3,
         )
         .groupby(genre_keys)
         .count()
     )
     genre_counts = session.evaluate(
         genre_count_query,
         privacy_budget=PureDPBudget(epsilon=1),
```

### Comparing `tmlt_analytics-0.6.1/examples/interactive_evaluation.ipynb` & `tmlt_analytics-0.7.0rc1/examples/interactive_evaluation.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998299319727891%*

 * *Differences: {"'cells'": '{14: {\'source\': {insert: [(3, \'    column="Y", \\n\')], delete: [3]}}}'}*

```diff
@@ -139,15 +139,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "new_sessions = sess.partition_and_create(\n",
                 "    \"joined_data\", \n",
                 "    privacy_budget=PureDPBudget(3),\n",
-                "    attr_name=\"Y\", \n",
+                "    column=\"Y\", \n",
                 "    splits={\"partition_0\": 0, \"partition_1\": 1}\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `tmlt_analytics-0.6.1/examples/private_join.ipynb` & `tmlt_analytics-0.7.0rc1/examples/private_join.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/examples/zcdp_puredp_switching.ipynb` & `tmlt_analytics-0.7.0rc1/examples/zcdp_puredp_switching.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/pyproject.toml` & `tmlt_analytics-0.7.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 readme = "README.md"
 authors = []
 license = "Apache-2.0"
 homepage = "https://www.tmlt.dev/"
 repository = "https://gitlab.com/tumult-labs/analytics"
 documentation = "https://docs.tmlt.dev/analytics/latest"
 # The version field is required in this file format, even though it's ignored because of poetry-dynamic-versioning.
-version = "0.6.1"
+version = "0.7.0-rc.1"
 
 classifiers = [
    "Development Status :: 4 - Beta",
    "Intended Audience :: Developers",
    "Intended Audience :: Education",
    "Intended Audience :: Science/Research",
    "Natural Language :: English",
@@ -31,28 +31,29 @@
   { path = "NOTICE", format = "sdist" },
 ]
 packages = [
   { include = "tmlt" },
 ]
 
 
-### Note If Updating Dependencies ### 
-# Also make sure to update the dependency matrix
-# located in noxfile.py:test_multi_deps(), if needed. 
 [tool.poetry.dependencies]
 python = "^3.7.1, <3.10.0"
 
-"tmlt.core" = "^0.6.0"
+# When updating Core, PySpark, Pandas or SymPy, remember to update
+# test_multi_deps in the Noxfile.
+
+"tmlt.core" = "^0.9.0"
 
 pandas = "^1.2.0"
 pyspark = { version = "^3.0.0,<3.4.0", extras = ["sql"] }
 sympy = "^1.8,<1.10"
 typeguard = "^2.12.1,<2.13.0"
 typing-extensions = "^3.10.0"
 
+
 [tool.poetry.dev-dependencies]
 # Build scripting
 nox = "2022.8.7"
 nox_poetry = "1.0.1"
 
 # Linters, formatters
 black = "21.9b0"
@@ -80,14 +81,15 @@
 # Needed for code snippets in tutorials
 seaborn = "^0.11.1"
 
 # click 8.1.0 removes _unicodefun which breaks the CI; remove this after
 # upgrading Black.
 click = "8.0.4"
 
+
 [build-system]
 build-backend = "poetry_dynamic_versioning.backend"
 requires = ["poetry-core>=1.3.2", "poetry-dynamic-versioning"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
@@ -103,15 +105,18 @@
 
 [tool.mypy]
 explicit_package_bases = true
 follow_imports = "silent"
 ignore_missing_imports = true
 namespace_packages = true
 
-
+check_untyped_defs = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+warn_unreachable = true
 
 [tool.pylint.master]
 # See https://github.com/PyCQA/pylint/issues/1975#issuecomment-387924981
 extension-pkg-whitelist = ['numpy']
 load-plugins = ['pylint.extensions.docparams']
 # Only check param docs in docstrings that contain an Args: section.
 # Set to "no" to show docstrings missing argument documentation.
```

### Comparing `tmlt_analytics-0.6.1/test/conftest.py` & `tmlt_analytics-0.7.0rc1/test/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Creates a Spark Context to use for each testing session."""
 
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # TODO(#2206): Import these fixtures from core once it is rewritten
 # pylint: disable=unused-import
 import logging
 from typing import Any, Sequence
 from unittest.mock import Mock, create_autospec
 
 import numpy as np
```

### Comparing `tmlt_analytics-0.6.1/test/unit/query_expr_compiler/test_measurement_visitor.py` & `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_measurement_visitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# type: ignore[attr-defined]
 """Tests for MeasurementVisitor."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
-# pylint: disable=protected-access, pointless-string-statement, no-member, no-self-use
+# Copyright Tumult Labs 2023
 
+# pylint: disable=protected-access, no-member, no-self-use
 
-from typing import Dict, List, Optional, Tuple, Union
+from typing import List, Optional, Union
 from unittest.mock import patch
 
 import pandas as pd
 import pytest
 import sympy as sp
 from pyspark.sql import DataFrame
 from pyspark.sql.types import LongType, StringType, StructField, StructType
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler._measurement_visitor import (
     MeasurementVisitor,
     _get_query_bounds,
 )
 from tmlt.analytics._schema import ColumnDescriptor, ColumnType, Schema
+from tmlt.analytics._table_identifier import NamedTable
+from tmlt.analytics._table_reference import lookup_domain, lookup_metric
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountDistinctMechanism,
     CountMechanism,
 )
 from tmlt.analytics.query_expr import DropInfinity as DropInfExpr
@@ -70,20 +71,15 @@
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.transformations.chaining import ChainTT
-from tmlt.core.transformations.dictionary import GetValue
 from tmlt.core.transformations.spark_transformations.groupby import GroupBy
-from tmlt.core.transformations.spark_transformations.nan import DropNaNs, DropNulls
-from tmlt.core.transformations.spark_transformations.nan import (
-    ReplaceInfs as ReplaceInfTransformation,
-)
 from tmlt.core.transformations.spark_transformations.select import (
     Select as SelectTransformation,
 )
 from tmlt.core.utils.exact_number import ExactNumber
 from tmlt.core.utils.type_utils import assert_never
 
 from ...conftest import (  # pylint: disable=no-name-in-module
@@ -102,101 +98,15 @@
     if not isinstance(t.transformation2, ChainTT):
         right = [t.transformation2]
     else:
         right = chain_to_list(t.transformation2)
     return left + right
 
 
-"""Tests just for _get_query_bounds."""
-
-
-@pytest.mark.parametrize("bound", [(0), (-123456), (7899000)])
-def test_equal_upper_and_lower_average(bound: float) -> None:
-    """Test _get_query_bounds on Average query expr, with lower=upper."""
-    average = GroupByBoundedAverage(
-        child=PrivateSource("private"),
-        groupby_keys=KeySet.from_dict({}),
-        measure_column="",
-        low=bound,
-        high=bound,
-    )
-    (low, high) = _get_query_bounds(average)
-    assert low == high
-    expected = ExactNumber.from_float(bound, round_up=True)
-    assert low == expected
-    assert high == expected
-
-
-@pytest.mark.parametrize("bound", [(0), (-123456), (7899000)])
-def test_equal_upper_and_lower_stdev(bound: float) -> None:
-    """Test _get_query_bounds on STDEV query expr, with lower=upper."""
-    stdev = GroupByBoundedSTDEV(
-        child=PrivateSource("private"),
-        groupby_keys=KeySet.from_dict({}),
-        measure_column="",
-        low=bound,
-        high=bound,
-    )
-    (low, high) = _get_query_bounds(stdev)
-    assert low == high
-    expected = ExactNumber.from_float(bound, round_up=True)
-    assert low == expected
-    assert high == expected
-
-
-@pytest.mark.parametrize("bound", [(0), (-123456), (7899000)])
-def test_equal_upper_and_lower_sum(bound: float) -> None:
-    """Test _get_query_bounds on Sum query expr, with lower=upper."""
-    sum_query = GroupByBoundedSum(
-        child=PrivateSource("private"),
-        groupby_keys=KeySet.from_dict({}),
-        measure_column="",
-        low=bound,
-        high=bound,
-    )
-    (low, high) = _get_query_bounds(sum_query)
-    assert low == high
-    expected = ExactNumber.from_float(bound, round_up=True)
-    assert low == expected
-    assert high == expected
-
-
-@pytest.mark.parametrize("bound", [(0), (-123456), (7899000)])
-def test_equal_upper_and_lower_variance(bound: float) -> None:
-    """Test _get_query_bounds on Variance query expr, with lower=upper."""
-    variance = GroupByBoundedVariance(
-        child=PrivateSource("private"),
-        groupby_keys=KeySet.from_dict({}),
-        measure_column="",
-        low=bound,
-        high=bound,
-    )
-    (low, high) = _get_query_bounds(variance)
-    assert low == high
-    expected = ExactNumber.from_float(bound, round_up=True)
-    assert low == expected
-    assert high == expected
-
-
-@pytest.mark.parametrize("bound", [(0), (-123456), (7899000)])
-def test_equal_upper_and_lower_quantile(bound: float) -> None:
-    """Test _get_query_bounds on Quantile query expr, with lower=upper."""
-    quantile = GroupByQuantile(
-        child=PrivateSource("private"),
-        groupby_keys=KeySet.from_dict({}),
-        measure_column="",
-        low=bound,
-        high=bound,
-        quantile=0.5,
-    )
-    (low, high) = _get_query_bounds(quantile)
-    assert low == high
-    expected = ExactNumber.from_float(bound, round_up=True)
-    assert low == expected
-    assert high == expected
+### Tests just for _get_query_bounds. ###
 
 
 @pytest.mark.parametrize("lower,upper", [(0, 1), (-123456, 0), (7899000, 9999999)])
 def test_average(lower: float, upper: float) -> None:
     """Test _get_query_bounds on Average query expr, with lower!=upper."""
     average = GroupByBoundedAverage(
         child=PrivateSource("private"),
@@ -275,15 +185,15 @@
 
 
 @pytest.fixture(name="test_data", scope="class")
 def prepare_visitor(spark, request):
     """Setup tests."""
     input_domain = DictDomain(
         {
-            "private": SparkDataFrameDomain(
+            NamedTable("private"): SparkDataFrameDomain(
                 {
                     "A": SparkStringColumnDescriptor(),
                     "B": SparkIntegerColumnDescriptor(),
                     "X": SparkFloatColumnDescriptor(),
                     "null": SparkFloatColumnDescriptor(allow_null=True),
                     "nan": SparkFloatColumnDescriptor(allow_nan=True),
                     "inf": SparkFloatColumnDescriptor(allow_inf=True),
@@ -297,25 +207,28 @@
                         allow_nan=True, allow_inf=True
                     ),
                     "null_and_nan_and_inf": SparkFloatColumnDescriptor(
                         allow_null=True, allow_nan=True, allow_inf=True
                     ),
                 }
             ),
-            "private_2": SparkDataFrameDomain(
+            NamedTable("private_2"): SparkDataFrameDomain(
                 {
                     "A": SparkStringColumnDescriptor(),
                     "C": SparkIntegerColumnDescriptor(),
                 }
             ),
         }
     )
 
     input_metric = DictMetric(
-        {"private": SymmetricDifference(), "private_2": SymmetricDifference()}
+        {
+            NamedTable("private"): SymmetricDifference(),
+            NamedTable("private_2"): SymmetricDifference(),
+        }
     )
 
     public_sources = {
         "public": spark.createDataFrame(
             pd.DataFrame({"A": ["zero", "one"], "B": [0, 1]}),
             schema=StructType(
                 [
@@ -324,15 +237,15 @@
                 ]
             ),
         )
     }
     request.cls.base_query = PrivateSource(source_id="private")
 
     catalog = Catalog()
-    catalog.add_private_source(
+    catalog.add_private_table(
         "private",
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR),
             "B": ColumnDescriptor(ColumnType.INTEGER),
             "X": ColumnDescriptor(ColumnType.DECIMAL),
             "null": ColumnDescriptor(ColumnType.DECIMAL, allow_null=True),
             "nan": ColumnDescriptor(ColumnType.DECIMAL, allow_nan=True),
@@ -346,62 +259,70 @@
             "nan_and_inf": ColumnDescriptor(
                 ColumnType.DECIMAL, allow_nan=True, allow_inf=True
             ),
             "null_and_nan_and_inf": ColumnDescriptor(
                 ColumnType.DECIMAL, allow_null=True, allow_nan=True, allow_inf=True
             ),
         },
-        stability=3,
     )
-    catalog.add_private_view(
+    catalog.add_private_table(
         "private_2",
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR),
             "C": ColumnDescriptor(ColumnType.INTEGER),
         },
-        stability=3,
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "public",
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR),
             "B": ColumnDescriptor(ColumnType.INTEGER),
         },
     )
     request.cls.catalog = catalog
 
     budget = ExactNumber(10).expr
-    stability = {"private": ExactNumber(3).expr, "private_2": ExactNumber(3).expr}
+    stability = {
+        NamedTable("private"): ExactNumber(3).expr,
+        NamedTable("private_2"): ExactNumber(3).expr,
+    }
     request.cls.visitor = MeasurementVisitor(
         per_query_privacy_budget=budget,
         stability=stability,
         input_domain=input_domain,
         input_metric=input_metric,
         output_measure=PureDP(),
         default_mechanism=NoiseMechanism.LAPLACE,
         public_sources=public_sources,
         catalog=catalog,
+        table_constraints={t: [] for t in stability},
     )
     # for the methods which alter the output measure of a visitor.
     request.cls.pick_noise_visitor = MeasurementVisitor(
         per_query_privacy_budget=budget,
         stability=stability,
         input_domain=input_domain,
         input_metric=input_metric,
         output_measure=PureDP(),
         default_mechanism=NoiseMechanism.LAPLACE,
         public_sources=public_sources,
         catalog=catalog,
+        table_constraints={t: [] for t in stability},
     )
 
 
 @pytest.mark.usefixtures("test_data")
 class TestMeasurementVisitor:
     """Tests for Measurement Visitor."""
 
+    visitor: MeasurementVisitor
+    pick_noise_visitor: MeasurementVisitor
+    catalog: Catalog
+    base_query: QueryExpr
+
     @pytest.mark.parametrize(
         "query_mechanism,output_measure,expected_mechanism",
         [
             (CountMechanism.DEFAULT, PureDP(), NoiseMechanism.GEOMETRIC),
             (CountMechanism.DEFAULT, RhoZCDP(), NoiseMechanism.DISCRETE_GAUSSIAN),
             (CountMechanism.LAPLACE, PureDP(), NoiseMechanism.GEOMETRIC),
             (CountMechanism.LAPLACE, RhoZCDP(), NoiseMechanism.GEOMETRIC),
@@ -539,15 +460,15 @@
         expected_mechanism: Optional[NoiseMechanism],
     ) -> None:
         """Test _pick_noise_for_non_count for GroupByBoundedAverage query exprs."""
         query = GroupByBoundedAverage(
             child=self.base_query,
             measure_column="",
             low=0,
-            high=0,
+            high=1,
             mechanism=query_mechanism,
             groupby_keys=KeySet.from_dict({}),
         )
         self.pick_noise_visitor.output_measure = output_measure
         # pylint: disable=protected-access
         if expected_mechanism is not None:
             got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
@@ -632,15 +553,15 @@
         expected_mechanism: Optional[NoiseMechanism],
     ) -> None:
         """Test _pick_noise_for_non_count for GroupByBoundedSum query exprs."""
         query = GroupByBoundedSum(
             child=self.base_query,
             measure_column="",
             low=0,
-            high=0,
+            high=1,
             mechanism=query_mechanism,
             groupby_keys=KeySet.from_dict({}),
         )
         self.pick_noise_visitor.output_measure = output_measure
         # pylint: disable=protected-access
         if expected_mechanism is not None:
             got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
@@ -725,15 +646,15 @@
         expected_mechanism: Optional[NoiseMechanism],
     ) -> None:
         """Test _pick_noise_for_non_count for GroupByBoundedVariance query exprs."""
         query = GroupByBoundedVariance(
             child=self.base_query,
             measure_column="",
             low=0,
-            high=0,
+            high=1,
             mechanism=query_mechanism,
             groupby_keys=KeySet.from_dict({}),
         )
         self.pick_noise_visitor.output_measure = output_measure
         # pylint: disable=protected-access
         if expected_mechanism is not None:
             got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
@@ -818,15 +739,15 @@
         expected_mechanism: Optional[NoiseMechanism],
     ) -> None:
         """Test _pick_noise_for_non_count for GroupByBoundedSTDEV query exprs."""
         query = GroupByBoundedSTDEV(
             child=self.base_query,
             measure_column="",
             low=0,
-            high=0,
+            high=1,
             mechanism=query_mechanism,
             groupby_keys=KeySet.from_dict({}),
         )
         self.pick_noise_visitor.output_measure = output_measure
         # pylint: disable=protected-access
         if expected_mechanism is not None:
             got_mechanism = self.pick_noise_visitor._pick_noise_for_non_count(
@@ -866,42 +787,42 @@
             GroupByBoundedVariance,
         ]
         if isinstance(mechanism, AverageMechanism):
             query = GroupByBoundedAverage(
                 child=self.base_query,
                 measure_column="",
                 low=0,
-                high=0,
+                high=1,
                 mechanism=mechanism,
                 groupby_keys=KeySet.from_dict({}),
             )
         elif isinstance(mechanism, StdevMechanism):
             query = GroupByBoundedSTDEV(
                 child=self.base_query,
                 measure_column="",
                 low=0,
-                high=0,
+                high=1,
                 mechanism=mechanism,
                 groupby_keys=KeySet.from_dict({}),
             )
         elif isinstance(mechanism, SumMechanism):
             query = GroupByBoundedSum(
                 child=self.base_query,
                 measure_column="",
                 low=0,
-                high=0,
+                high=1,
                 mechanism=mechanism,
                 groupby_keys=KeySet.from_dict({}),
             )
         elif isinstance(mechanism, VarianceMechanism):
             query = GroupByBoundedVariance(
                 child=self.base_query,
                 measure_column="",
                 low=0,
-                high=0,
+                high=1,
                 mechanism=mechanism,
                 groupby_keys=KeySet.from_dict({}),
             )
         else:
             assert_never(mechanism)
         with pytest.raises(
             AssertionError, match="Query's measure column should be numeric."
@@ -989,230 +910,151 @@
         assert_frame_equal_with_sort(
             got.output_domain.group_keys.toPandas(),
             expected_output_domain.group_keys.toPandas(),
         )
         assert got.output_metric == expected_output_metric
 
     @pytest.mark.parametrize(
-        "query,expected_mid_stability,expected_mechanism,expected_new_child",
+        "query,expected_mid_stability,expected_mechanism",
         [
             (
                 GroupByBoundedAverage(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
                     measure_column="B",
                     low=-100,
                     high=100,
                     mechanism=AverageMechanism.LAPLACE,
                 ),
                 ExactNumber(3).expr,
                 NoiseMechanism.GEOMETRIC,
-                None,
             ),
             (
                 GroupByBoundedAverage(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
                     measure_column="nan",
                     low=-100,
                     high=100,
                     mechanism=AverageMechanism.LAPLACE,
                 ),
                 ExactNumber(3).expr,
                 NoiseMechanism.LAPLACE,
-                DropNullAndNan(child=PrivateSource("private"), columns=["nan"]),
             ),
             (
                 GroupByBoundedSum(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
                     measure_column="X",
                     low=-100,
                     high=100,
                     mechanism=SumMechanism.LAPLACE,
                 ),
                 ExactNumber(3).expr,
                 NoiseMechanism.LAPLACE,
-                None,
             ),
             (
                 GroupByBoundedSum(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
                     measure_column="null",
                     low=-100,
                     high=100,
                     mechanism=SumMechanism.LAPLACE,
                 ),
                 ExactNumber(3).expr,
                 NoiseMechanism.LAPLACE,
-                DropNullAndNan(child=PrivateSource("private"), columns=["null"]),
             ),
             (
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
                     measure_column="B",
                     low=-100,
                     high=100,
                     mechanism=VarianceMechanism.GAUSSIAN,
                 ),
                 ExactNumber(3).expr,
                 NoiseMechanism.DISCRETE_GAUSSIAN,
-                None,
             ),
             (
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
                     measure_column="inf",
                     low=-100,
                     high=100,
                     mechanism=VarianceMechanism.LAPLACE,
                 ),
                 ExactNumber(3).expr,
                 NoiseMechanism.LAPLACE,
-                ReplaceInfExpr(
-                    child=PrivateSource("private"), replace_with={"inf": (-100, 100)}
-                ),
             ),
             (
                 GroupByBoundedSTDEV(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
                     measure_column="B",
                     low=-100,
                     high=100,
                     mechanism=StdevMechanism.DEFAULT,
                 ),
                 ExactNumber(3).expr,
                 NoiseMechanism.GEOMETRIC,
-                None,
             ),
             (
                 GroupByBoundedSTDEV(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero", "one"]}),
                     measure_column="null_and_nan_and_inf",
                     low=-100,
                     high=100,
                     mechanism=StdevMechanism.DEFAULT,
                 ),
                 ExactNumber(3).expr,
                 NoiseMechanism.LAPLACE,
-                ReplaceInfExpr(
-                    child=DropNullAndNan(
-                        child=PrivateSource("private"), columns=["null_and_nan_and_inf"]
-                    ),
-                    replace_with={"null_and_nan_and_inf": (-100, 100)},
-                ),
             ),
         ],
     )
     def test_build_common(
         self,
         query: Union[
             GroupByBoundedAverage,
             GroupByBoundedSTDEV,
             GroupByBoundedSum,
             GroupByBoundedVariance,
         ],
         expected_mid_stability: sp.Expr,
         expected_mechanism: NoiseMechanism,
-        expected_new_child: Optional[QueryExpr],
     ):
         """Test _build_common."""
         info = self.visitor._build_common(query)  # pylint: disable=protected-access
-        get_value_transformation: GetValue
-        if expected_new_child is None:
-            assert isinstance(info.transformation, GetValue)
-            get_value_transformation = info.transformation
-        else:
-            expected_null_nan_columns: List[str] = []
-            expected_inf_replace: Dict[str, Tuple[float, float]] = {}
-            if isinstance(expected_new_child, ReplaceInfExpr):
-                expected_inf_replace = expected_new_child.replace_with
-                if isinstance(expected_new_child.child, DropNullAndNan):
-                    expected_null_nan_columns = expected_new_child.child.columns
-            if isinstance(expected_new_child, DropNullAndNan):
-                expected_null_nan_columns = expected_new_child.columns
-            assert isinstance(info.transformation, ChainTT)
-            transformations = chain_to_list(info.transformation)
-            assert isinstance(transformations[0], GetValue)
-            get_value_transformation = transformations[0]
-            got_null_nan_columns: List[str] = []
-            for t in transformations[1:]:
-                assert isinstance(t, (ReplaceInfTransformation, DropNaNs, DropNulls))
-                if isinstance(t, ReplaceInfTransformation):
-                    assert sorted(list(t.replace_map.keys())) == sorted(
-                        list(expected_inf_replace)
-                    )
-                    for k, v in t.replace_map.items():
-                        assert v == expected_inf_replace[k]
-                elif isinstance(t, DropNaNs):
-                    got_null_nan_columns += t.columns
-                elif isinstance(t, DropNulls):
-                    got_null_nan_columns += t.columns
-            assert sorted(list(set(got_null_nan_columns))) == sorted(
-                expected_null_nan_columns
-            )
-        assert get_value_transformation.key == "private"
-        assert get_value_transformation.input_domain == self.visitor.input_domain
-        assert get_value_transformation.input_metric == self.visitor.input_metric
-        assert (
-            get_value_transformation.output_domain
-            == self.visitor.input_domain["private"]
-        )
-        assert (
-            get_value_transformation.output_metric
-            == self.visitor.input_metric["private"]
-        )
+        transformation: ChainTT
+        assert isinstance(info.transformation, ChainTT)
+        transformation = info.transformation
+
+        assert transformation.input_domain == self.visitor.input_domain
+        assert transformation.input_metric == self.visitor.input_metric
 
         assert info.mechanism == expected_mechanism
         assert info.mid_stability == expected_mid_stability
         assert info.lower_bound == ExactNumber.from_float(query.low, round_up=True)
         assert info.upper_bound == ExactNumber.from_float(query.high, round_up=False)
 
         assert isinstance(info.groupby, GroupBy)
-        assert isinstance(self.visitor.input_domain["private"], SparkDataFrameDomain)
+        table_domain = transformation.output_domain
+        assert isinstance(table_domain, SparkDataFrameDomain)
         expected_groupby_domain = SparkGroupedDataFrameDomain(
-            schema=self.visitor.input_domain["private"].schema.copy(),
-            group_keys=query.groupby_keys.dataframe(),
+            schema=dict(table_domain.schema), group_keys=query.groupby_keys.dataframe()
         )
-        if expected_new_child is not None:
-            new_transform: QueryExpr = expected_new_child
-            while isinstance(new_transform, (ReplaceInfExpr, DropNullAndNan)):
-                if isinstance(new_transform, ReplaceInfExpr):
-                    replace_inf_expr: ReplaceInfExpr = new_transform
-                    schema = expected_groupby_domain.schema
-                    for col in replace_inf_expr.replace_with:
-                        if isinstance(schema[col], SparkFloatColumnDescriptor):
-                            schema[col] = SparkFloatColumnDescriptor(allow_inf=False)
-                    new_transform = replace_inf_expr.child
-                elif isinstance(new_transform, DropNullAndNan):
-                    drop_null_and_nan_expr: DropNullAndNan = new_transform
-                    schema = expected_groupby_domain.schema
-                    for col in new_transform.columns:
-                        if isinstance(schema[col], SparkFloatColumnDescriptor):
-                            schema[col] = SparkFloatColumnDescriptor(
-                                allow_null=False, allow_nan=False
-                            )
-                        else:
-                            schema[col] = SparkIntegerColumnDescriptor(allow_null=False)
-                    new_transform = drop_null_and_nan_expr.child
-                expected_groupby_domain = SparkGroupedDataFrameDomain(
-                    schema=schema, group_keys=query.groupby_keys.dataframe()
-                )
         assert isinstance(info.groupby.output_domain, SparkGroupedDataFrameDomain)
         assert info.groupby.output_domain.schema == expected_groupby_domain.schema
         assert_frame_equal_with_sort(
             info.groupby.output_domain.group_keys.toPandas(),
             expected_groupby_domain.group_keys.toPandas(),
         )
-        assert info.new_child == expected_new_child
 
     def test_validate_measurement(self):
         """Test _validate_measurement."""
         with patch(
             "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
             autospec=True,
         ) as mock_measurement:
@@ -1227,32 +1069,23 @@
             with pytest.raises(
                 AssertionError,
                 match="Privacy function does not match per-query privacy budget.",
             ):
                 self.visitor._validate_measurement(mock_measurement, mid_stability)
             # pylint: enable=protected-access
 
-    def _check_measurement(
-        self, measurement: Measurement, child_is_base_query: bool = True
-    ):
+    def _check_measurement(self, measurement: Measurement):
         """Check the basic attributes of a measurement (for all query exprs).
 
-        If ``child_is_base_query`` is true, it is assumed that the child
-        query was ``PrivateSource("private")``.
-
         The measurement almost certainly looks like this:
         ``child_transformation | mock_measurement``
         so extensive testing of the latter is likely to be counterproductive.
         """
         assert isinstance(measurement, ChainTM)
 
-        if child_is_base_query:
-            assert isinstance(measurement.transformation, GetValue)
-            assert measurement.transformation.key == "private"
-
         assert measurement.transformation.input_domain == self.visitor.input_domain
         assert measurement.transformation.input_metric == self.visitor.input_metric
         assert isinstance(
             measurement.transformation.output_domain, SparkDataFrameDomain
         )
         assert (
             measurement.transformation.output_domain
@@ -1287,20 +1120,24 @@
         self,
         mock_measurement,
         child_query: QueryExpr,
         expected_mechanism: NoiseMechanism,
     ) -> None:
         """Initialize a mock measurement."""
         # pylint: disable=protected-access
-        transformation = self.visitor._visit_child_transformation(
+        transformation, reference, _ = self.visitor._visit_child_transformation(
             child_query, expected_mechanism
         )
         # pylint: enable=protected-access
-        mock_measurement.input_domain = transformation.output_domain
-        mock_measurement.input_metric = transformation.output_metric
+        mock_measurement.input_domain = lookup_domain(
+            transformation.output_domain, reference
+        )
+        mock_measurement.input_metric = lookup_metric(
+            transformation.output_metric, reference
+        )
         mock_measurement.privacy_function.return_value = self.visitor.budget
 
     @pytest.mark.parametrize(
         "query,output_measure,expected_mechanism",
         [
             (
                 GroupByCount(
@@ -1365,24 +1202,24 @@
             "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
             autospec=True,
         ) as mock_measurement, patch(
             "tmlt.analytics._query_expr_compiler."
             + "_measurement_visitor.create_count_measurement",
             autospec=True,
         ) as mock_create_count:
-
             self.visitor.output_measure = output_measure
             self._setup_mock_measurement(
                 mock_measurement, query.child, expected_mechanism
             )
             mock_create_count.return_value = mock_measurement
 
             measurement = self.visitor.visit_groupby_count(query)
+            assert isinstance(measurement, ChainTM)
 
-            self._check_measurement(measurement, query.child == self.base_query)
+            self._check_measurement(measurement)
             self.check_mock_groupby_call(
                 mock_groupby,
                 measurement.transformation,
                 query.groupby_keys,
                 expected_mechanism,
             )
 
@@ -1475,67 +1312,45 @@
             "tmlt.analytics._query_expr_compiler._measurement_visitor.Measurement",
             autospec=True,
         ) as mock_measurement, patch(
             "tmlt.analytics._query_expr_compiler."
             + "_measurement_visitor.create_count_distinct_measurement",
             autospec=True,
         ) as mock_create_count_distinct:
-
             self.visitor.output_measure = output_measure
 
-            mock_measurement.privacy_function.return_value = self.visitor.budget
             mock_create_count_distinct.return_value = mock_measurement
-            # Sometimes a CountDistinct query needs to know which columns to select
-            query_needs_columns_selected = (
-                query.columns_to_count is not None and len(query.columns_to_count) > 0
-            )
-
-            expected_child_query: QueryExpr
-            expected_child_query = query.child
-            # If it is expected that a query will need a
-            # specific set of columns selected,
-            # make that expected Select query now
-            # (since the function modifies the query)
-            if query_needs_columns_selected:
-                # Build the list of columns that we're expecting to group by
-                groupby_columns: List[str] = list(query.groupby_keys.schema().keys())
-                # There is literally no way this cannot be true,
-                # but if you leave this out then MyPy will complain.
-                assert query.columns_to_count is not None
-                expected_child_query = SelectExpr(
-                    child=query.child, columns=query.columns_to_count + groupby_columns
-                )
             self._setup_mock_measurement(
-                mock_measurement, expected_child_query, expected_mechanism
+                mock_measurement, query.child, expected_mechanism
             )
+            if query.columns_to_count:
+                select_columns = query.columns_to_count + list(
+                    query.groupby_keys.schema().keys()
+                )
+                mock_measurement.input_domain = SparkDataFrameDomain(
+                    {
+                        c: d
+                        for c, d in mock_measurement.input_domain.schema.items()
+                        if c in select_columns
+                    }
+                )
 
             measurement = self.visitor.visit_groupby_count_distinct(query)
 
-            self._check_measurement(
-                measurement,
-                (query.child == self.base_query and not query_needs_columns_selected),
-            )
+            self._check_measurement(measurement)
             assert isinstance(measurement, ChainTM)
             assert measurement.measurement == mock_measurement
-            if query_needs_columns_selected:
+            if query.columns_to_count:
                 assert isinstance(measurement.transformation, ChainTT)
-                if query.child == self.base_query:
-                    assert isinstance(
-                        measurement.transformation.transformation1, GetValue
-                    )
-                    get_value = measurement.transformation.transformation1
-                    assert isinstance(get_value, GetValue)
-                    assert get_value.key == "private"
                 assert isinstance(
                     measurement.transformation.transformation2, SelectTransformation
                 )
-                select_transformation = measurement.transformation.transformation2
-                assert isinstance(select_transformation, SelectTransformation)
-                assert isinstance(expected_child_query, SelectExpr)
-                assert select_transformation.columns == expected_child_query.columns
+                assert (
+                    measurement.transformation.transformation2.columns == select_columns
+                )
 
             mid_stability = measurement.transformation.stability_function(
                 self.visitor.stability
             )
 
             assert measurement.measurement == mock_measurement
             self.check_mock_groupby_call(
@@ -1621,45 +1436,45 @@
             (
                 GroupByQuantile(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     quantile=0.5,
                     measure_column="X",
                     low=0,
-                    high=0,
+                    high=1,
                 ),
                 RhoZCDP(),
                 None,
             ),
             (
                 GroupByQuantile(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     quantile=0.5,
                     measure_column="nan_and_inf",
                     low=0,
-                    high=0,
+                    high=1,
                 ),
                 RhoZCDP(),
                 ReplaceInfExpr(
                     DropNullAndNan(PrivateSource("private"), ["nan_and_inf"]),
-                    {"nan_and_inf": (0, 0)},
+                    {"nan_and_inf": (0, 1)},
                 ),
             ),
             (
                 GroupByQuantile(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     quantile=0.5,
                     measure_column="inf",
                     low=0,
-                    high=0,
+                    high=1,
                 ),
                 RhoZCDP(),
-                ReplaceInfExpr(PrivateSource("private"), {"inf": (0, 0)}),
+                ReplaceInfExpr(PrivateSource("private"), {"inf": (0, 1)}),
             ),
         ],
     )
     def test_visit_groupby_quantile(
         self,
         query: GroupByQuantile,
         output_measure: Union[PureDP, RhoZCDP],
@@ -1688,18 +1503,15 @@
             self._setup_mock_measurement(
                 mock_measurement, expected_child_query, expected_mechanism
             )
             mock_create_quantile.return_value = mock_measurement
 
             measurement = self.visitor.visit_groupby_quantile(query)
 
-            self._check_measurement(
-                measurement,
-                query.child == self.base_query and expected_new_child is None,
-            )
+            self._check_measurement(measurement)
             assert isinstance(measurement, ChainTM)
             assert measurement.measurement == mock_measurement
             self.check_mock_groupby_call(
                 mock_groupby,
                 measurement.transformation,
                 query.groupby_keys,
                 expected_mechanism,
@@ -1718,46 +1530,14 @@
                 d_in=mid_stability,
                 d_out=self.visitor.budget,
                 output_measure=self.visitor.output_measure,
                 groupby_transformation=mock_groupby.return_value,
                 quantile_column=query.output_column,
             )
 
-            # Check for the drop transformations, if expected
-            if expected_new_child is not None:
-                expected_null_nan_columns: List[str] = []
-                expected_inf_replace: Dict[str, Tuple[float, float]] = {}
-                if isinstance(expected_new_child, ReplaceInfExpr):
-                    expected_inf_replace = expected_new_child.replace_with
-                    if isinstance(expected_new_child.child, DropNullAndNan):
-                        expected_null_nan_columns = expected_new_child.child.columns
-                elif isinstance(expected_new_child, DropNullAndNan):
-                    expected_null_nan_columns = expected_new_child.columns
-                assert isinstance(measurement.transformation, ChainTT)
-                transformations = chain_to_list(measurement.transformation)
-                assert isinstance(transformations[0], GetValue)
-                got_null_nan_columns: List[str] = []
-                for t in transformations[1:]:
-                    assert isinstance(
-                        t, (ReplaceInfTransformation, DropNaNs, DropNulls)
-                    )
-                    if isinstance(t, ReplaceInfTransformation):
-                        assert sorted(list(t.replace_map.keys())) == sorted(
-                            list(expected_inf_replace.keys())
-                        )
-                        for k, v in t.replace_map.items():
-                            assert v == expected_inf_replace[k]
-                    elif isinstance(t, DropNaNs):
-                        got_null_nan_columns += t.columns
-                    elif isinstance(t, DropNulls):
-                        got_null_nan_columns += t.columns
-                assert sorted(list(set(got_null_nan_columns))) == sorted(
-                    expected_null_nan_columns
-                )
-
     @pytest.mark.parametrize(
         "query,output_measure,expected_mechanism",
         [
             (
                 GroupByBoundedSum(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
@@ -1799,15 +1579,15 @@
             (
                 GroupByBoundedSum(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     mechanism=SumMechanism.DEFAULT,
                     measure_column="B",
                     low=0,
-                    high=0,
+                    high=1,
                 ),
                 RhoZCDP(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
         ],
     )
     def test_visit_groupby_bounded_sum(
@@ -1833,15 +1613,15 @@
             self._setup_mock_measurement(
                 mock_measurement, query.child, expected_mechanism
             )
             mock_create_sum.return_value = mock_measurement
 
             measurement = self.visitor.visit_groupby_bounded_sum(query)
 
-            self._check_measurement(measurement, query.child == self.base_query)
+            self._check_measurement(measurement)
             assert isinstance(measurement, ChainTM)
             assert measurement.measurement == mock_measurement
             self.check_mock_groupby_call(
                 mock_groupby,
                 measurement.transformation,
                 query.groupby_keys,
                 expected_mechanism,
@@ -1910,15 +1690,15 @@
             (
                 GroupByBoundedAverage(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     mechanism=AverageMechanism.DEFAULT,
                     measure_column="B",
                     low=0,
-                    high=0,
+                    high=1,
                 ),
                 RhoZCDP(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
         ],
     )
     def test_visit_groupby_bounded_average(
@@ -1944,15 +1724,15 @@
             self._setup_mock_measurement(
                 mock_measurement, query.child, expected_mechanism
             )
             mock_create_average.return_value = mock_measurement
 
             measurement = self.visitor.visit_groupby_bounded_average(query)
 
-            self._check_measurement(measurement, query.child == self.base_query)
+            self._check_measurement(measurement)
             assert isinstance(measurement, ChainTM)
             assert measurement.measurement == mock_measurement
             self.check_mock_groupby_call(
                 mock_groupby,
                 measurement.transformation,
                 query.groupby_keys,
                 expected_mechanism,
@@ -2021,15 +1801,15 @@
             (
                 GroupByBoundedVariance(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     mechanism=VarianceMechanism.DEFAULT,
                     measure_column="B",
                     low=0,
-                    high=0,
+                    high=1,
                 ),
                 RhoZCDP(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
         ],
     )
     def test_visit_groupby_bounded_variance(
@@ -2055,15 +1835,15 @@
             self._setup_mock_measurement(
                 mock_measurement, query.child, expected_mechanism
             )
             mock_create_variance.return_value = mock_measurement
 
             measurement = self.visitor.visit_groupby_bounded_variance(query)
 
-            self._check_measurement(measurement, query.child == self.base_query)
+            self._check_measurement(measurement)
             assert isinstance(measurement, ChainTM)
             assert measurement.measurement == mock_measurement
             self.check_mock_groupby_call(
                 mock_groupby,
                 measurement.transformation,
                 query.groupby_keys,
                 expected_mechanism,
@@ -2132,15 +1912,15 @@
             (
                 GroupByBoundedSTDEV(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({"A": ["zero"]}),
                     mechanism=StdevMechanism.DEFAULT,
                     measure_column="B",
                     low=0,
-                    high=0,
+                    high=1,
                 ),
                 RhoZCDP(),
                 NoiseMechanism.DISCRETE_GAUSSIAN,
             ),
         ],
     )
     def test_visit_groupby_bounded_stdev(
@@ -2167,15 +1947,15 @@
             self._setup_mock_measurement(
                 mock_measurement, query.child, expected_mechanism
             )
             mock_create_stdev.return_value = mock_measurement
 
             measurement = self.visitor.visit_groupby_bounded_stdev(query)
 
-            self._check_measurement(measurement, query.child == self.base_query)
+            self._check_measurement(measurement)
             assert isinstance(measurement, ChainTM)
             assert measurement.measurement == mock_measurement
             self.check_mock_groupby_call(
                 mock_groupby,
                 measurement.transformation,
                 query.groupby_keys,
                 expected_mechanism,
@@ -2200,31 +1980,31 @@
             )
 
     @pytest.mark.parametrize(
         "query",
         [
             (PrivateSource("private")),
             (Rename(child=PrivateSource("private"), column_mapper={"A": "A2"})),
-            (Filter(child=PrivateSource("private"), predicate="B > 2")),
+            (Filter(child=PrivateSource("private"), condition="B > 2")),
             (SelectExpr(child=PrivateSource("private"), columns=["A"])),
             (
                 Map(
                     child=PrivateSource("private"),
                     f=lambda row: {"C": "c" + str(row["B"])},
                     schema_new_columns=Schema({"C": "VARCHAR"}),
                     augment=True,
                 )
             ),
             (
                 FlatMap(
                     child=PrivateSource("private"),
                     f=lambda row: [{"i": n for n in range(row["B"] + 1)}],
-                    max_num_rows=11,
                     schema_new_columns=Schema({"i": "DECIMAL"}),
                     augment=False,
+                    max_num_rows=11,
                 )
             ),
             (
                 JoinPrivate(
                     child=PrivateSource("private"),
                     right_operand_expr=PrivateSource("private_2"),
                     truncation_strategy_left=TruncationStrategy.DropExcess(3),
```

### Comparing `tmlt_analytics-0.6.1/test/unit/query_expr_compiler/test_output_schema_visitor.py` & `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/test_output_schema_visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-# type: ignore[attr-defined]
-# pylint: disable=no-self-use, protected-access, no-member
 """Tests for OutputSchemaVisitor."""
+
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2023
+
+# pylint: disable=no-self-use, protected-access, no-member
+
 import datetime
-import re
 from typing import Dict, List, Type
 
 import pytest
 from pyspark.sql import SparkSession
 from pyspark.sql.types import LongType, StringType, StructField, StructType
 
 from tmlt.analytics._catalog import Catalog
@@ -67,184 +70,174 @@
         [], schema=StructType([StructField("A", LongType(), False)])
     )
 )
 
 OUTPUT_SCHEMA_INVALID_QUERY_TESTS = [
     (  # Query references public source instead of private source
         PrivateSource("public"),
-        "Attempted query on 'public'. 'public' is not a private table.",
+        "Attempted query on table 'public', which is not a private table",
     ),
     (  # JoinPublic has invalid public_id
         JoinPublic(child=PrivateSource("private"), public_table="private"),
-        "Attempted JoinPublic on 'private' table. 'private' is not a public table.",
+        "Attempted public join on table 'private', which is not a public table",
     ),
     (  # JoinPublic references invalid private source
         JoinPublic(
             child=PrivateSource("private_source_not_in_catalog"), public_table="public"
         ),
-        "Query references invalid source 'private_source_not_in_catalog'.",
+        "Query references nonexistent table 'private_source_not_in_catalog'",
     ),
     (  # JoinPublic on columns not common to both tables
         JoinPublic(
             child=PrivateSource("private"), public_table="public", join_columns=["B"]
         ),
-        "Join columns must be common to both tables.",
+        "Join columns must be common to both tables",
     ),
     (  # JoinPrivate on columns not common to both tables
         JoinPrivate(
             PrivateSource("private"),
             Rename(PrivateSource("private"), {"B": "Q"}),
             TruncationStrategy.DropExcess(1),
             TruncationStrategy.DropExcess(1),
             join_columns=["B"],
         ),
-        "Join columns must be common to both tables.",
+        "Join columns must be common to both tables",
     ),
     (  # JoinPublic on tables with no common columns
         JoinPublic(
             child=Rename(PrivateSource("private"), {"A": "Q"}), public_table="public"
         ),
-        "Tables have no common columns to join on.",
+        "Tables have no common columns to join on",
     ),
     (  # JoinPrivate on tables with no common columns
         JoinPrivate(
             PrivateSource("private"),
-            Rename(
-                PrivateSource("private"),
-                {"A": "ZA", "B": "ZB", "X": "ZX", "D": "ZD", "T": "ZT"},
-            ),
+            Rename(Select(PrivateSource("private"), ["A"]), {"A": "Z"}),
             TruncationStrategy.DropExcess(1),
             TruncationStrategy.DropExcess(1),
         ),
-        "Tables have no common columns to join on.",
+        "Tables have no common columns to join on",
     ),
     (  # JoinPublic on column with mismatched types
         JoinPublic(
             child=PrivateSource("private"), public_table="public", join_columns=["A"]
         ),
-        "Join columns must have identical types on both tables.",
+        "Join columns must have identical types on both tables, "
+        "but column 'A' does not",
     ),
     (  # JoinPrivate on column with mismatched types
         JoinPrivate(
             PrivateSource("private"),
             Rename(Rename(PrivateSource("private"), {"A": "Q"}), {"B": "A"}),
             TruncationStrategy.DropExcess(1),
             TruncationStrategy.DropExcess(1),
             join_columns=["A"],
         ),
-        "Join columns must have identical types on both tables.",
+        "Join columns must have identical types on both tables, "
+        "but column 'A' does not",
     ),
     (  # Filter on invalid column
-        Filter(child=PrivateSource("private"), predicate="NONEXISTENT>1"),
-        "Invalid filter expression: 'NONEXISTENT>1' in Filter query.",
+        Filter(child=PrivateSource("private"), condition="NONEXISTENT>1"),
+        "Invalid filter condition 'NONEXISTENT>1'.*",
     ),
     (  # Rename on non-existent column
         Rename(child=PrivateSource("private"), column_mapper={"NONEXISTENT": "Z"}),
-        "Non existent columns {'NONEXISTENT'} in Rename query.",
+        "Nonexistent columns {'NONEXISTENT'} in rename query",
     ),
     (  # Rename when column exists
         Rename(child=PrivateSource("private"), column_mapper={"A": "B"}),
-        "Cannot rename 'A' to 'B'. Column 'B' already exists.",
+        "Cannot rename 'A' to 'B': column 'B' already exists",
     ),
     (  # Select non-existent column
         Select(child=PrivateSource("private"), columns=["NONEXISTENT"]),
-        "Non existent columns {'NONEXISTENT'} in Select query.",
+        "Nonexistent columns {'NONEXISTENT'} in select query",
     ),
     (  # Nested grouping FlatMap
         FlatMap(
             child=FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"i": row["X"]} for i in range(row["Repeat"])],
-                max_num_rows=2,
                 schema_new_columns=Schema({"i": "INTEGER"}, grouping_column="i"),
                 augment=True,
+                max_num_rows=2,
             ),
             f=lambda row: [{"j": row["X"]} for i in range(row["Repeat"])],
-            max_num_rows=2,
             schema_new_columns=Schema({"j": "INTEGER"}, grouping_column="j"),
             augment=True,
+            max_num_rows=2,
         ),
         "Multiple grouping transformations are used in this query. "
         "Only one grouping transformation is allowed.",
     ),
     (  # FlatMap with inner grouping FlatMap but outer augment=False
         FlatMap(
             child=FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"i": row["X"]} for i in range(row["Repeat"])],
-                max_num_rows=2,
                 schema_new_columns=Schema({"i": "INTEGER"}, grouping_column="i"),
                 augment=True,
+                max_num_rows=2,
             ),
             f=lambda row: [{"j": row["X"]} for i in range(row["Repeat"])],
-            max_num_rows=2,
             schema_new_columns=Schema({"j": "INTEGER"}),
             augment=False,
+            max_num_rows=2,
         ),
-        "Need to set augment=True to ensure that the grouping column is available for "
-        "groupby.",
+        "Flat map must set augment=True to ensure that grouping column 'i' is not lost",
     ),
     (  # Map with inner grouping FlatMap but outer augment=False
         Map(
             child=FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"i": row["X"]} for i in range(row["Repeat"])],
-                max_num_rows=2,
                 schema_new_columns=Schema({"i": "INTEGER"}, grouping_column="i"),
                 augment=True,
+                max_num_rows=2,
             ),
             f=lambda row: {"C": 2 * str(row["B"])},
             schema_new_columns=Schema({"C": "VARCHAR"}),
             augment=False,
         ),
-        "Need to set augment=True to ensure that the grouping column is available for "
-        "groupby.",
+        "Map must set augment=True to ensure that grouping column 'i' is not lost",
     ),
     (  # ReplaceNullAndNan with a column that doesn't exist
         ReplaceNullAndNan(
-            child=PrivateSource("private"), replace_with={"bad_column": "new_string"}
+            child=PrivateSource("private"), replace_with={"bad": "new_string"}
         ),
-        "ReplaceNullAndNan.replace_with contains a replacement value for the column"
-        " bad_column, but data has no column named bad_column",
+        r"Column 'bad' does not exist in this table, available columns are \[.*\]",
     ),
     (
         # ReplaceNullAndNan with bad replacement type
         ReplaceNullAndNan(
             child=PrivateSource("private"), replace_with={"B": "not_an_int"}
         ),
-        "ReplaceNullAndNan.replace_with has column B's default value set to not_an_int,"
-        " which does not match the column type INTEGER",
+        "Column 'B' cannot have nulls replaced with 'not_an_int', as .* type INTEGER",
     ),
     (
         # ReplaceInfinity with nonexistent column
         ReplaceInfinity(
             child=PrivateSource("private"), replace_with={"wrong": (-1, 1)}
         ),
-        "ReplaceInfinity.replace_with contains replacement values for the column wrong,"
-        " but data has no column named wrong",
+        r"Column 'wrong' does not exist in this table, available columns are \[.*\]",
     ),
     (
         #  ReplaceInfinity with non-decimal column
         ReplaceInfinity(child=PrivateSource("private"), replace_with={"A": (-1, 1)}),
-        re.escape(
-            "ReplaceInfinity.replace_with contains replacement values for the column A,"
-            " but the column A has type VARCHAR (not DECIMAL)"
-        ),
+        r"Column 'A' has a replacement value provided.*of type VARCHAR \(not DECIMAL\) "
+        "and so cannot contain infinite values",
     ),
     (
         # DropNullAndNan with column that doesn't exist
         DropNullAndNan(child=PrivateSource("private"), columns=["bad"]),
-        "DropNullAndNan.columns contains the column bad, but data has no column"
-        " named bad",
+        r"Column 'bad' does not exist in this table, available columns are \[.*\]",
     ),
     (
         # DropInfinity with column that doesn't exist
         DropInfinity(child=PrivateSource("private"), columns=["bad"]),
-        "DropInfinity.columns contains the column bad, but data has no column"
-        " named bad",
+        r"Column 'bad' does not exist in this table, available columns are \[.*\]",
     ),
     (  # Type mismatch for the measure column of GroupByQuantile
         GroupByQuantile(
             child=PrivateSource("private"),
             groupby_keys=KeySet.from_dict({"B": [0, 1, 2]}),
             measure_column="A",
             quantile=0.5,
@@ -267,88 +260,87 @@
         "Expected types: 'INTEGER' or 'DECIMAL'",
     ),
     (  # Grouping column is set in a FlatMap but not used in a later GroupBy
         GroupByCount(
             child=FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"i": row["B"]} for i in range(row["Repeat"])],
-                max_num_rows=2,
                 schema_new_columns=Schema({"i": "INTEGER"}, grouping_column="i"),
                 augment=True,
+                max_num_rows=2,
             ),
             groupby_keys=KeySet.from_dict({"B": [0, 1, 2]}),
         ),
-        "Column produced by grouping transformation 'i' is not in groupby columns",
+        "Column 'i' produced by grouping transformation is not in groupby columns",
     ),
     (  # Grouping column is set but not used in a later groupby_public_source
         GroupByCount(
             child=FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"i": row["B"]} for i in range(row["Repeat"])],
-                max_num_rows=2,
                 schema_new_columns=Schema({"i": "INTEGER"}, grouping_column="i"),
                 augment=True,
+                max_num_rows=2,
             ),
             # pylint: disable=protected-access
             groupby_keys=KeySet(dataframe=GET_GROUPBY_COLUMN_A),
         ),
-        "Column produced by grouping transformation 'i' is not in groupby columns",
+        "Column 'i' produced by grouping transformation is not in groupby columns",
     ),
 ]
 
 ###TESTS FOR QUERY VALIDATION###
 
 
 @pytest.fixture(name="validation_visitor", scope="class")
 def setup_validation(request):
     """Set up test data."""
     catalog = Catalog()
-    catalog.add_private_source(
+    catalog.add_private_table(
         "private",
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR),
             "B": ColumnDescriptor(ColumnType.INTEGER),
             "X": ColumnDescriptor(ColumnType.DECIMAL),
             "D": ColumnDescriptor(ColumnType.DATE),
             "T": ColumnDescriptor(ColumnType.TIMESTAMP),
         },
-        stability=1,
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "public", spark_schema_to_analytics_columns(GET_PUBLIC().schema)
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "groupby_column_a",
         spark_schema_to_analytics_columns(GET_GROUPBY_COLUMN_A().schema),
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "groupby_column_b",
         spark_schema_to_analytics_columns(GET_GROUPBY_COLUMN_B().schema),
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "groupby_non_existing_column",
         spark_schema_to_analytics_columns(GET_GROUPBY_NON_EXISTING_COLUMN().schema),
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "groupby_column_wrong_type",
         spark_schema_to_analytics_columns(GET_GROUPBY_COLUMN_WRONG_TYPE().schema),
     )
-    catalog.add_private_view(
-        "groupby_one_column_private",
-        {"A": ColumnDescriptor(ColumnType.VARCHAR)},
-        stability=1,
+    catalog.add_private_table(
+        "groupby_one_column_private", {"A": ColumnDescriptor(ColumnType.VARCHAR)}
     )
     visitor = OutputSchemaVisitor(catalog)
     request.cls.visitor = visitor
 
 
 @pytest.mark.usefixtures("validation_visitor")
 class TestValidation:
     """Test Validation with Visitor."""
 
+    visitor: OutputSchemaVisitor
+
     @pytest.mark.parametrize(
         "query_expr,expected_error_msg", OUTPUT_SCHEMA_INVALID_QUERY_TESTS
     )
     def test_invalid_query_expr(
         self, query_expr: QueryExpr, expected_error_msg: str
     ) -> None:
         """Check that appropriate exceptions are raised on invalid queries."""
@@ -363,16 +355,16 @@
                 ValueError,
                 "Groupby column 'A' has type 'INTEGER', but the column "
                 "with the same name in the input data has type 'VARCHAR' instead.",
             ),
             (
                 KeySet.from_dict({"X": [0, 1]}),
                 ValueError,
-                "Groupby column 'X' has type 'INTEGER', but the column with the same"
-                " name in the input data has type 'DECIMAL' instead.",
+                "Groupby column 'X' has type 'INTEGER', but the column with the"
+                " same name in the input data has type 'DECIMAL' instead.",
             ),
             (
                 KeySet.from_dict({"Y": ["0"]}),
                 KeyError,
                 "Groupby column 'Y' is not in the input schema.",
             ),
             (
@@ -445,95 +437,81 @@
         for DataClass in [
             GroupByBoundedAverage,
             GroupByBoundedSTDEV,
             GroupByBoundedSum,
             GroupByBoundedVariance,
         ]:
             with pytest.raises(exception_type, match=expected_error_msg):
-                DataClass(  # type: ignore
-                    PrivateSource("private"), groupby_keys, "B", 1.0, 5.0
-                ).accept(self.visitor)
+                DataClass(PrivateSource("private"), groupby_keys, "B", 1.0, 5.0).accept(
+                    self.visitor
+                )
         with pytest.raises(exception_type, match=expected_error_msg):
             GroupByQuantile(
                 PrivateSource("private"), groupby_keys, "B", 0.5, 1.0, 5.0
             ).accept(self.visitor)
 
 
 ###QUERY VALIDATION WITH NULLS###
 @pytest.fixture(name="test_data_nulls", scope="class")
-def setup_visitor_with_nulls(request):
+def setup_visitor_with_nulls(request) -> None:
     """Set up test data."""
     catalog = Catalog()
-    catalog.add_private_source(
+    catalog.add_private_table(
         "private",
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True),
             "B": ColumnDescriptor(ColumnType.INTEGER, allow_null=True),
             "X": ColumnDescriptor(
                 ColumnType.DECIMAL, allow_null=True, allow_inf=True, allow_nan=True
             ),
             "D": ColumnDescriptor(ColumnType.DATE, allow_null=True),
             "T": ColumnDescriptor(ColumnType.TIMESTAMP, allow_null=True),
             "NOTNULL": ColumnDescriptor(ColumnType.INTEGER, allow_null=False),
         },
-        stability=1,
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "public",
         {
             "A": ColumnDescriptor(ColumnType.INTEGER, allow_null=True),
             "A+B": ColumnDescriptor(ColumnType.INTEGER, allow_null=True),
         },
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "groupby_column_a", {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "groupby_column_b", {"B": ColumnDescriptor(ColumnType.INTEGER, allow_null=True)}
     )
-    catalog.add_public_source(
-        "groupby_non_existing_column", {"yay": ColumnDescriptor(ColumnType.INTEGER)}
+    catalog.add_public_table(
+        "groupby_nonexistent_column", {"yay": ColumnDescriptor(ColumnType.INTEGER)}
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "groupby_column_wrong_type", {"A": ColumnDescriptor(ColumnType.INTEGER)}
     )
-    catalog.add_private_view(
+    catalog.add_private_table(
         "groupby_one_column_private",
         {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)},
-        stability=1,
     )
     visitor = OutputSchemaVisitor(catalog)
     request.cls.visitor = visitor
 
 
 @pytest.mark.usefixtures("test_data_nulls")
 class TestValidationWithNulls:
     """Test Validation with Nulls."""
 
+    visitor: OutputSchemaVisitor
+
     @pytest.mark.parametrize(
         "query_expr,expected_error_msg", OUTPUT_SCHEMA_INVALID_QUERY_TESTS
     )
     def test_invalid_query_expr_null(
         self, query_expr: QueryExpr, expected_error_msg: str
     ) -> None:
         """Check that appropriate exceptions are raised on invalid queries."""
-        # There's one query where you need to rename all the columns,
-        # and this set of tests has a column named NOTNULL
-        # where the other doesn't.
-        # we could either copy-and-paste every single other test case,
-        # or we can fix just this one test case, right here
-        if (
-            isinstance(query_expr, JoinPrivate)
-            and expected_error_msg == "Tables have no common columns to join on."
-        ):
-            # Help whoever is debugging this, if the isinstance assertion ever fails
-            assert isinstance(query_expr.right_operand_expr, Rename)
-            # type assertion for mypy's benefit
-            # rename the NOTNULL column too
-            query_expr.right_operand_expr.column_mapper["NOTNULL"] = "ZNOTNULL"
         with pytest.raises(ValueError, match=expected_error_msg):
             query_expr.accept(self.visitor)
 
     @pytest.mark.parametrize(
         "groupby_keys,exception_type,expected_error_msg",
         [
             (
@@ -617,17 +595,17 @@
         for DataClass in [
             GroupByBoundedAverage,
             GroupByBoundedSTDEV,
             GroupByBoundedSum,
             GroupByBoundedVariance,
         ]:
             with pytest.raises(exception_type, match=expected_error_msg):
-                DataClass(  # type: ignore
-                    PrivateSource("private"), groupby_keys, "B", 1.0, 5.0
-                ).accept(self.visitor)
+                DataClass(PrivateSource("private"), groupby_keys, "B", 1.0, 5.0).accept(
+                    self.visitor
+                )
         with pytest.raises(exception_type, match=expected_error_msg):
             GroupByQuantile(
                 PrivateSource("private"), groupby_keys, "B", 0.5, 1.0, 5.0
             ).accept(self.visitor)
 
     def test_visit_private_source(self) -> None:
         """Test visit_private_source."""
@@ -711,18 +689,18 @@
         self, column_mapper: Dict[str, str], expected_schema: Schema
     ) -> None:
         """Test visit_rename."""
         query = Rename(child=PrivateSource("private"), column_mapper=column_mapper)
         schema = self.visitor.visit_rename(query)
         assert schema == expected_schema
 
-    @pytest.mark.parametrize("predicate", ["B > X", "X < 500", "NOTNULL < 30"])
-    def test_visit_filter(self, predicate: str) -> None:
+    @pytest.mark.parametrize("condition", ["B > X", "X < 500", "NOTNULL < 30"])
+    def test_visit_filter(self, condition: str) -> None:
         """Test visit_filter."""
-        query = Filter(child=PrivateSource("private"), predicate=predicate)
+        query = Filter(child=PrivateSource("private"), condition=condition)
         schema = self.visitor.visit_filter(query)
         assert (
             schema
             == self.visitor._catalog.tables[  # pylint: disable=protected-access
                 "private"
             ].schema
         )
@@ -895,19 +873,19 @@
     @pytest.mark.parametrize(
         "query,expected_schema",
         [
             (
                 FlatMap(
                     child=PrivateSource("private"),
                     f=lambda row: [{"i": i} for i in range(len(row["A"] + 1))],
-                    max_num_rows=10,
                     schema_new_columns=Schema(
                         {"i": ColumnDescriptor(ColumnType.INTEGER, allow_null=False)}
                     ),
                     augment=True,
+                    max_num_rows=10,
                 ),
                 Schema(
                     {
                         "A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True),
                         "B": ColumnDescriptor(ColumnType.INTEGER, allow_null=True),
                         "X": ColumnDescriptor(
                             ColumnType.DECIMAL,
@@ -924,19 +902,19 @@
                     }
                 ),
             ),
             (
                 FlatMap(
                     child=PrivateSource("private"),
                     f=lambda row: [{"i": i} for i in range(len(row["A"] + 1))],
-                    max_num_rows=10,
                     schema_new_columns=Schema(
                         {"i": ColumnDescriptor(ColumnType.INTEGER, allow_null=False)}
                     ),
                     augment=False,
+                    max_num_rows=10,
                 ),
                 Schema({"i": ColumnDescriptor(ColumnType.INTEGER, allow_null=True)}),
             ),
         ],
     )
     def test_visit_flat_map(self, query: FlatMap, expected_schema: Schema) -> None:
         """Test visit_flat_map."""
```

### Comparing `tmlt_analytics-0.6.1/test/unit/query_expr_compiler/test_transformation_visitor.py` & `tmlt_analytics-0.7.0rc1/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# type: ignore[attr-defined]
 """Tests for TransformationVisitor."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
-# pylint: disable=no-self-use, no-member, protected-access
+# Copyright Tumult Labs 2023
 
 import datetime
-from typing import Any, Dict, List, Mapping, Optional, Tuple, Union, cast
+from typing import Dict, List, Mapping, Optional, Tuple, Union
 
 import pandas as pd
 import pytest
+from pyspark.sql import DataFrame
 from pyspark.sql.types import LongType, StringType, StructField, StructType
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
     OutputSchemaVisitor,
 )
 from tmlt.analytics._query_expr_compiler._transformation_visitor import (
@@ -21,16 +20,17 @@
 )
 from tmlt.analytics._schema import (
     ColumnDescriptor,
     ColumnType,
     Schema,
     analytics_to_spark_columns_descriptor,
 )
+from tmlt.analytics._table_identifier import Identifier
+from tmlt.analytics._table_reference import TableReference, lookup_domain, lookup_metric
 from tmlt.analytics.keyset import KeySet
-from tmlt.analytics.query_expr import AnalyticsDefault
 from tmlt.analytics.query_expr import DropInfinity as DropInfExpr
 from tmlt.analytics.query_expr import (
     DropNullAndNan,
     Filter,
     FlatMap,
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
@@ -46,1045 +46,879 @@
     QueryExpr,
     Rename,
     ReplaceInfinity,
     ReplaceNullAndNan,
     Select,
 )
 from tmlt.analytics.truncation_strategy import TruncationStrategy
-from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
-    SparkDateColumnDescriptor,
     SparkFloatColumnDescriptor,
-    SparkIntegerColumnDescriptor,
-    SparkStringColumnDescriptor,
-    SparkTimestampColumnDescriptor,
 )
-from tmlt.core.measurements.aggregations import NoiseMechanism
-from tmlt.core.metrics import DictMetric, IfGroupedBy, SymmetricDifference
+from tmlt.core.metrics import IfGroupedBy, SymmetricDifference
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.transformations.chaining import ChainTT
-from tmlt.core.transformations.dictionary import GetValue
-from tmlt.core.transformations.spark_transformations.filter import (
-    Filter as FilterTransformation,
-)
-from tmlt.core.transformations.spark_transformations.join import (
-    PrivateJoin as PrivateJoinTransformation,
-)
-from tmlt.core.transformations.spark_transformations.join import (
-    PublicJoin as PublicJoinTransformation,
-)
-from tmlt.core.transformations.spark_transformations.join import (
-    TruncationStrategy as CoreTruncationStrategy,
-)
-from tmlt.core.transformations.spark_transformations.map import (
-    FlatMap as FlatMapTransformation,
-)
-from tmlt.core.transformations.spark_transformations.map import GroupingFlatMap
-from tmlt.core.transformations.spark_transformations.map import Map as MapTransformation
-from tmlt.core.transformations.spark_transformations.nan import (
-    DropInfs as DropInfTransformation,
-)
-from tmlt.core.transformations.spark_transformations.nan import (
-    DropNaNs,
-    DropNulls,
-    ReplaceInfs,
-    ReplaceNaNs,
-    ReplaceNulls,
-)
-from tmlt.core.transformations.spark_transformations.rename import (
-    Rename as RenameTransformation,
-)
-from tmlt.core.transformations.spark_transformations.select import (
-    Select as SelectTransformation,
-)
+from tmlt.core.transformations.dictionary import AugmentDictTransformation
+from tmlt.core.transformations.identity import Identity as IdentityTransformation
 
-from ...conftest import (  # pylint: disable=no-name-in-module
-    assert_frame_equal_with_sort,
+from .conftest import (
+    DATE1,
+    TIMESTAMP1,
+    TestTransformationVisitor,
+    TestTransformationVisitorNulls,
+    chain_to_list,
 )
 
 
-def chain_to_list(t: ChainTT) -> List[Transformation]:
-    """Turns a ChainTT's tree into a list, in order from left to right."""
-    left: List[Transformation]
-    if not isinstance(t.transformation1, ChainTT):
-        left = [t.transformation1]
-    else:
-        left = chain_to_list(t.transformation1)
-    right: List[Transformation]
-    if not isinstance(t.transformation2, ChainTT):
-        right = [t.transformation2]
-    else:
-        right = chain_to_list(t.transformation2)
-    return left + right
-
-
-@pytest.fixture(name="visitor", scope="class")
-def set_up_visitor(spark, request):
-    """Returns a TransformationVisitor for use in test functions."""
-    input_domain = DictDomain(
-        {
-            "private": SparkDataFrameDomain(
-                {
-                    "A": SparkStringColumnDescriptor(allow_null=True),
-                    "B": SparkIntegerColumnDescriptor(allow_null=True),
-                    "X": SparkFloatColumnDescriptor(
-                        allow_null=True, allow_nan=True, allow_inf=True
-                    ),
-                    "D": SparkDateColumnDescriptor(allow_null=True),
-                    "T": SparkTimestampColumnDescriptor(allow_null=True),
-                }
-            ),
-            "private_2": SparkDataFrameDomain(
-                {
-                    "A": SparkStringColumnDescriptor(allow_null=True),
-                    "C": SparkIntegerColumnDescriptor(allow_null=True),
-                }
-            ),
-        }
-    )
-    input_metric = DictMetric(
-        {"private": SymmetricDifference(), "private_2": SymmetricDifference()}
-    )
-    public_sources = {
-        "public": spark.createDataFrame(
-            pd.DataFrame({"A": ["zero", "one"], "B": [0, 1]}),
-            schema=StructType(
-                [
-                    StructField("A", StringType(), False),
-                    StructField("B", LongType(), True),
-                ]
-            ),
-        )
-    }
-    visitor = TransformationVisitor(
-        input_domain=input_domain,
-        input_metric=input_metric,
-        mechanism=NoiseMechanism.LAPLACE,
-        public_sources=public_sources,
-    )
-    request.cls.visitor = visitor
-
+class TestAddRows(TestTransformationVisitor):
+    """Tests for the transformation visitor using for AddMaxRows."""
 
-@pytest.fixture(name="catalog", scope="class")
-def set_up_catalog(request):
-    """Returns a catalog for use in test functions."""
-
-    catalog = Catalog()
-    catalog.add_private_source(
-        "private",
-        {
-            "A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True),
-            "B": ColumnDescriptor(ColumnType.INTEGER, allow_null=True),
-            "X": ColumnDescriptor(
-                ColumnType.DECIMAL, allow_null=True, allow_nan=True, allow_inf=True
-            ),
-            "D": ColumnDescriptor(ColumnType.DATE, allow_null=True),
-            "T": ColumnDescriptor(ColumnType.TIMESTAMP, allow_null=True),
-        },
-        stability=3,
-    )
-    catalog.add_private_view(
-        "private_2",
-        {
-            "A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True),
-            "C": ColumnDescriptor(ColumnType.INTEGER, allow_null=True),
-        },
-        stability=3,
-    )
-    catalog.add_public_source(
-        "public",
-        {
-            "A": ColumnDescriptor(ColumnType.VARCHAR),
-            "B": ColumnDescriptor(ColumnType.INTEGER, allow_null=True),
-        },
-    )
-    request.cls.catalog = catalog
+    visitor: TransformationVisitor
+    catalog: Catalog
+    input_data: Dict[Identifier, Union[DataFrame, Dict[Identifier, DataFrame]]]
+    dataframes: Dict[str, DataFrame]
 
-
-@pytest.mark.usefixtures("visitor", "catalog")
-class TestTransformationVisitor:
-    """Tests for Transformation Visitor."""
-
-    def _validate_transform_basics(self, t: Transformation, query: QueryExpr) -> None:
+    def _validate_transform_basics(
+        self, t: Transformation, reference: TableReference, query: QueryExpr
+    ) -> None:
         assert t.input_domain == self.visitor.input_domain
         assert t.input_metric == self.visitor.input_metric
         assert isinstance(t, ChainTT)
         first_transform = chain_to_list(t)[0]
-        assert isinstance(first_transform, GetValue)
+        assert isinstance(first_transform, IdentityTransformation)
 
         expected_schema = query.accept(OutputSchemaVisitor(self.catalog))
         expected_output_domain = SparkDataFrameDomain(
             analytics_to_spark_columns_descriptor(expected_schema)
         )
         expected_output_metric = (
             SymmetricDifference()
             if expected_schema.grouping_column is None
             else IfGroupedBy(
                 expected_schema.grouping_column, self.visitor.inner_metric()
             )
         )
-        assert t.output_domain == expected_output_domain
-        assert t.output_metric == expected_output_metric
-
-    def _assert_dict_equal_without_ordering(
-        self, d1: Mapping[Any, Any], d2: Mapping[Any, Any]
-    ) -> None:
-        """Assert that two dictionaries map the same keys to the same values.
+        assert lookup_domain(t.output_domain, reference) == expected_output_domain
+        assert lookup_metric(t.output_metric, reference) == expected_output_metric
 
-        In Python, two dictionaries are equal if they contain the same key-value
-        pairs *and* those pairs were created in the same order:
-        ``{'A': 'a1', 'B': 'b1'} != {'B': 'b1', 'A': 'a1'}``.
-        """
-        assert sorted(list(d1.keys())) == sorted(list(d2.keys()))
-        for k in list(d1.keys()):
-            assert d1[k] == d2[k]
-
-    @pytest.mark.parametrize("source_id", ["private", "private_2"])
-    def test_visit_private_source(self, source_id: "str") -> None:
+    @pytest.mark.parametrize("source_id", ["rows1", "rows2"])
+    def test_visit_private_source(self, source_id: str) -> None:
         """Test visit_private_source"""
         query = PrivateSource(source_id=source_id)
-        transformation = self.visitor.visit_private_source(query)
-        assert isinstance(transformation, GetValue)
-        assert transformation.key == source_id
-        assert transformation.input_domain == self.visitor.input_domain
-        assert transformation.input_metric == self.visitor.input_metric
-        assert transformation.output_domain == self.visitor.input_domain[source_id]
-        assert transformation.output_metric == SymmetricDifference()
+        transformation, reference, constraints = query.accept(self.visitor)
+        assert isinstance(transformation, IdentityTransformation)
+        assert isinstance(reference, TableReference)
+        assert isinstance(reference.identifier, Identifier)
+        assert lookup_domain(transformation.output_domain, reference) == lookup_domain(
+            self.visitor.input_domain, reference
+        )
+        assert (
+            lookup_metric(transformation.output_metric, reference)
+            == SymmetricDifference()
+        )
+        assert constraints == []
 
     def test_invalid_private_source(self) -> None:
         """Test visiting an invalid private source."""
         query = PrivateSource(source_id="source_that_does_not_exist")
         with pytest.raises((KeyError, ValueError)):
-            self.visitor.visit_private_source(query)
+            query.accept(self.visitor)
 
-    @pytest.mark.parametrize("mapper", [({"A": "columnA"}), ({"A": "aaaaa"})])
-    def test_visit_rename(self, mapper: Dict[str, str]) -> None:
+    @pytest.mark.parametrize(
+        "mapper,expected_df",
+        [
+            (
+                {"S": "columnS"},
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1]],
+                    columns=["columnS", "I", "F", "D", "T"],
+                ),
+            ),
+            (
+                {"D": "date", "T": "time"},
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1]],
+                    columns=["S", "I", "F", "date", "time"],
+                ),
+            ),
+        ],
+    )
+    def test_visit_rename(self, mapper: Dict[str, str], expected_df: DataFrame) -> None:
         """Test visit_rename."""
-        query = Rename(column_mapper=mapper, child=PrivateSource(source_id="private"))
-        transformation = self.visitor.visit_rename(query)
-        self._validate_transform_basics(transformation, query)
-        assert isinstance(transformation, ChainTT)
-        assert isinstance(transformation.transformation2, RenameTransformation)
-        assert transformation.transformation2.rename_mapping == mapper
+        query = Rename(column_mapper=mapper, child=PrivateSource(source_id="rows1"))
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
+        assert isinstance(transformation, ChainTT)
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
+        # check dataframe renamed as expected
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     def test_visit_invalid_rename(self) -> None:
         """Test visit_rename with an invalid query."""
         query = Rename(
             column_mapper={"column_that_does_not_exit": "asdf"},
-            child=PrivateSource(source_id="private"),
+            child=PrivateSource(source_id="rows1"),
         )
         with pytest.raises(ValueError):
-            self.visitor.visit_rename(query)
+            query.accept(self.visitor)
 
-    @pytest.mark.parametrize("filter_expr", ["B > X", "A = 'ABC'"])
-    def test_visit_filter(self, filter_expr: str) -> None:
+    @pytest.mark.parametrize(
+        "filter_expr,expected_df",
+        [
+            (
+                "F > I",
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1]],
+                    columns=["S", "I", "F", "D", "T"],
+                ),
+            ),
+            ("S = 'ABC'", pd.DataFrame(columns=["S", "I", "F", "D", "T"])),
+        ],
+    )
+    def test_visit_filter(self, filter_expr: str, expected_df: DataFrame) -> None:
         """Test visit_filter."""
-        query = Filter(predicate=filter_expr, child=PrivateSource(source_id="private"))
-        transformation = self.visitor.visit_filter(query)
-        self._validate_transform_basics(transformation, query)
-        assert isinstance(transformation, ChainTT)
-        assert isinstance(transformation.transformation2, FilterTransformation)
-        assert transformation.transformation2.filter_expr == filter_expr
+        query = Filter(condition=filter_expr, child=PrivateSource(source_id="rows1"))
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
+        assert isinstance(transformation, ChainTT)
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     def test_visit_invalid_filter(self) -> None:
         """Test visit_filter with an invalid query."""
         query = Filter(
-            predicate="not a valid predicate", child=PrivateSource(source_id="private")
+            condition="not a valid condition", child=PrivateSource(source_id="rows1")
         )
         with pytest.raises(ValueError):
-            self.visitor.visit_filter(query)
+            query.accept(self.visitor)
 
-    @pytest.mark.parametrize("columns", [(["A"]), (["A", "B", "X"])])
-    def test_visit_select(self, columns: List[str]) -> None:
+    @pytest.mark.parametrize(
+        "columns,expected_df",
+        [
+            (["S"], pd.DataFrame([["0"]], columns=["S"])),
+            (["S", "I", "F"], pd.DataFrame([["0", 0, 0.1]], columns=["S", "I", "F"])),
+        ],
+    )
+    def test_visit_select(self, columns: List[str], expected_df: DataFrame) -> None:
         """Test visit_select."""
-        query = Select(columns=columns, child=PrivateSource(source_id="private"))
-        transformation = self.visitor.visit_select(query)
-        self._validate_transform_basics(transformation, query)
-        assert isinstance(transformation, ChainTT)
-        assert isinstance(transformation.transformation2, SelectTransformation)
-        assert transformation.transformation2.columns == columns
+        query = Select(columns=columns, child=PrivateSource(source_id="rows1"))
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
+        assert isinstance(transformation, ChainTT)
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     def test_visit_invalid_select(self) -> None:
         """Test visit_select with invalid query."""
         query = Select(
             columns=["column_that_does_not_exist"],
-            child=PrivateSource(source_id="private"),
+            child=PrivateSource(source_id="rows1"),
         )
         with pytest.raises(ValueError):
-            self.visitor.visit_select(query)
+            query.accept(self.visitor)
 
     @pytest.mark.parametrize(
-        "query",
+        "query,expected_df",
         [
             (
                 Map(
-                    child=PrivateSource("private"),
-                    f=lambda row: {"C": 2 * str(row["B"])},
-                    schema_new_columns=Schema({"C": "VARCHAR"}),
+                    child=PrivateSource("rows1"),
+                    f=lambda row: {"X": 2 * str(row["S"])},
+                    schema_new_columns=Schema({"X": "VARCHAR"}),
                     augment=True,
-                )
+                ),
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1, "00"]],
+                    columns=["S", "I", "F", "D", "T", "X"],
+                ),
             ),
             (
                 Map(
-                    child=PrivateSource("private"),
-                    f=lambda row: {"C": 2 * str(row["B"])},
-                    schema_new_columns=Schema({"C": "VARCHAR"}),
+                    child=PrivateSource("rows1"),
+                    f=lambda row: {"X": 2 * str(row["S"])},
+                    schema_new_columns=Schema({"X": "VARCHAR"}),
                     augment=False,
-                )
+                ),
+                pd.DataFrame([["00"]], columns=["X"]),
             ),
         ],
     )
-    def test_visit_map(self, query: Map) -> None:
+    def test_visit_map(self, query: Map, expected_df: DataFrame) -> None:
         """Test visit_map."""
-        transformation = self.visitor.visit_map(query)
-        self._validate_transform_basics(transformation, query)
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
         assert isinstance(transformation, ChainTT)
-        assert isinstance(transformation.transformation2, MapTransformation)
-        transformer = transformation.transformation2.row_transformer
-        assert transformer.augment == query.augment
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     @pytest.mark.parametrize(
-        "query",
+        "query,expected_df",
         [
             (
                 FlatMap(
-                    child=PrivateSource("private"),
-                    f=lambda row: [{"A_is_zero": 1 if row["A"] == "zero" else 2}],
-                    max_num_rows=1,
-                    schema_new_columns=Schema({"A_is_zero": "INTEGER"}),
+                    child=PrivateSource("rows1"),
+                    f=lambda row: [{"S_is_zero": 1 if row["S"] == "0" else 2}],
+                    schema_new_columns=Schema({"S_is_zero": "INTEGER"}),
                     augment=True,
-                )
+                    max_num_rows=1,
+                ),
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1, 1]],
+                    columns=["S", "I", "F", "D", "T", "S_is_zero"],
+                ),
             ),
             (
                 FlatMap(
-                    child=PrivateSource("private"),
-                    f=lambda row: [{"i": n for n in range(row["B"] + 1)}],
+                    child=PrivateSource("rows1"),
+                    f=lambda row: [{"i": n for n in range(row["I"] + 1)}],
+                    schema_new_columns=Schema({"i": "INTEGER"}),
+                    augment=False,
                     max_num_rows=10,
-                    schema_new_columns=Schema({"i": "DECIMAL"}),
+                ),
+                pd.DataFrame([[0]], columns=["i"]),
+            ),
+            (
+                FlatMap(
+                    child=PrivateSource("rows1"),
+                    f=lambda row: [{"i": n} for n in range(row["I"] + 10)],
+                    schema_new_columns=Schema({"i": "INTEGER"}),
                     augment=False,
-                )
+                    max_num_rows=3,
+                ),
+                pd.DataFrame([[0], [1], [2]], columns=["i"]),
             ),
         ],
     )
-    def test_visit_flat_map_without_grouping(self, query: FlatMap) -> None:
+    def test_visit_flat_map_without_grouping(
+        self, query: FlatMap, expected_df: DataFrame
+    ) -> None:
         """Test visit_flat_map when query has no grouping_column."""
-        transformation = self.visitor.visit_flat_map(query)
-        self._validate_transform_basics(transformation, query)
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
         assert isinstance(transformation, ChainTT)
-        assert isinstance(transformation.transformation2, FlatMapTransformation)
-        assert isinstance(transformation.transformation2, FlatMapTransformation)
-        flat_map_transform = transformation.transformation2
-        assert flat_map_transform.max_num_rows == query.max_num_rows
-        assert flat_map_transform.row_transformer.augment == query.augment
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     @pytest.mark.parametrize(
-        "query",
+        "query,expected_df",
         [
             (
                 FlatMap(
-                    child=PrivateSource("private"),
-                    f=lambda row: [{"Group": 0 if row["X"] == 0 else 17}],
-                    max_num_rows=2,
+                    child=PrivateSource("rows1"),
+                    f=lambda row: [{"group": 0 if row["F"] == 0 else 17}],
                     schema_new_columns=Schema(
-                        {"Group": ColumnDescriptor(ColumnType.INTEGER)},
-                        grouping_column="Group",
+                        {"group": ColumnDescriptor(ColumnType.INTEGER)},
+                        grouping_column="group",
                     ),
                     augment=True,
-                )
+                    max_num_rows=2,
+                ),
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1, 17]],
+                    columns=["S", "I", "F", "D", "T", "group"],
+                ),
             )
         ],
     )
-    def test_visit_flat_map_with_grouping(self, query: FlatMap) -> None:
+    def test_visit_flat_map_with_grouping(
+        self, query: FlatMap, expected_df: DataFrame
+    ) -> None:
         """Test visit_flat_map when query has a grouping_column."""
-        transformation = self.visitor.visit_flat_map(query)
-        self._validate_transform_basics(transformation, query)
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
         assert isinstance(transformation, ChainTT)
-        assert isinstance(transformation.transformation2, GroupingFlatMap)
-        assert isinstance(transformation.transformation2, GroupingFlatMap)
-        group_map_transform = transformation.transformation2
-        assert group_map_transform.max_num_rows == query.max_num_rows
-        assert group_map_transform.row_transformer.augment == query.augment
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
+
+    def test_visit_flat_map_invalid(self) -> None:
+        """Test visit_flat_map with invalid query."""
+        query = FlatMap(
+            child=PrivateSource("rows1"),
+            f=lambda row: [{"group": 0 if row["F"] == 0 else 17}],
+            schema_new_columns=Schema(
+                {"group": ColumnDescriptor(ColumnType.INTEGER)}, grouping_column="group"
+            ),
+            augment=True,
+            max_num_rows=None,
+        )
+        with pytest.raises(
+            ValueError,
+            match=(
+                "Flat maps on tables without IDs must have"
+                " a defined max_num_rows parameter."
+            ),
+        ):
+            query.accept(self.visitor)
 
     @pytest.mark.parametrize(
-        "query,expected_left_truncation_strategy,"
-        + "expected_left_truncation_threshold,expected_right_truncation_strategy,"
-        + "expected_right_truncation_threshold,expected_join_cols",
+        "query,expected_df",
         [
             (
                 JoinPrivate(
-                    child=PrivateSource("private"),
-                    right_operand_expr=PrivateSource("private_2"),
+                    child=PrivateSource("rows1"),
+                    right_operand_expr=PrivateSource("rows2"),
                     truncation_strategy_left=TruncationStrategy.DropExcess(3),
                     truncation_strategy_right=TruncationStrategy.DropExcess(10),
                 ),
-                CoreTruncationStrategy.TRUNCATE,
-                3,
-                CoreTruncationStrategy.TRUNCATE,
-                10,
-                ["A"],
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1, "a"]],
+                    columns=["S", "I", "F", "D", "T", "field"],
+                ),
             ),
             (
                 JoinPrivate(
-                    child=PrivateSource("private_2"),
-                    right_operand_expr=PrivateSource("private"),
+                    child=PrivateSource("rows2"),
+                    right_operand_expr=PrivateSource("rows1"),
                     truncation_strategy_left=TruncationStrategy.DropExcess(3),
                     truncation_strategy_right=TruncationStrategy.DropNonUnique(),
-                    join_columns=["A"],
+                    join_columns=["I"],
+                ),
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1, "a"]],
+                    columns=["S", "I", "F", "D", "T", "field"],
                 ),
-                CoreTruncationStrategy.TRUNCATE,
-                3,
-                CoreTruncationStrategy.DROP,
-                1,
-                ["A"],
             ),
         ],
     )
     def test_visit_join_private(
-        self,
-        query: JoinPrivate,
-        expected_left_truncation_strategy: CoreTruncationStrategy,
-        expected_left_truncation_threshold: int,
-        expected_right_truncation_strategy: CoreTruncationStrategy,
-        expected_right_truncation_threshold: int,
-        expected_join_cols: List[str],
+        self, query: JoinPrivate, expected_df: DataFrame
     ) -> None:
         """Test visit_join_private."""
-        transformation = self.visitor.visit_join_private(query)
-
+        transformation, reference, constraints = query.accept(self.visitor)
         assert transformation.input_domain == self.visitor.input_domain
         assert transformation.input_metric == self.visitor.input_metric
-        assert isinstance(transformation, ChainTT)
 
         expected_schema = query.accept(OutputSchemaVisitor(self.catalog))
         expected_output_domain = SparkDataFrameDomain(
             analytics_to_spark_columns_descriptor(expected_schema)
         )
         expected_output_metric = (
             SymmetricDifference()
             if expected_schema.grouping_column is None
             else IfGroupedBy(
                 expected_schema.grouping_column, self.visitor.inner_metric()
             )
         )
-        assert transformation.output_domain == expected_output_domain
-        assert transformation.output_metric == expected_output_metric
-
-        assert isinstance(transformation, ChainTT)
-        assert isinstance(transformation.transformation2, PrivateJoinTransformation)
-        private_join_transform = cast(
-            PrivateJoinTransformation, transformation.transformation2
-        )
-        assert (
-            private_join_transform.left_truncation_strategy
-            == expected_left_truncation_strategy
-        )
-        assert (
-            private_join_transform.right_truncation_strategy
-            == expected_right_truncation_strategy
-        )
         assert (
-            private_join_transform.left_truncation_threshold
-            == expected_left_truncation_threshold
+            lookup_domain(transformation.output_domain, reference)
+            == expected_output_domain
         )
         assert (
-            private_join_transform.right_truncation_threshold
-            == expected_right_truncation_threshold
+            lookup_metric(transformation.output_metric, reference)
+            == expected_output_metric
         )
 
-        assert private_join_transform.join_cols == expected_join_cols
+        assert isinstance(transformation, ChainTT)
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     def test_visit_join_private_with_invalid_truncation_strategy(self) -> None:
         """Test visit_join_private raises an error with an invalid strategy."""
 
         class InvalidStrategy(TruncationStrategy.Type):
             """An invalid truncation strategy."""
 
         query1 = JoinPrivate(
-            child=PrivateSource(source_id="private"),
-            right_operand_expr=PrivateSource("private_2"),
+            child=PrivateSource("rows1"),
+            right_operand_expr=PrivateSource("rows2"),
             truncation_strategy_left=InvalidStrategy(),
             truncation_strategy_right=TruncationStrategy.DropExcess(3),
         )
         expected_error_msg = (
             f"Truncation strategy type {InvalidStrategy.__qualname__} is not supported."
         )
         with pytest.raises(ValueError, match=expected_error_msg):
-            self.visitor.visit_join_private(query1)
+            query1.accept(self.visitor)
 
         query2 = JoinPrivate(
-            child=PrivateSource(source_id="private"),
-            right_operand_expr=PrivateSource("private_2"),
+            child=PrivateSource("rows1"),
+            right_operand_expr=PrivateSource("rows2"),
             truncation_strategy_left=TruncationStrategy.DropExcess(2),
             truncation_strategy_right=InvalidStrategy(),
         )
         with pytest.raises(ValueError, match=expected_error_msg):
-            self.visitor.visit_join_private(query2)
+            query2.accept(self.visitor)
+
+        query3 = JoinPrivate(
+            child=PrivateSource("rows1"),
+            right_operand_expr=PrivateSource("rows2"),
+            truncation_strategy_left=None,
+            truncation_strategy_right=None,
+        )
+        with pytest.raises(
+            ValueError,
+            match="When joining without IDs, truncation strategies are required.",
+        ):
+            self.visitor.visit_join_private(query3)
 
     @pytest.mark.parametrize(
-        "source_id,join_columns", [("public", None), ("public", ["A", "B"])]
+        "source_id,join_columns,expected_df",
+        [
+            (
+                "public",
+                None,
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1, "x"]],
+                    columns=["S", "I", "F", "D", "T", "public"],
+                ),
+            ),
+            (
+                "public",
+                ["S", "I"],
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1, "x"]],
+                    columns=["S", "I", "F", "D", "T", "public"],
+                ),
+            ),
+        ],
     )
     def test_visit_join_public_str(
-        self, source_id: str, join_columns: Optional[List[str]]
+        self, source_id: str, join_columns: Optional[List[str]], expected_df: DataFrame
     ) -> None:
         """Test visit_join_public with a string identifying the public source."""
         query = JoinPublic(
-            child=PrivateSource(source_id="private"),
+            child=PrivateSource(source_id="rows1"),
             public_table=source_id,
             join_columns=join_columns,
         )
-        transformation = self.visitor.visit_join_public(query)
-        self._validate_transform_basics(transformation, query)
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
         assert isinstance(transformation, ChainTT)
-        assert isinstance(transformation.transformation2, PublicJoinTransformation)
-        public_join_transform = transformation.transformation2
-        if join_columns is not None:
-            assert public_join_transform.join_cols == join_columns
-        got_df = public_join_transform.public_df
-        assert_frame_equal_with_sort(
-            got_df.toPandas(), self.visitor.public_sources[source_id].toPandas()
-        )
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     @pytest.mark.parametrize(
-        "df,df_schema,expected_join_cols,expected_join_on_null",
+        "df,df_schema,expected_df",
         [
             (
-                pd.DataFrame({"A": ["asdf", "qwer"], "B": [0, 1]}),
+                pd.DataFrame({"S": ["asdf", "qwer"], "I": [0, 1]}),
                 StructType(
                     [
-                        StructField("A", StringType(), False),
-                        StructField("B", LongType(), False),
+                        StructField("S", StringType(), True),
+                        StructField("I", LongType(), True),
                     ]
                 ),
-                ["A", "B"],
-                False,
+                pd.DataFrame([], columns=["S", "I", "F", "D", "T"]),
             ),
             (
-                pd.DataFrame({"A": [None, "abc", "def"], "new_column": [0, 1, 2]}),
+                pd.DataFrame({"S": [None, "0", "def"], "new_column": [0, 1, 2]}),
                 StructType(
                     [
-                        StructField("A", StringType(), True),
+                        StructField("S", StringType(), True),
                         StructField("new_column", LongType(), False),
                     ]
                 ),
-                ["A"],
-                True,
+                pd.DataFrame(
+                    [["0", 0, 0.1, DATE1, TIMESTAMP1, 1]],
+                    columns=["S", "I", "F", "D", "T", "new_column"],
+                ),
             ),
         ],
     )
     def test_visit_join_public_df(
-        self,
-        spark,
-        df: pd.DataFrame,
-        df_schema: StructType,
-        expected_join_cols: List[str],
-        expected_join_on_null: bool,
+        self, spark, df: pd.DataFrame, df_schema: StructType, expected_df: DataFrame
     ) -> None:
         """Test visit_join_public with a dataframe."""
         public_df = spark.createDataFrame(df, schema=df_schema)
         query = JoinPublic(
-            child=PrivateSource(source_id="private"), public_table=public_df
+            child=PrivateSource(source_id="rows1"), public_table=public_df
         )
-        transformation = self.visitor.visit_join_public(query)
-        self._validate_transform_basics(transformation, query)
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
         assert isinstance(transformation, ChainTT)
-        assert isinstance(transformation.transformation2, PublicJoinTransformation)
-        public_join_transform = transformation.transformation2
-        assert public_join_transform.join_cols == expected_join_cols
-        got_df = public_join_transform.public_df
-        assert_frame_equal_with_sort(got_df.toPandas(), public_df.toPandas())
-        # pylint: disable=protected-access
-        assert public_join_transform._join_on_nulls == expected_join_on_null
-        # pylint: enable=protected-access
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     @pytest.mark.parametrize(
-        "replace_with,expected_replace_with,expect_nan_replacement",
+        "replace_with,expected_df",
         [
             (
                 {},
-                {
-                    "A": "",
-                    "B": 0,
-                    "X": 0.0,
-                    "D": datetime.date.fromtimestamp(0),
-                    "T": datetime.datetime.fromtimestamp(0),
-                },
-                True,
+                pd.DataFrame(
+                    [[float("inf"), "string", 0.0], [float("-inf"), "", 1.5]],
+                    columns=["inf", "null", "nan"],
+                ),
+            ),
+            (
+                {"nan": 0.0},
+                pd.DataFrame(
+                    [[float("inf"), "string", 0.0], [float("-inf"), None, 1.5]],
+                    columns=["inf", "null", "nan"],
+                ),
+            ),
+            (
+                {"null": "not null"},
+                pd.DataFrame(
+                    [
+                        [float("inf"), "string", float("nan")],
+                        [float("-inf"), "not null", 1.5],
+                    ],
+                    columns=["inf", "null", "nan"],
+                ),
             ),
-            ({"X": 0}, {"X": 0.0}, True),
-            ({"A": "replacement_str"}, {"A": "replacement_str"}, False),
         ],
     )
     def test_visit_replace_null_and_nan(
         self,
         replace_with: Mapping[
-            str, Union[int, float, str, datetime.date, datetime.datetime]
+            str, Union[int, float, str, datetime.date, datetime.datetime, float]
         ],
-        expected_replace_with: Mapping[
-            str, Union[int, float, str, datetime.date, datetime.datetime]
-        ],
-        expect_nan_replacement: bool,
+        expected_df: DataFrame,
     ):
         """Test visit_replace_null_and_nan."""
         query = ReplaceNullAndNan(
-            child=PrivateSource(source_id="private"), replace_with=replace_with
+            child=PrivateSource(source_id="rows_infs_nans"), replace_with=replace_with
         )
-        transformation = self.visitor.visit_replace_null_and_nan(query)
-        self._validate_transform_basics(transformation, query)
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
         assert isinstance(transformation, ChainTT)
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
         expected_output_schema = query.accept(OutputSchemaVisitor(self.catalog))
         expected_output_domain = SparkDataFrameDomain(
             schema=analytics_to_spark_columns_descriptor(expected_output_schema)
         )
-        transformations = chain_to_list(transformation)
-
-        replace_transform: ReplaceNulls
-        if expect_nan_replacement:
-            assert len(transformations) == 3
-            assert isinstance(transformations[1], ReplaceNulls)
-            replace_transform = transformations[1]
-
-            nan_transform = transformations[2]
-            assert isinstance(nan_transform, ReplaceNaNs)
-            expected_nan_replace = {
-                k: v
-                for k, v in expected_replace_with.items()
-                if expected_output_schema[k].column_type == ColumnType.DECIMAL
-            }
-            self._assert_dict_equal_without_ordering(
-                expected_nan_replace, nan_transform.replace_map
-            )
-        else:
-            assert len(transformations) == 2
-            assert isinstance(transformations[1], ReplaceNulls)
-            replace_transform = transformations[1]
-
         expected_output_schema = query.accept(OutputSchemaVisitor(self.catalog))
         expected_output_domain = SparkDataFrameDomain(
             schema=analytics_to_spark_columns_descriptor(expected_output_schema)
         )
-        assert expected_output_domain == transformation.output_domain
-        self._assert_dict_equal_without_ordering(
-            expected_replace_with, replace_transform.replace_map
+        assert expected_output_domain == lookup_domain(
+            transformation.output_domain, reference
         )
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     def test_visit_replace_null_and_nan_with_grouping_column(self) -> None:
         """Test behavior of visit_replace_null_and_nan with IfGroupedBy metric."""
         flatmap_query = FlatMap(
-            child=PrivateSource("private"),
-            f=lambda row: [{"Group": 0 if row["X"] == 0 else 17}],
-            max_num_rows=2,
+            child=PrivateSource("rows_infs_nans"),
+            f=lambda row: [{"group": 0 if row["inf"] < 0 else 17}],
             schema_new_columns=Schema(
-                {"Group": ColumnDescriptor(ColumnType.INTEGER, allow_null=True)},
-                grouping_column="Group",
+                {"group": ColumnDescriptor(ColumnType.INTEGER, allow_null=True)},
+                grouping_column="group",
             ),
             augment=True,
+            max_num_rows=2,
         )
         with pytest.raises(
             ValueError,
             match=(
-                "Cannot replace null values in column Group, because it is being used"
+                "Cannot replace null values in column group, because it is being used"
                 " as a grouping column"
             ),
         ):
             invalid_replace_query = ReplaceNullAndNan(
-                child=flatmap_query, replace_with={"Group": -10}
+                child=flatmap_query, replace_with={"group": -10}
             )
-            self.visitor.visit_replace_null_and_nan(invalid_replace_query)
+            invalid_replace_query.accept(self.visitor)
+
         valid_replace_query = ReplaceNullAndNan(child=flatmap_query, replace_with={})
-        expected_replace_with = {
-            "A": "",
-            "B": 0,
-            "X": 0.0,
-            "D": datetime.date.fromtimestamp(0),
-            "T": datetime.datetime.fromtimestamp(0),
-        }
-        transformation = self.visitor.visit_replace_null_and_nan(valid_replace_query)
-        self._validate_transform_basics(transformation, valid_replace_query)
+        transformation, reference, constraints = valid_replace_query.accept(
+            self.visitor
+        )
+        self._validate_transform_basics(transformation, reference, valid_replace_query)
         assert isinstance(transformation, ChainTT)
         transformations = chain_to_list(transformation)
-        assert isinstance(transformations[0], GetValue)
-        assert isinstance(transformations[1], GroupingFlatMap)
-        assert isinstance(transformations[2], ReplaceNulls)
-        replace_nulls = transformations[2]
-        self._assert_dict_equal_without_ordering(
-            replace_nulls.replace_map, expected_replace_with
-        )
-        expected_replace_nan = {"X": 0.0}
-        assert len(transformations) == 4
-        assert isinstance(transformations[3], ReplaceNaNs)
-        replace_nans = transformations[3]
-        assert replace_nans.replace_map == expected_replace_nan
+        assert isinstance(transformations[0], IdentityTransformation)
+        assert isinstance(transformations[1], AugmentDictTransformation)
+        assert isinstance(transformations[2], AugmentDictTransformation)
+        expected_df = pd.DataFrame(
+            [[float("inf"), "string", 0, 17], [float("-inf"), "", 1.5, 0]],
+            columns=["inf", "null", "nan", "group"],
+        )
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     @pytest.mark.parametrize(
-        "replace_with,expected_replace_with",
+        "replace_with,expected_df",
         [
-            ({}, {"X": (AnalyticsDefault.DECIMAL, AnalyticsDefault.DECIMAL)}),
-            ({"X": (-100.0, 100.0)}, {"X": (-100.0, 100.0)}),
+            (
+                {},
+                pd.DataFrame(
+                    [[0.0, "string", float("nan")], [0.0, None, 1.5]],
+                    columns=["inf", "null", "nan"],
+                ),
+            ),
+            (
+                {"inf": (-100.0, 100.0)},
+                pd.DataFrame(
+                    [[100.0, "string", float("nan")], [-100.0, None, 1.5]],
+                    columns=["inf", "null", "nan"],
+                ),
+            ),
         ],
     )
     def test_visit_replace_infinity(
-        self,
-        replace_with: Dict[str, Tuple[float, float]],
-        expected_replace_with: Dict[str, Tuple[float, float]],
+        self, replace_with: Dict[str, Tuple[float, float]], expected_df: DataFrame
     ):
         """Test visit_replace_infinity."""
         query = ReplaceInfinity(
-            child=PrivateSource(source_id="private"), replace_with=replace_with
+            child=PrivateSource(source_id="rows_infs_nans"), replace_with=replace_with
         )
-        transformation = self.visitor.visit_replace_infinity(query)
-        self._validate_transform_basics(transformation, query)
-        assert isinstance(transformation, ChainTT)
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
+
         expected_output_schema = query.accept(OutputSchemaVisitor(self.catalog))
         expected_output_domain = SparkDataFrameDomain(
             schema=analytics_to_spark_columns_descriptor(expected_output_schema)
         )
-        assert isinstance(transformation.transformation2, ReplaceInfs)
-        replace_transform = transformation.transformation2
-
-        assert expected_output_domain == replace_transform.output_domain
-        self._assert_dict_equal_without_ordering(
-            expected_replace_with, replace_transform.replace_map
+        assert (
+            lookup_domain(transformation.output_domain, reference)
+            == expected_output_domain
         )
 
+        assert isinstance(transformation, ChainTT)
+        assert isinstance(transformation.transformation2, AugmentDictTransformation)
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
+
     def test_visit_drop_null_and_nan_with_grouping_column(self) -> None:
         """Test behavior of visit_drop_null_and_nan with IfGroupedBy metric."""
         flatmap_query = FlatMap(
-            child=PrivateSource("private"),
-            f=lambda row: [{"Group": 0 if row["X"] == 0 else 17}],
-            max_num_rows=2,
+            child=PrivateSource("rows_infs_nans"),
+            f=lambda row: [{"group": 0 if row["inf"] < 0 else 17}],
             schema_new_columns=Schema(
-                {"Group": ColumnDescriptor(ColumnType.INTEGER, allow_null=True)},
-                grouping_column="Group",
+                {"group": ColumnDescriptor(ColumnType.INTEGER, allow_null=True)},
+                grouping_column="group",
             ),
             augment=True,
+            max_num_rows=2,
         )
         with pytest.raises(
             ValueError,
             match=(
-                "Cannot drop null values in column Group, because it is being used as a"
+                "Cannot drop null values in column group, because it is being used as a"
                 " grouping column"
             ),
         ):
-            invalid_drop_query = DropNullAndNan(child=flatmap_query, columns=["Group"])
-            self.visitor.visit_drop_null_and_nan(invalid_drop_query)
+            invalid_drop_query = DropNullAndNan(child=flatmap_query, columns=["group"])
+            invalid_drop_query.accept(self.visitor)
         valid_drop_query = DropNullAndNan(child=flatmap_query, columns=[])
-        expected_columns = ["A", "B", "X", "D", "T"]
-        t = self.visitor.visit_drop_null_and_nan(valid_drop_query)
-        self._validate_transform_basics(t, valid_drop_query)
-        assert isinstance(t, ChainTT)
-        transformations = chain_to_list(t)
-        assert isinstance(transformations[0], GetValue)
-        assert isinstance(transformations[1], GroupingFlatMap)
-        assert isinstance(transformations[2], DropNulls)
-        assert sorted(set(transformations[2].columns)) == sorted(set(expected_columns))
+        transformation, reference, constraints = valid_drop_query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, valid_drop_query)
+        assert isinstance(transformation, ChainTT)
+        transformations = chain_to_list(transformation)
+        assert len(transformations) == 3
+        assert isinstance(transformations[0], IdentityTransformation)
+        assert isinstance(transformations[1], AugmentDictTransformation)
+        assert isinstance(transformations[2], AugmentDictTransformation)
+        ###expect group col added, row dropped
+        expected_df = pd.DataFrame(columns=["inf", "null", "nan", "group"])
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     def test_visit_drop_infinity_with_grouping_column(self) -> None:
         """Test behavior of visit_drop_infinity with IfGroupedBy metric."""
         flatmap_query = FlatMap(
-            child=PrivateSource("private"),
-            f=lambda row: [{"Group": 0 if row["X"] == 0 else 17}],
-            max_num_rows=2,
+            child=PrivateSource("rows_infs_nans"),
+            f=lambda row: [{"group": 0 if row["inf"] < 0 else 17}],
             schema_new_columns=Schema(
-                {"Group": ColumnDescriptor(ColumnType.INTEGER, allow_null=True)},
-                grouping_column="Group",
+                {"group": ColumnDescriptor(ColumnType.INTEGER, allow_null=True)},
+                grouping_column="group",
             ),
             augment=True,
+            max_num_rows=2,
         )
         with pytest.raises(
             ValueError,
             match=(
-                "Cannot drop infinite values in column Group, because it is being used"
+                "Cannot drop infinite values in column group, because it is being used"
                 " as a grouping column"
             ),
         ):
-            invalid_drop_query = DropInfExpr(child=flatmap_query, columns=["Group"])
-            self.visitor.visit_drop_infinity(invalid_drop_query)
+            invalid_drop_query = DropInfExpr(child=flatmap_query, columns=["group"])
+            invalid_drop_query.accept(self.visitor)
         valid_drop_query = DropInfExpr(child=flatmap_query, columns=[])
-        expected_columns = ["X"]
-        t = self.visitor.visit_drop_infinity(valid_drop_query)
-        self._validate_transform_basics(t, valid_drop_query)
-        assert isinstance(t, ChainTT)
-        transformations = chain_to_list(t)
-        assert isinstance(transformations[0], GetValue)
-        assert isinstance(transformations[1], GroupingFlatMap)
-        assert isinstance(transformations[2], DropInfTransformation)
-        assert sorted(set(transformations[2].columns)) == sorted(set(expected_columns))
+        transformation, reference, constraints = valid_drop_query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, valid_drop_query)
+        assert isinstance(transformation, ChainTT)
+        transformations = chain_to_list(transformation)
+        assert isinstance(transformations[0], IdentityTransformation)
+        assert isinstance(transformations[1], AugmentDictTransformation)
+        assert isinstance(transformations[2], AugmentDictTransformation)
+        expected_df = pd.DataFrame(columns=["inf", "null", "nan", "group"])
+
+        self._validate_result(transformation, reference, expected_df)
+        assert constraints == []
 
     def test_measurement_visits(self):
         """Test that visiting measurement queries raises an error."""
         with pytest.raises(NotImplementedError):
             self.visitor.visit_groupby_count(
                 GroupByCount(
                     groupby_keys=KeySet.from_dict({}),
-                    child=PrivateSource(source_id="private"),
+                    child=PrivateSource(source_id="rows1"),
                 )
             )
 
         with pytest.raises(NotImplementedError):
             self.visitor.visit_groupby_count_distinct(
                 GroupByCountDistinct(
                     groupby_keys=KeySet.from_dict({}),
-                    child=PrivateSource(source_id="private"),
+                    child=PrivateSource(source_id="rows1"),
                 )
             )
 
         with pytest.raises(NotImplementedError):
             self.visitor.visit_groupby_quantile(
                 GroupByQuantile(
-                    child=PrivateSource(source_id="private"),
+                    child=PrivateSource(source_id="rows1"),
                     groupby_keys=KeySet.from_dict({}),
                     measure_column="A",
                     quantile=0.1,
                     low=0,
                     high=1,
                 )
             )
 
         with pytest.raises(NotImplementedError):
             self.visitor.visit_groupby_bounded_sum(
                 GroupByBoundedSum(
-                    child=PrivateSource(source_id="private"),
+                    child=PrivateSource(source_id="rows1"),
                     groupby_keys=KeySet.from_dict({}),
                     measure_column="A",
                     low=0,
                     high=1,
                 )
             )
 
         with pytest.raises(NotImplementedError):
             self.visitor.visit_groupby_bounded_average(
                 GroupByBoundedAverage(
-                    child=PrivateSource(source_id="private"),
+                    child=PrivateSource(source_id="rows1"),
                     groupby_keys=KeySet.from_dict({}),
                     measure_column="A",
                     low=0,
                     high=1,
                 )
             )
 
         with pytest.raises(NotImplementedError):
             self.visitor.visit_groupby_bounded_variance(
                 GroupByBoundedVariance(
-                    child=PrivateSource(source_id="private"),
+                    child=PrivateSource(source_id="rows1"),
                     groupby_keys=KeySet.from_dict({}),
                     measure_column="A",
                     low=0,
                     high=1,
                 )
             )
 
         with pytest.raises(NotImplementedError):
             self.visitor.visit_groupby_bounded_stdev(
                 GroupByBoundedSTDEV(
-                    child=PrivateSource(source_id="private"),
+                    child=PrivateSource(source_id="rows1"),
                     groupby_keys=KeySet.from_dict({}),
                     measure_column="A",
                     low=0,
                     high=1,
                 )
             )
 
 
-@pytest.fixture(name="complex_visitor", scope="class")
-def set_up_complex_visitor(request) -> None:
-    """Set up complex visitor for use in following tests."""
-    input_domain = DictDomain(
-        {
-            "private": SparkDataFrameDomain(
-                {
-                    "A": SparkStringColumnDescriptor(allow_null=True),
-                    "B": SparkIntegerColumnDescriptor(allow_null=True),
-                    "NOTNULL": SparkFloatColumnDescriptor(allow_null=False),
-                    "null": SparkFloatColumnDescriptor(allow_null=True),
-                    "nan": SparkFloatColumnDescriptor(allow_nan=True),
-                    "inf": SparkFloatColumnDescriptor(allow_inf=True),
-                    "null_and_nan": SparkFloatColumnDescriptor(
-                        allow_null=True, allow_nan=True
-                    ),
-                    "null_and_inf": SparkFloatColumnDescriptor(
-                        allow_null=True, allow_inf=True
-                    ),
-                    "nan_and_inf": SparkFloatColumnDescriptor(
-                        allow_nan=True, allow_inf=True
-                    ),
-                    "null_and_nan_and_inf": SparkFloatColumnDescriptor(
-                        allow_null=True, allow_nan=True, allow_inf=True
-                    ),
-                    "D": SparkDateColumnDescriptor(allow_null=True),
-                    "T": SparkTimestampColumnDescriptor(allow_null=True),
-                }
-            )
-        }
-    )
-    input_metric = DictMetric({"private": SymmetricDifference()})
-    visitor = TransformationVisitor(
-        input_domain=input_domain,
-        input_metric=input_metric,
-        mechanism=NoiseMechanism.LAPLACE,
-        public_sources={},
-    )
-    request.cls.visitor = visitor
+class TestAddRowsNulls(TestTransformationVisitorNulls):
+    """Test the TransformationVisitor with nulls, NaNs, and infs."""
 
+    visitor: TransformationVisitor
+    catalog: Catalog
 
-@pytest.fixture(name="complex_catalog", scope="class")
-def set_up_complex_catalog(request):
-    """Set up complex catalog for following tests."""
-    catalog = Catalog()
-    catalog.add_private_source(
-        "private",
-        {
-            "A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True),
-            "B": ColumnDescriptor(ColumnType.INTEGER, allow_null=True),
-            "NOTNULL": ColumnDescriptor(ColumnType.DECIMAL, allow_null=False),
-            "null": ColumnDescriptor(ColumnType.DECIMAL, allow_null=True),
-            "nan": ColumnDescriptor(ColumnType.DECIMAL, allow_nan=True),
-            "inf": ColumnDescriptor(ColumnType.DECIMAL, allow_inf=True),
-            "null_and_nan": ColumnDescriptor(
-                ColumnType.DECIMAL, allow_null=True, allow_nan=True
-            ),
-            "null_and_inf": ColumnDescriptor(
-                ColumnType.DECIMAL, allow_null=True, allow_inf=True
-            ),
-            "nan_and_inf": ColumnDescriptor(
-                ColumnType.DECIMAL, allow_nan=True, allow_inf=True
-            ),
-            "null_and_nan_and_inf": ColumnDescriptor(
-                ColumnType.DECIMAL, allow_null=True, allow_nan=True, allow_inf=True
-            ),
-            "D": ColumnDescriptor(ColumnType.DATE, allow_null=True),
-            "T": ColumnDescriptor(ColumnType.TIMESTAMP, allow_null=True),
-        },
-        stability=3,
-    )
-    request.cls.catalog = catalog
-
-
-@pytest.mark.usefixtures("complex_visitor", "complex_catalog")
-class TestTransformationVisitorWithComplexSchema:
-    """Test the TransformationVisitor with a complicated schema."""
-
-    def _validate_transform_basics(self, t: Transformation, query: QueryExpr) -> None:
+    def _validate_transform_basics(
+        self, t: Transformation, reference: TableReference, query: QueryExpr
+    ) -> None:
         """Check the basics of a transformation."""
         assert t.input_domain == self.visitor.input_domain
         assert t.input_metric == self.visitor.input_metric
-        first_transform: Transformation
-        if isinstance(t, ChainTT):
-            first_transform = chain_to_list(t)[0]
-        else:
-            first_transform = t
-        assert isinstance(first_transform, GetValue)
 
         expected_schema = query.accept(OutputSchemaVisitor(self.catalog))
         expected_output_domain = SparkDataFrameDomain(
             analytics_to_spark_columns_descriptor(expected_schema)
         )
         expected_output_metric = (
             SymmetricDifference()
             if expected_schema.grouping_column is None
             else IfGroupedBy(
                 expected_schema.grouping_column, self.visitor.inner_metric()
             )
         )
-        assert t.output_domain == expected_output_domain
-        assert t.output_metric == expected_output_metric
+        assert lookup_domain(t.output_domain, reference) == expected_output_domain
+        assert lookup_metric(t.output_metric, reference) == expected_output_metric
 
     @pytest.mark.parametrize(
         "query_columns,expected_null_cols,expected_nan_cols",
         [
-            (["A"], ["A"], []),
-            (["A", "B", "D", "T"], ["A", "B", "D", "T"], []),
-            (["NOTNULL"], [], []),
-            (["null", "nan", "inf"], ["null"], ["nan"]),
-            (
-                ["null_and_nan", "null_and_inf", "nan_and_inf"],
-                ["null_and_nan", "null_and_inf"],
-                ["null_and_nan", "nan_and_inf"],
-            ),
-            (
-                ["null", "nan", "inf", "null_and_nan_and_inf"],
-                ["null", "null_and_nan_and_inf"],
-                ["nan", "null_and_nan_and_inf"],
-            ),
-            (
-                [],
-                [
-                    "A",
-                    "B",
-                    "null",
-                    "null_and_nan",
-                    "null_and_inf",
-                    "null_and_nan_and_inf",
-                    "D",
-                    "T",
-                ],
-                ["nan", "null_and_nan", "nan_and_inf", "null_and_nan_and_inf"],
+            (
+                ["not_null"],
+                ["null", "null_nan", "null_inf", "null_nan_inf"],
+                ["nan", "null_nan", "nan_inf", "null_nan_inf"],
+            ),
+            (
+                ["null", "nan", "inf"],
+                ["null_nan", "null_inf", "null_nan_inf"],
+                ["null_nan", "nan_inf", "null_nan_inf"],
             ),
+            (
+                ["null_nan", "null_inf", "nan_inf"],
+                ["null", "null_nan_inf"],
+                ["nan", "null_nan_inf"],
+            ),
+            (
+                ["null", "nan", "inf", "null_nan_inf"],
+                ["null_nan", "null_inf"],
+                ["null_nan", "nan_inf"],
+            ),
+            ([], [], []),
         ],
     )
     def test_visit_drop_null_and_nan(
         self,
         query_columns: List[str],
         expected_null_cols: List[str],
         expected_nan_cols: List[str],
     ) -> None:
-        """Test visit_drop_invalid."""
-        query = DropNullAndNan(child=PrivateSource("private"), columns=query_columns)
-        transform = self.visitor.visit_drop_null_and_nan(query)
-        self._validate_transform_basics(transform, query)
-        if not expected_null_cols and not expected_nan_cols:
-            # There should just be a GetValue transformation
-            assert isinstance(transform, GetValue)
-            # nothing else to test!
-            return
-        assert isinstance(transform, ChainTT)
-        transformations = chain_to_list(transform)
-        # Pop the get_value transformation off the front of the list
-        # (_validate_transform_basics checks that the first transformation
-        # is a GetValue transformation)
-        transformations.pop(0)
-
-        # We expect transformations to happen in this order:
-        # DropNulls -> DropNaNs
-        # but each one will only be present if it makes sense
-        if expected_null_cols:
-            null_transform = transformations.pop(0)
-            assert isinstance(null_transform, DropNulls)
-            assert sorted(null_transform.columns) == sorted(expected_null_cols)
-        if expected_nan_cols:
-            nan_transform = transformations.pop(0)
-            assert isinstance(nan_transform, DropNaNs)
-            assert sorted(nan_transform.columns) == sorted(expected_nan_cols)
+        """Test generating transformations from a DropNullAndNan."""
+        query = DropNullAndNan(PrivateSource("rows"), query_columns)
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
+        assert constraints == []
+
+        output_domain = lookup_domain(transformation.output_domain, reference)
+        assert isinstance(output_domain, SparkDataFrameDomain)
+
+        for col in output_domain.schema:
+            col_descriptor = output_domain.schema[col]
+            assert col_descriptor.allow_null == (col in expected_null_cols)
+            if isinstance(col_descriptor, SparkFloatColumnDescriptor):
+                assert col_descriptor.allow_nan == (col in expected_nan_cols)
 
     @pytest.mark.parametrize(
         "query_columns,expected_inf_cols",
         [
-            (["inf"], ["inf"]),
-            (["null", "nan", "inf"], ["null", "nan", "inf"]),
-            (
-                ["null_and_nan", "null_and_inf", "nan_and_inf"],
-                ["null_and_nan", "null_and_inf", "nan_and_inf"],
-            ),
-            (
-                ["null", "nan", "inf", "null_and_nan_and_inf"],
-                ["null", "nan", "inf", "null_and_nan_and_inf"],
-            ),
-            ([], ["inf", "null_and_inf", "nan_and_inf", "null_and_nan_and_inf"]),
+            (["not_null"], ["inf", "null_inf", "nan_inf", "null_nan_inf"]),
+            (["null", "nan", "inf"], ["null_inf", "nan_inf", "null_nan_inf"]),
+            (["null_nan", "null_inf", "nan_inf"], ["inf", "null_nan_inf"]),
+            (["null", "nan", "inf", "null_nan_inf"], ["null_inf", "nan_inf"]),
         ],
     )
     def test_visit_drop_infinity(
         self, query_columns: List[str], expected_inf_cols: List[str]
     ) -> None:
-        """Test visit_drop_infinity."""
-        query = DropInfExpr(child=PrivateSource("private"), columns=query_columns)
-        transform = self.visitor.visit_drop_infinity(query)
-        self._validate_transform_basics(transform, query)
-        assert isinstance(transform, ChainTT)
-        transformations = chain_to_list(transform)
-        # Pop the get_value transformation off the front of the list
-        # (_validate_transform_basics checks that the first transformation
-        # is a GetValue transformation)
-        transformations.pop(0)
-
-        inf_transform = transformations.pop(0)
-        assert isinstance(inf_transform, DropInfTransformation)
-        assert sorted(inf_transform.columns) == sorted(expected_inf_cols)
+        """Test generating transformations from a DropInfinity."""
+        query = DropInfExpr(child=PrivateSource("rows"), columns=query_columns)
+        transformation, reference, constraints = query.accept(self.visitor)
+        self._validate_transform_basics(transformation, reference, query)
+        assert constraints == []
+
+        output_domain = lookup_domain(transformation.output_domain, reference)
+        assert isinstance(output_domain, SparkDataFrameDomain)
+
+        for col in output_domain.schema:
+            col_descriptor = output_domain.schema[col]
+            if isinstance(col_descriptor, SparkFloatColumnDescriptor):
+                assert col_descriptor.allow_inf == (col in expected_inf_cols)
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_binning_spec.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_binning_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for BinningSpec."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # pylint: disable=pointless-string-statement
 
 import datetime
 from typing import Any, List
 
 import pytest
 
@@ -224,15 +224,14 @@
     assert spec.bins(include_null=True) == ["high", "low", None]
     assert spec.column_descriptor.column_type == ColumnType.VARCHAR
     bin_tests = {-16: None, -15: "high", -5: "high", -4: "low", 4: "low", 10: "high"}
     for val, expected_bin in bin_tests.items():
         assert spec(val) == expected_bin
 
 
-# TODO Binning: add tests somwhere around here
 def test_binning_inf_nan() -> None:
     """Binning infinite/NaN values works as expected."""
     spec = BinningSpec(
         [float("-inf"), 0.0, float("inf")],
         right=False,
         names=["negative", "nonnegative"],
     )
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_cleanup.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/test/unit/test_keyset.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_keyset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for KeySet."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # pylint: disable=no-self-use
 
 
 import datetime
 from typing import Dict, List, Mapping, Optional, Union
 
 import pandas as pd
@@ -302,15 +302,15 @@
     """KeySet.from_dataframe raises an appropriate exception on invalid inputs."""
     sdf = spark.createDataFrame(df)
     with pytest.raises(ValueError, match=expected_err_msg):
         KeySet.from_dataframe(sdf)
 
 
 @pytest.mark.parametrize(
-    "keyset_df,expr,expected_df",
+    "keyset_df,condition,expected_df",
     [
         (
             pd.DataFrame([[0, "b0"], [1, "b0"], [2, "b0"]], columns=["A", "B"]),
             "A > 0",
             pd.DataFrame([[1, "b0"], [2, "b0"]], columns=["A", "B"]),
         ),
         (
@@ -322,19 +322,22 @@
             pd.DataFrame({"A": ["a0", "a1", "a123456"]}),
             "length(A) > 3",
             pd.DataFrame({"A": ["a123456"]}),
         ),
     ],
 )
 def test_filter_str(
-    spark, keyset_df: pd.DataFrame, expr: Union[Column, str], expected_df: pd.DataFrame
+    spark,
+    keyset_df: pd.DataFrame,
+    condition: Union[Column, str],
+    expected_df: pd.DataFrame,
 ) -> None:
     """Test KeySet.filter works"""
     keyset = KeySet(spark.createDataFrame(keyset_df))
-    filtered_keyset = keyset.filter(expr)
+    filtered_keyset = keyset.filter(condition)
     assert_frame_equal_with_sort(filtered_keyset.dataframe().toPandas(), expected_df)
 
 
 @pytest.mark.parametrize(
     "df_in,input_schema,expected_schema",
     [
         (
@@ -401,31 +404,31 @@
     df_out = keyset.dataframe()
     for col in df_out.schema:
         assert col.dataType == expected_schema[col.name]
 
 
 # This test is not parameterized because Column parameters are
 # Python expressions containing the KeySet's DataFrame.
-def test_filter_expr() -> None:
-    """Test KeySet.filter with Columns expressions."""
+def test_filter_condition() -> None:
+    """Test KeySet.filter with Columns conditions."""
     keyset = KeySet.from_dict({"A": ["abc", "def", "ghi"], "B": [0, 100]})
     filtered = keyset.filter(keyset.dataframe().B > 0)
     expected = pd.DataFrame(
         [["abc", 100], ["def", 100], ["ghi", 100]], columns=["A", "B"]
     )
     assert_frame_equal_with_sort(filtered.dataframe().toPandas(), expected)
 
     filtered2 = keyset.filter(keyset.dataframe().A != "string that is not there")
     assert_frame_equal_with_sort(
         filtered2.dataframe().toPandas(), keyset.dataframe().toPandas()
     )
 
 
-# This test also uses a Column as a filter expression, and is not
-# parameterized for the same reason as test_filter_expr.
+# This test also uses a Column as a filter condition, and is not
+# parameterized for the same reason as test_filter_condition.
 def test_filter_to_empty() -> None:
     """Test when KeySet.filter should return an empty dataframe, it does"""
     keyset = KeySet.from_dict({"A": [-1, -2, -3]})
     filtered = keyset.filter("A > 0")
     pd_df = filtered.dataframe().toPandas()
     assert isinstance(pd_df, pd.DataFrame)
     assert pd_df.empty
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_noise_info.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_noise_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for noise info."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 from typing import Dict
 
 import pytest
 import sympy as sp
 
 from tmlt.analytics._noise_info import (
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_privacy_budget_rounding_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for :mod:`tmlt.analytics._privacy_budget_rounding_helper`."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # pylint: disable=pointless-string-statement
 
 
 from typeguard import typechecked
 
 from tmlt.analytics._privacy_budget_rounding_helper import (
     BUDGET_RELATIVE_TOLERANCE,
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_protected_change.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_protected_change.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Tests for :mod:`tmlt.analytics.protected_change`."""
 
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # SPDX-License-Identifier: Apache-2.0
 
 from contextlib import nullcontext as does_not_raise
 from typing import Any, ContextManager, List
 
 import pytest
 
-from tmlt.analytics.protected_change import AddMaxRows, AddMaxRowsInMaxGroups, AddOneRow
+from tmlt.analytics.protected_change import (
+    AddMaxRows,
+    AddMaxRowsInMaxGroups,
+    AddOneRow,
+    AddRowsWithID,
+)
 
 
 def test_add_one_row():
     """For AddOneRow, max_rows = 1."""
     assert isinstance(AddOneRow(), AddMaxRows)
     assert AddOneRow().max_rows == 1
 
@@ -74,7 +79,30 @@
 )
 def test_add_max_rows_per_group_invalid(
     args: List[Any], expectation: ContextManager[None]
 ):
     """Invalid inputs are rejected by AddMaxRowsInMaxGroups."""
     with expectation:
         AddMaxRowsInMaxGroups(*args)
+
+
+@pytest.mark.parametrize(
+    "args,expectation",
+    [
+        (["x"], does_not_raise()),
+        (["y"], does_not_raise()),
+        (
+            [1],
+            pytest.raises(
+                TypeError, match="^type of id_column must be str; got int instead$"
+            ),
+        ),
+        (["x", "x_space"], does_not_raise()),
+        (["x", ""], pytest.raises(ValueError, match="identifier must be non-empty")),
+    ],
+)
+def test_add_rows_with_id_invalid(
+    args: List[Any], expectation: ContextManager[None]
+) -> None:
+    """Invalid arguments are rejected by AddRowsWithID."""
+    with expectation:
+        AddRowsWithID(*args)
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_query_builder.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_query_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for :mod:`~tmlt.analytics.query_builder`."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # pylint: disable=no-self-use
 import datetime
 import re
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 import pandas as pd
 import pytest
@@ -40,14 +40,16 @@
 from tmlt.analytics.truncation_strategy import TruncationStrategy
 
 from ..conftest import assert_frame_equal_with_sort  # pylint: disable=no-name-in-module
 
 PRIVATE_ID = "private"
 
 Row = Dict[str, Any]
+
+
 ###DEFINE ROOT BUILDER###
 def root_builder():
     """Set up QueryBuilder."""
     root_built = QueryBuilder(PRIVATE_ID)
     return root_built
 
 
@@ -59,15 +61,15 @@
     query = (
         root_builder()
         .join_public(join_table, join_columns)
         .groupby(KeySet.from_dict({"A + B": ["0", "1", "2"]}))
         .count()
     )
 
-    assert query.child.join_columns == join_columns  # type: ignore
+    assert query.child.join_columns == join_columns
 
     # Check query expression
     assert isinstance(query, GroupByCount)
 
     join_expr = query.child
     assert isinstance(join_expr, JoinPublic)
     assert join_expr.public_table == join_table
@@ -85,15 +87,15 @@
     query = (
         root_builder()
         .join_public(join_table, join_columns)
         .groupby(KeySet.from_dict({"A + B": ["0", "1", "2"]}))
         .count()
     )
 
-    assert query.child.join_columns == join_columns  # type: ignore
+    assert query.child.join_columns == join_columns
 
     # Check query expression
     assert isinstance(query, GroupByCount)
 
     join_expr = query.child
     assert isinstance(join_expr, JoinPublic)
     assert isinstance(join_expr.public_table, DataFrame)
@@ -133,14 +135,45 @@
     right_operand_expr = private_join_expr.right_operand_expr
     assert isinstance(right_operand_expr, PrivateSource)
     assert right_operand_expr.source_id == "private_2"
 
     assert isinstance(query, GroupByCount)
 
 
+def test_join_private_str() -> None:
+    """Test join_private("table_name") works as expected."""
+    query = (
+        root_builder()
+        .join_private(
+            right_operand="private_2",
+            truncation_strategy_left=TruncationStrategy.DropExcess(1),
+            truncation_strategy_right=TruncationStrategy.DropExcess(2),
+            join_columns=None,
+        )
+        .groupby(KeySet.from_dict({"A": ["1", "2"]}))
+        .count()
+    )
+
+    assert isinstance(query, GroupByCount)
+    private_join_expr = query.child
+    assert isinstance(private_join_expr, JoinPrivate)
+    assert private_join_expr.join_columns is None
+    assert private_join_expr.truncation_strategy_left == TruncationStrategy.DropExcess(
+        1
+    )
+    assert private_join_expr.truncation_strategy_right == TruncationStrategy.DropExcess(
+        2
+    )
+    right_operand_expr = private_join_expr.right_operand_expr
+    assert isinstance(right_operand_expr, PrivateSource)
+    assert right_operand_expr.source_id == "private_2"
+
+    assert isinstance(query, GroupByCount)
+
+
 def test_rename():
     """QueryBuilder rename works as expected."""
     column_mapper = {"A": "Z"}
     query = (
         root_builder()
         .rename(column_mapper)
         .groupby(KeySet.from_dict({"Z": ["1", "2"]}))
@@ -157,23 +190,23 @@
     root_expr = rename_expr.child
     assert isinstance(root_expr, PrivateSource)
     assert root_expr.source_id == PRIVATE_ID
 
 
 def test_filter():
     """QueryBuilder filter works as expected."""
-    predicate = "A == '0'"
-    query = root_builder().filter(predicate).count()
+    condition = "A == '0'"
+    query = root_builder().filter(condition).count()
 
     # Check query expression
     assert isinstance(query, GroupByCount)
 
     filter_expr = query.child
     assert isinstance(filter_expr, Filter)
-    assert filter_expr.predicate == predicate
+    assert filter_expr.condition == condition
 
     root_expr = filter_expr.child
     assert isinstance(root_expr, PrivateSource)
     assert root_expr.source_id == PRIVATE_ID
 
 
 def test_select():
@@ -297,51 +330,51 @@
     # This should fail whether augment and grouping are true or false
     with pytest.raises(
         ValueError,
         match=re.escape('"" (the empty string) is not a supported column name'),
     ):
         root_builder().flat_map(
             f=duplicate_rows,
-            max_num_rows=2,
             new_column_types={"": "VARCHAR"},
             augment=False,
             grouping=False,
+            max_num_rows=2,
         )
     with pytest.raises(
         ValueError,
         match=re.escape('"" (the empty string) is not a supported column name'),
     ):
         root_builder().flat_map(
             f=duplicate_rows,
-            max_num_rows=2,
             new_column_types={"": "VARCHAR"},
             augment=False,
             grouping=True,
+            max_num_rows=2,
         )
     with pytest.raises(
         ValueError,
         match=re.escape('"" (the empty string) is not a supported column name'),
     ):
         root_builder().flat_map(
             f=duplicate_rows,
-            max_num_rows=2,
             new_column_types={"": "VARCHAR"},
             augment=True,
             grouping=False,
+            max_num_rows=2,
         )
     with pytest.raises(
         ValueError,
         match=re.escape('"" (the empty string) is not a supported column name'),
     ):
         root_builder().flat_map(
             f=duplicate_rows,
-            max_num_rows=2,
             new_column_types={"": "VARCHAR"},
             augment=True,
             grouping=True,
+            max_num_rows=2,
         )
 
 
 def test_flat_map_augment_is_false():
     """QueryBuilder flat_map works as expected with augment=False."""
 
     def duplicate_rows(_: Row) -> List[Row]:
@@ -350,15 +383,20 @@
         Args:
             _: Row to apply function to.
         """
         return [{"C": "0"}, {"C": "1"}]
 
     query = (
         root_builder()
-        .flat_map(duplicate_rows, 2, new_column_types={"C": "VARCHAR"}, augment=False)
+        .flat_map(
+            duplicate_rows,
+            new_column_types={"C": "VARCHAR"},
+            augment=False,
+            max_num_rows=2,
+        )
         .groupby(KeySet.from_dict({"C": ["0", "1"]}))
         .count()
     )
 
     # Check query expression
     assert isinstance(query, GroupByCount)
 
@@ -389,15 +427,20 @@
         Args:
             _: Row to apply function to.
         """
         return [{"C": "0"}, {"C": "1"}]
 
     query = (
         root_builder()
-        .flat_map(duplicate_rows, 2, new_column_types={"C": "VARCHAR"}, augment=True)
+        .flat_map(
+            duplicate_rows,
+            new_column_types={"C": "VARCHAR"},
+            augment=True,
+            max_num_rows=2,
+        )
         .groupby(KeySet.from_dict({"A": ["0", "1"], "C": ["0", "1"]}))
         .count()
     )
 
     # Check query expression
     assert isinstance(query, GroupByCount)
 
@@ -425,21 +468,21 @@
     def duplicate_rows(_: Row) -> List[Row]:
         return [{"C": "0"}, {"C": "1"}]
 
     query = (
         root_builder()
         .flat_map(
             duplicate_rows,
-            2,
             new_column_types={
                 "C": ColumnDescriptor(
                     ColumnType.VARCHAR, allow_null=True, allow_nan=True, allow_inf=True
                 )
             },
             grouping=True,
+            max_num_rows=2,
         )
         .groupby(KeySet.from_dict({"A": ["0", "1"], "C": ["0", "1"]}))
         .count()
     )
 
     # Check query expression
     assert isinstance(query, GroupByCount)
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_query_expr_compiler.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_query_expr_compiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# type: ignore[attr-defined]
 """Tests for QueryExprCompiler."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
-# pylint: disable= no-member, protected-access, no-self-use
+# Copyright Tumult Labs 2023
+
+# pylint: disable=no-member, protected-access, no-self-use
 
 import datetime
-from typing import List, Union
+from typing import Dict, List, Union
 from unittest.mock import patch
 
 import pandas as pd
 import pytest
 import sympy as sp
-from pyspark.sql import SparkSession
-from pyspark.sql.functions import col  # pylint: disable=no-name-in-module
+from pyspark.sql import DataFrame, SparkSession
+from pyspark.sql.functions import col
 from pyspark.sql.types import (
     DateType,
     DoubleType,
     LongType,
     StringType,
     StructField,
     StructType,
@@ -28,14 +28,16 @@
 from tmlt.analytics._query_expr_compiler import QueryExprCompiler
 from tmlt.analytics._schema import (
     ColumnDescriptor,
     ColumnType,
     Schema,
     analytics_to_spark_columns_descriptor,
 )
+from tmlt.analytics._table_identifier import Identifier, NamedTable
+from tmlt.analytics._transformation_utils import get_table_from_ref
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountMechanism,
     Filter,
     FlatMap,
     GroupByBoundedAverage,
@@ -65,18 +67,15 @@
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
 from tmlt.core.measurements.aggregations import NoiseMechanism
 from tmlt.core.measures import PureDP, RhoZCDP
 from tmlt.core.metrics import DictMetric, SymmetricDifference
 
-from ..conftest import (  # pylint: disable=no-name-in-module
-    assert_frame_equal_with_sort,
-    create_mock_measurement,
-)
+from ..conftest import assert_frame_equal_with_sort, create_mock_measurement
 
 GROUPBY_TWO_COLUMNS = pd.DataFrame([["0", 0], ["0", 1], ["1", 1]], columns=["A", "B"])
 GROUPBY_TWO_SCHEMA = StructType(
     [StructField("A", StringType(), False), StructField("B", LongType(), False)]
 )
 GET_GROUPBY_TWO = lambda: SparkSession.builder.getOrCreate().createDataFrame(
     GROUPBY_TWO_COLUMNS, schema=GROUPBY_TWO_SCHEMA
@@ -212,17 +211,17 @@
         [
             GroupByBoundedSum(
                 child=ReplaceNullAndNan(
                     replace_with={},
                     child=FlatMap(
                         child=PrivateSource("private"),
                         f=lambda row: [{}, {}],
-                        max_num_rows=2,
                         schema_new_columns=Schema({}),
                         augment=True,
+                        max_num_rows=2,
                     ),
                 ),
                 groupby_keys=KeySet.from_dict({}),
                 measure_column="X",
                 low=0.0,
                 high=3.0,
             )
@@ -234,22 +233,22 @@
             GroupByBoundedSum(
                 child=ReplaceNullAndNan(
                     replace_with={},
                     child=FlatMap(
                         child=FlatMap(
                             child=PrivateSource("private"),
                             f=lambda row: [{"Repeat": 1 if row["A"] == "0" else 2}],
-                            max_num_rows=1,
                             schema_new_columns=Schema({"Repeat": "INTEGER"}),
                             augment=True,
+                            max_num_rows=1,
                         ),
                         f=lambda row: [{"i": row["X"]} for i in range(row["Repeat"])],
-                        max_num_rows=2,
                         schema_new_columns=Schema({"i": "DECIMAL"}),
                         augment=False,
+                        max_num_rows=2,
                     ),
                 ),
                 groupby_keys=KeySet.from_dict({}),
                 measure_column="i",
                 low=0.0,
                 high=3.0,
             )
@@ -261,38 +260,38 @@
             GroupByBoundedSum(
                 child=ReplaceNullAndNan(
                     replace_with={},
                     child=FlatMap(
                         child=FlatMap(
                             child=PrivateSource("private"),
                             f=lambda row: [{"Repeat": 1 if row["A"] == "0" else 2}],
-                            max_num_rows=1,
                             schema_new_columns=Schema(
                                 {"Repeat": "INTEGER"}, grouping_column="Repeat"
                             ),
                             augment=True,
+                            max_num_rows=1,
                         ),
                         f=lambda row: [{"i": row["X"]} for i in range(row["Repeat"])],
-                        max_num_rows=2,
                         schema_new_columns=Schema({"i": "DECIMAL"}),
                         augment=True,
+                        max_num_rows=2,
                     ),
                 ),
                 groupby_keys=KeySet.from_dict({"Repeat": [1, 2]}),
                 measure_column="i",
                 low=0.0,
                 high=3.0,
             )
         ],
         [pd.DataFrame({"Repeat": [1, 2], "sum": [3.0, 6.0]})],
     ),
     (  # Filter
         [
             GroupByCount(
-                child=Filter(child=PrivateSource("private"), predicate="A == '0'"),
+                child=Filter(child=PrivateSource("private"), condition="A == '0'"),
                 groupby_keys=KeySet.from_dict({}),
             )
         ],
         [pd.DataFrame({"count": [3]})],
     ),
     (  # Rename
         [
@@ -522,104 +521,119 @@
 
     groupby_one_column_df = spark.createDataFrame(
         pd.DataFrame([["0"], ["1"], ["2"]], columns=["A"]),
         schema=StructType([StructField("A", StringType(), False)]),
     )
     request.cls.groupby_one_column_df = groupby_one_column_df
 
-    stability = {"private": sp.Integer(3), "private_2": sp.Integer(3)}
+    stability = {
+        NamedTable("private"): sp.Integer(3),
+        NamedTable("private_2"): sp.Integer(3),
+    }
 
     request.cls.stability = stability
 
     input_domain = DictDomain(
         {
-            "private": SparkDataFrameDomain(
+            NamedTable("private"): SparkDataFrameDomain(
                 {
                     "A": SparkStringColumnDescriptor(),
                     "B": SparkIntegerColumnDescriptor(),
                     "X": SparkFloatColumnDescriptor(),
                 }
             ),
-            "private_2": SparkDataFrameDomain(
+            NamedTable("private_2"): SparkDataFrameDomain(
                 {
                     "A": SparkStringColumnDescriptor(),
                     "C": SparkIntegerColumnDescriptor(),
                 }
             ),
         }
     )
 
     request.cls.input_domain = input_domain
 
     catalog = Catalog()
-    catalog.add_private_source(
+    catalog.add_private_table(
         "private",
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR),
             "B": ColumnDescriptor(ColumnType.INTEGER),
             "X": ColumnDescriptor(ColumnType.DECIMAL),
         },
-        stability=3,
     )
-    catalog.add_private_view(
+    catalog.add_private_table(
         "private_2",
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR),
             "C": ColumnDescriptor(ColumnType.INTEGER),
         },
-        stability=3,
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "public",
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR),
             "B": ColumnDescriptor(ColumnType.INTEGER),
             "A+B": ColumnDescriptor(ColumnType.INTEGER),
         },
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "dtypes",
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR),
             "int": ColumnDescriptor(ColumnType.INTEGER),
             "float": ColumnDescriptor(
                 ColumnType.DECIMAL, allow_nan=True, allow_inf=True
             ),
             "date": ColumnDescriptor(ColumnType.DATE),
             "timestamp": ColumnDescriptor(ColumnType.TIMESTAMP),
         },
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "groupby_two_columns",
         {
             "A": ColumnDescriptor(ColumnType.VARCHAR),
             "B": ColumnDescriptor(ColumnType.INTEGER),
         },
     )
-    catalog.add_public_source(
+    catalog.add_public_table(
         "groupby_one_column", {"A": ColumnDescriptor(ColumnType.VARCHAR)}
     )
 
     request.cls.catalog = catalog
 
     input_metric = DictMetric(
-        {"private": SymmetricDifference(), "private_2": SymmetricDifference()}
+        {
+            NamedTable("private"): SymmetricDifference(),
+            NamedTable("private_2"): SymmetricDifference(),
+        }
     )
     request.cls.input_metric = input_metric
 
     request.cls.compiler = QueryExprCompiler()
 
 
 @pytest.mark.usefixtures("test_data")
 class TestQueryExprCompiler:
     """Unit tests for class QueryExprCompiler.
 
     Tests :class:`~tmlt.analytics._query_expr_compiler.QueryExprCompiler`.
     """
 
+    sdf: DataFrame
+    dtypes_df: DataFrame
+    join_df: DataFrame
+    groupby_one_column_df: DataFrame
+    groupby_two_columns_df: DataFrame
+    stability: Dict
+    input_domain: DictDomain
+    input_metric: DictMetric
+    catalog: Catalog
+    compiler: QueryExprCompiler
+
     @pytest.mark.parametrize(
         "query_expr,expected",
         [
             (
                 GroupByCountDistinct(
                     child=PrivateSource("private"),
                     groupby_keys=KeySet.from_dict({}),
@@ -692,16 +706,17 @@
             input_metric=self.input_metric,
             public_sources={
                 "public": self.join_df,
                 "groupby_two_columns": self.groupby_two_columns_df,
                 "groupby_one_column": self.groupby_one_column_df,
             },
             catalog=self.catalog,
+            table_constraints={t: [] for t in self.stability.keys()},
         )
-        actual = measurement({"private": count_distinct_df})
+        actual = measurement({NamedTable("private"): count_distinct_df})
         assert len(actual) == 1
         assert_frame_equal_with_sort(actual[0].toPandas(), expected)
 
     @pytest.mark.parametrize("query_exprs,expected", QUERY_EXPR_COMPILER_TESTS)
     def test_queries(self, query_exprs: List[QueryExpr], expected: List[pd.DataFrame]):
         """Tests that compiled measurement produces correct results.
 
@@ -718,16 +733,17 @@
             public_sources={
                 "public": self.join_df,
                 "dtypes": self.dtypes_df,
                 "groupby_two_columns": self.groupby_two_columns_df,
                 "groupby_one_column": self.groupby_one_column_df,
             },
             catalog=self.catalog,
+            table_constraints={t: [] for t in self.stability.keys()},
         )
-        actual = measurement({"private": self.sdf})
+        actual = measurement({NamedTable("private"): self.sdf})
         assert len(actual) == len(expected)
         for actual_sdf, expected_df in zip(actual, expected):
             assert_frame_equal_with_sort(actual_sdf.toPandas(), expected_df)
 
     @pytest.mark.parametrize(
         "query,output_measure,expected",
         [
@@ -905,26 +921,26 @@
                 GroupByBoundedSum(
                     child=ReplaceNullAndNan(
                         replace_with={},
                         child=FlatMap(
                             child=FlatMap(
                                 child=PrivateSource("private"),
                                 f=lambda row: [{"Repeat": 1 if row["A"] == "0" else 2}],
-                                max_num_rows=1,
                                 schema_new_columns=Schema(
                                     {"Repeat": "INTEGER"}, grouping_column="Repeat"
                                 ),
                                 augment=True,
+                                max_num_rows=1,
                             ),
                             f=lambda row: [
                                 {"i": row["X"]} for i in range(row["Repeat"])
                             ],
-                            max_num_rows=2,
                             schema_new_columns=Schema({"i": "DECIMAL"}),
                             augment=True,
+                            max_num_rows=2,
                         ),
                     ),
                     groupby_keys=KeySet.from_dict({"Repeat": [1, 2]}),
                     measure_column="i",
                     low=0.0,
                     high=3.0,
                     mechanism=SumMechanism.LAPLACE,
@@ -946,16 +962,17 @@
             [query],
             privacy_budget=sp.oo,
             stability=self.stability,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={"public": self.join_df},
             catalog=self.catalog,
+            table_constraints={t: [] for t in self.stability.keys()},
         )
-        actual = measurement({"private": self.sdf})
+        actual = measurement({NamedTable("private"): self.sdf})
         assert len(actual) == len(expected)
         for actual_sdf, expected_df in zip(actual, expected):
             assert_frame_equal_with_sort(actual_sdf.toPandas(), expected_df)
 
     @pytest.mark.parametrize(
         "query_exprs",
         [
@@ -1016,26 +1033,26 @@
                             replace_with={},
                             child=FlatMap(
                                 child=FlatMap(
                                     child=PrivateSource("private"),
                                     f=lambda row: [
                                         {"Repeat": 1 if row["A"] == "0" else 2}
                                     ],
-                                    max_num_rows=1,
                                     schema_new_columns=Schema(
                                         {"Repeat": "INTEGER"}, grouping_column="Repeat"
                                     ),
                                     augment=True,
+                                    max_num_rows=1,
                                 ),
                                 f=lambda row: [
                                     {"i": row["X"]} for i in range(row["Repeat"])
                                 ],
-                                max_num_rows=2,
                                 schema_new_columns=Schema({"i": "DECIMAL"}),
                                 augment=True,
+                                max_num_rows=2,
                             ),
                         ),
                         groupby_keys=KeySet.from_dict({"Repeat": [1, 2]}),
                         measure_column="i",
                         low=0.0,
                         high=3.0,
                         mechanism=SumMechanism.GAUSSIAN,
@@ -1045,43 +1062,51 @@
         ],
     )
     def test_gaussian_noise_param_on_float_errors(self, query_exprs: List[QueryExpr]):
         """Tests that Gaussian noise with floating-point values errors."""
         compiler = QueryExprCompiler(output_measure=RhoZCDP())
         with pytest.raises(
             NotImplementedError,
-            match="GAUSSIAN noise is not yet compatible with floating-point values.",
+            match=(
+                "(GAUSSIAN)|(Discrete gaussian) noise is not yet compatible with"
+                " floating-point values."
+            ),
         ):
             compiler(
                 query_exprs,
                 privacy_budget=sp.oo,
                 stability=self.stability,
                 input_domain=self.input_domain,
                 input_metric=self.input_metric,
                 public_sources={"public": self.join_df},
                 catalog=self.catalog,
+                table_constraints={t: [] for t in self.stability.keys()},
             )
 
     def test_join_public_dataframe(self, spark):
         """Public join works with public tables given as Spark dataframes."""
         # This sets up a DF with a column that Spark thinks could contain NaNs,
         # but which doesn't actually contain any. This is allowed by Analytics,
         # but it has caused some bugs in the past which this test should
         # detect.
         public_sdf = spark.createDataFrame(
             pd.DataFrame({"A": ["0", "1"], "Y": [0.1, float("nan")]})
         ).fillna(0)
 
-        output_sdf = self.compiler.build_transformation(
+        transformation, reference, _constraints = self.compiler.build_transformation(
             JoinPublic(PrivateSource("private"), public_sdf),
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={},
             catalog=self.catalog,
-        )({"private": self.sdf})
+            table_constraints={t: [] for t in self.stability.keys()},
+        )
+
+        source_dict = {NamedTable("private"): self.sdf}
+        output_sdf = get_table_from_ref(transformation, reference)(source_dict)
 
         assert_frame_equal_with_sort(
             output_sdf.toPandas(),
             pd.DataFrame(
                 [
                     ("0", 0, 0.0, 0.1),
                     ("0", 0, 1.0, 0.1),
@@ -1095,26 +1120,29 @@
     def test_join_private(self, spark):
         """Tests that join private works."""
         sdf_2 = spark.createDataFrame(  # pylint: disable=no-member
             pd.DataFrame(
                 [["0", 0], ["0", 2], ["1", 2], ["0", 0], ["1", 4]], columns=["A", "C"]
             )
         )
-        output_sdf = self.compiler.build_transformation(
+        transformation, reference, _constraints = self.compiler.build_transformation(
             JoinPrivate(
                 child=PrivateSource("private"),
                 right_operand_expr=PrivateSource("private_2"),
                 truncation_strategy_left=TruncationStrategy.DropExcess(3),
                 truncation_strategy_right=TruncationStrategy.DropExcess(3),
             ),
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={},
             catalog=self.catalog,
-        )({"private": self.sdf, "private_2": sdf_2})
+            table_constraints={t: [] for t in self.stability.keys()},
+        )
+        source_dict = {NamedTable("private"): self.sdf, NamedTable("private_2"): sdf_2}
+        output_sdf = get_table_from_ref(transformation, reference)(source_dict)
 
         assert_frame_equal_with_sort(
             output_sdf.toPandas(),
             pd.DataFrame(
                 [
                     ["0", 0, 0.0, 0],
                     ["0", 0, 0.0, 0],
@@ -1180,25 +1208,28 @@
                 ),
                 6,  # 1 * (1 * 3) + 1 * (1 * 3)
             ),
         ],
     )
     def test_join_private_output_stability(self, join_query, expected_output_stability):
         """Tests that join private gives correct output stability."""
-        transformation = self.compiler.build_transformation(
+        transformation, reference, _constraints = self.compiler.build_transformation(
             join_query,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={},
             catalog=self.catalog,
+            table_constraints={t: [] for t in self.stability.keys()},
         )
-        assert (
-            transformation.stability_function(self.stability)
-            == expected_output_stability
-        )
+
+        get_value_transform = get_table_from_ref(transformation, reference)
+
+        output_stability = get_value_transform.stability_function(self.stability)
+
+        assert output_stability == expected_output_stability
 
     def test_join_private_invalid_truncation_strategy(self):
         """Tests that join_private raises error if truncation strategy is invalid."""
 
         class Strategy(TruncationStrategy.Type):
             """An invalid truncation strategy."""
 
@@ -1214,59 +1245,62 @@
         with pytest.raises(ValueError, match=expected_error_msg):
             self.compiler.build_transformation(
                 query,
                 input_domain=self.input_domain,
                 input_metric=self.input_metric,
                 public_sources={},
                 catalog=self.catalog,
+                table_constraints={t: [] for t in self.stability.keys()},
             )
 
     @pytest.mark.parametrize(
         "flatmap_query,measure,expected_output_stability",
         [
             (
                 FlatMap(
                     child=PrivateSource("private"),
                     f=lambda _: [{"G": "a"}, {"G": "b"}],
-                    max_num_rows=2,
                     schema_new_columns=Schema({"G": "VARCHAR"}, grouping_column="G"),
                     augment=True,
+                    max_num_rows=2,
                 ),
                 RhoZCDP(),
                 3 * sp.sqrt(2),
             ),
             (
                 FlatMap(
                     child=PrivateSource("private"),
                     f=lambda _: [{"G": "a"}, {"G": "b"}],
-                    max_num_rows=2,
                     schema_new_columns=Schema({"G": "VARCHAR"}),
                     augment=True,
+                    max_num_rows=2,
                 ),
                 PureDP(),
                 6,
             ),
         ],
     )
     def test_flatmap_output_stability(
         self, flatmap_query, measure, expected_output_stability
     ):
         """Tests that flatmap gives correct output stability."""
         compiler = QueryExprCompiler(output_measure=measure)
-        transformation = compiler.build_transformation(
+        transformation, reference, _constraints = compiler.build_transformation(
             flatmap_query,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={},
             catalog=self.catalog,
+            table_constraints={t: [] for t in self.stability.keys()},
         )
-        assert (
-            transformation.stability_function(self.stability)
-            == expected_output_stability
-        )
+        get_value_transform = get_table_from_ref(transformation, reference)
+
+        output_stability = get_value_transform.stability_function(self.stability)
+
+        assert output_stability == expected_output_stability
 
     def test_float_groupby_sum(self, spark):
         """Tests that groupby sum on floating-point-valued column uses laplace."""
         sdf_float = spark.createDataFrame(
             pd.DataFrame(
                 [["0", 0, 0.0], ["0", 0, 1.0], ["0", 1, 2.0], ["1", 0, 3.0]],
                 columns=["A", "B", "X"],
@@ -1287,32 +1321,33 @@
             query_exprs,
             privacy_budget=sp.oo,
             stability=self.stability,
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             public_sources={},
             catalog=self.catalog,
+            table_constraints={t: [] for t in self.stability.keys()},
         )
-        actual = measurement({"private": sdf_float})
+        actual = measurement({NamedTable("private"): sdf_float})
         expected = [pd.DataFrame({"A": ["0", "1"], "sum": [2.0, 1.0]})]
         for actual_sdf, expected_df in zip(actual, expected):
             assert_frame_equal_with_sort(actual_sdf.toPandas(), expected_df)
 
     @pytest.mark.parametrize(
         "query_exprs",
         [
             (
                 # Top-level query needs to be instance of measurement QueryExpr
                 [
                     FlatMap(
                         child=PrivateSource("private"),
                         f=lambda row: [{}, {}],
-                        max_num_rows=2,
                         schema_new_columns=Schema({}),
                         augment=True,
+                        max_num_rows=2,
                     )
                 ]
             ),
             (  # Query's child has to be transformation QueryExpr
                 [
                     GroupByBoundedSum(
                         child=GroupByCount(
@@ -1337,51 +1372,61 @@
                 query_exprs,
                 privacy_budget=sp.oo,
                 stability=self.stability,
                 input_domain=self.input_domain,
                 input_metric=self.input_metric,
                 public_sources={"public": self.join_df},
                 catalog=self.catalog,
+                table_constraints={t: [] for t in self.stability.keys()},
             )
 
     def test_different_source_id(self):
         """Tests that different source ids are allowed."""
-        self.catalog.add_private_view(
+        self.catalog.add_private_table(
             source_id="doubled",
             col_types={
                 "A": ColumnType.VARCHAR,
                 "B": ColumnType.INTEGER,
                 "X": ColumnType.DECIMAL,
             },
-            stability=self.catalog.private_table.stability * 2,
         )
         query_exprs = [
             GroupByCount(
                 child=PrivateSource("private"), groupby_keys=KeySet.from_dict({})
             ),
             GroupByCount(
                 child=PrivateSource("doubled"), groupby_keys=KeySet.from_dict({})
             ),
         ]
-        stability = {"doubled": self.stability["private"] * 2, **self.stability}
+        stability = {
+            NamedTable("doubled"): self.stability[NamedTable("private")] * 2,
+            **self.stability,
+        }
         input_domain = DictDomain(
-            {"doubled": self.input_domain["private"], **self.input_domain.key_to_domain}
+            {
+                NamedTable("doubled"): self.input_domain[NamedTable("private")],
+                **self.input_domain.key_to_domain,
+            }
         )
         input_metric = DictMetric(
-            {"doubled": self.input_metric["private"], **self.input_metric.key_to_metric}
+            {
+                NamedTable("doubled"): self.input_metric[NamedTable("private")],
+                **self.input_metric.key_to_metric,
+            }
         )
 
         measurement = self.compiler(
             query_exprs,
             privacy_budget=sp.Integer(10),
             stability=stability,
             input_domain=input_domain,
             input_metric=input_metric,
             public_sources={"public": self.join_df},
             catalog=self.catalog,
+            table_constraints={t: [] for t in stability.keys()},
         )
         assert measurement.privacy_relation(stability, sp.Integer(10))
 
     def test_call_no_queries(self):
         """``__call__`` raises error if the sequence of queries has length 0."""
         with pytest.raises(
             ValueError, match=r"At least one query needs to be provided"
@@ -1390,14 +1435,15 @@
                 queries=[],
                 privacy_budget=sp.Integer(10),
                 stability=self.stability,
                 input_domain=self.input_domain,
                 input_metric=self.input_metric,
                 public_sources={"public": self.join_df},
                 catalog=self.catalog,
+                table_constraints={t: [] for t in self.stability.keys()},
             )
 
 
 class TestCompileGroupByQuantile:
     """Test compiling GroupByQuantile.
 
     This is separate from other tests because some noise is added even when
@@ -1422,34 +1468,33 @@
                     ["M", 24],
                     ["M", 25],
                 ],
                 columns=["Gender", "Age"],
             )
         )
         catalog = Catalog()
-        catalog.add_private_source(
+        catalog.add_private_table(
             "private",
             {
                 "Gender": ColumnDescriptor(ColumnType.VARCHAR),
                 "Age": ColumnDescriptor(ColumnType.INTEGER),
             },
-            stability=1,
         )
-        stability = {"private": sp.Integer(1)}
+        stability = {NamedTable("private"): sp.Integer(1)}
         input_domain = DictDomain(
             {
-                "private": SparkDataFrameDomain(
+                NamedTable("private"): SparkDataFrameDomain(
                     {
                         "Gender": SparkStringColumnDescriptor(),
                         "Age": SparkIntegerColumnDescriptor(),
                     }
                 )
             }
         )
-        input_metric = DictMetric({"private": SymmetricDifference()})
+        input_metric = DictMetric({NamedTable("private"): SymmetricDifference()})
         compiler = QueryExprCompiler(output_measure=output_measure)
 
         query_expr = GroupByQuantile(
             child=PrivateSource("private"),
             groupby_keys=KeySet.from_dict({"Gender": ["M", "F"]}),
             measure_column="Age",
             quantile=0.5,
@@ -1461,68 +1506,73 @@
             [query_expr],
             privacy_budget=sp.Integer(1000),
             stability=stability,
             input_domain=input_domain,
             input_metric=input_metric,
             public_sources={},
             catalog=catalog,
+            table_constraints={t: [] for t in stability},
         )
         assert measurement.input_domain == input_domain
         assert measurement.input_metric == input_metric
         assert measurement.output_measure == output_measure
         assert measurement.privacy_function(stability) == sp.Integer(1000)
 
-        [actual] = measurement({"private": sdf})
+        [actual] = measurement({NamedTable("private"): sdf})
 
         assert 26 < actual.filter(col("Gender") == "F").collect()[0]["out"] <= 28
         assert 22 < actual.filter(col("Gender") == "M").collect()[0]["out"] <= 24
 
 
 @pytest.fixture(name="test_component_data", scope="class")
 def setup_components(request):
     """Set up test."""
-    request.cls._stability = {"test": sp.Integer(3)}
+    request.cls._stability = {NamedTable("test"): sp.Integer(3)}
     request.cls._privacy_budget = sp.Integer(5)
     request.cls._input_domain = DictDomain(
         {
-            "test": SparkDataFrameDomain(
+            NamedTable("test"): SparkDataFrameDomain(
                 analytics_to_spark_columns_descriptor(
                     Schema({"A": "VARCHAR", "X": "INTEGER"})
                 )
             )
         }
     )
-    request.cls._input_metric = DictMetric({"test": SymmetricDifference()})
+    request.cls._input_metric = DictMetric({NamedTable("test"): SymmetricDifference()})
     request.cls._catalog = Catalog()
-    request.cls._catalog.add_private_source(
-        source_id="test",
-        col_types={"A": ColumnType.VARCHAR, "X": ColumnType.INTEGER},
-        stability=3,
+    request.cls._catalog.add_private_table(
+        source_id="test", col_types={"A": ColumnType.VARCHAR, "X": ColumnType.INTEGER}
     )
 
 
 @pytest.mark.usefixtures("test_component_data")
 class TestComponentIsUsed:
     """Tests that specific components are used inside of compiled measurements."""
 
+    _stability: Dict[Identifier, sp.Integer]
+    _privacy_budget: sp.Integer
+    _input_domain: DictDomain
+    _input_metric: DictMetric
+    _catalog: Catalog
+
     @pytest.mark.parametrize(
         "output_measure,query_expr,column,preprocessing_stability",
         [
             (output_measure, query_expr, column, preprocessing_stability)
             for output_measure in [PureDP(), RhoZCDP()]
             for preprocessing_expr, preprocessing_stability in [
                 (
                     ReplaceNullAndNan(
                         replace_with={},
                         child=FlatMap(
                             child=PrivateSource(source_id="test"),
                             f=lambda row: [{}, {}],
-                            max_num_rows=2,
                             schema_new_columns=Schema({}),
                             augment=True,
+                            max_num_rows=2,
                         ),
                     ),
                     2,
                 ),
                 (PrivateSource(source_id="test"), 1),
             ]
             for query_expr, column in [
@@ -1615,46 +1665,46 @@
         ) as mock_create_average_measurement, patch(
             "tmlt.analytics._query_expr_compiler._measurement_visitor."
             "create_sum_measurement"
         ) as mock_create_sum_measurement, patch(
             "tmlt.analytics._query_expr_compiler._measurement_visitor."
             "create_count_measurement"
         ) as mock_create_count_measurement:
-
             d_in = sp.Integer(3)
             d_out = sp.Integer(5)
             compiler = QueryExprCompiler(output_measure=output_measure)
             mock_create_measurement_dict = {
                 "count": mock_create_count_measurement,
                 "sum": mock_create_sum_measurement,
                 "average": mock_create_average_measurement,
                 "variance": mock_create_variance_measurement,
                 "standard deviation": mock_create_standard_deviation_measurement,
                 "quantile": mock_create_quantile_measurement,
             }
             mock_create_measurement = mock_create_measurement_dict[column]
             mock_create_measurement.return_value = create_mock_measurement(
-                input_domain=self._input_domain["test"],
-                input_metric=self._input_metric["test"],
+                input_domain=self._input_domain[NamedTable("test")],
+                input_metric=self._input_metric[NamedTable("test")],
                 output_measure=output_measure,
                 privacy_function_return_value=d_out,
                 privacy_function_implemented=True,
             )
             _ = compiler(
                 [query_expr],
                 privacy_budget=self._privacy_budget,
                 stability=self._stability,
                 input_domain=self._input_domain,
                 input_metric=self._input_metric,
                 public_sources={},
                 catalog=self._catalog,
+                table_constraints={t: [] for t in self._stability.keys()},
             )
             expected_arguments = {  # Other arguments are not checked
-                "input_domain": self._input_domain["test"],
-                "input_metric": self._input_metric["test"],
+                "input_domain": self._input_domain[NamedTable("test")],
+                "input_metric": self._input_metric[NamedTable("test")],
                 "d_in": d_in * preprocessing_stability,
                 "d_out": d_out,
             }
             if column != "quantile":
                 expected_arguments["noise_mechanism"] = (
                     NoiseMechanism.GEOMETRIC
                     if isinstance(output_measure, PureDP)
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_query_expression.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_query_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Tests for QueryExpr."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 # pylint: disable=too-many-arguments, unidiomatic-typecheck, pointless-string-statement
 
 import datetime
 import re
 from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple, Type, Union
 
 import pandas as pd
 import pytest
+from pyspark.sql import DataFrame
 from pyspark.sql.types import BinaryType, StructField, StructType
 
 from tmlt.analytics._schema import Schema
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.query_expr import (
     DropInfinity,
     DropNullAndNan,
@@ -88,15 +89,15 @@
     ):
         Rename(PrivateSource("private"), {"A": ""})
 
 
 def test_invalid_filter():
     """Tests that invalid Filter errors on post-init."""
     with pytest.raises(TypeError):
-        Filter(PrivateSource("private"), 0)
+        Filter(PrivateSource("private"), 0)  # type: ignore
 
 
 @pytest.mark.parametrize(
     "columns, expected_error_msg",
     [
         (True, "type of columns must be a list; got bool instead"),
         ([1], "type of columns[0] must be str; got int instead"),
@@ -152,17 +153,17 @@
             False,
             "Limit on number of rows '-1' must be nonnegative.",
         ),
         (  # Invalid augment
             FlatMap(
                 child=PrivateSource("private"),
                 f=lambda row: [{"Repeat": 1 if row["A"] == "0" else 2}],
-                max_num_rows=1,
                 schema_new_columns=Schema({"Repeat": "INTEGER"}),
                 augment=True,
+                max_num_rows=1,
             ),
             lambda row: [{"i": row["X"]} for i in range(row["Repeat"])],
             2,
             Schema({"i": "INTEGER"}),
             1.0,
             "type of augment must be bool; got float instead",
         ),
@@ -183,15 +184,15 @@
     max_num_rows: int,
     schema_new_columns: Schema,
     augment: bool,
     expected_error_msg: str,
 ):
     """Tests that invalid FlatMap errors on post-init."""
     with pytest.raises((TypeError, ValueError), match=expected_error_msg):
-        FlatMap(child, func, max_num_rows, schema_new_columns, augment)
+        FlatMap(child, func, schema_new_columns, augment, max_num_rows)
 
 
 @pytest.mark.parametrize(
     "join_columns,expected_error_msg",
     [
         ([], "Provided join columns must not be empty"),
         (["A", "A"], "Join columns must be distinct"),
@@ -300,15 +301,22 @@
             "type of low must be either float or int; got str instead",
         ),
         (
             KeySet.from_dict({"A": ["0", "1"]}),
             "B",
             10.0,
             1,
-            "Lower bound '10.0' can not be greater than the upper bound '1.0'.",
+            "Lower bound '10.0' must be less than the upper bound '1.0'.",
+        ),
+        (
+            KeySet.from_dict({"A": ["0", "1"]}),
+            "B",
+            1.0,
+            1.0,
+            "Lower bound '1.0' must be less than the upper bound '1.0'.",
         ),
     ],
 )
 def test_invalid_groupbyagg(
     keys: KeySet, measure_column: str, low: float, high: float, expected_error_msg: str
 ):
     """Test invalid GroupBy aggregates errors on post-init."""
@@ -359,15 +367,23 @@
         ),
         (
             KeySet.from_dict({"A": ["0", "1"]}),
             "B",
             0.5,
             10.0,
             1.0,
-            "Lower bound '10.0' can not be greater than the upper bound '1.0'.",
+            "Lower bound '10.0' must be less than the upper bound '1.0'.",
+        ),
+        (
+            KeySet.from_dict({"A": ["0", "1"]}),
+            "B",
+            0.5,
+            1.0,
+            1.0,
+            "Lower bound '1.0' must be less than the upper bound '1.0'.",
         ),
     ],
 )
 def test_invalid_groupbyquantile(
     keys: KeySet,
     measure_column: str,
     quantile: float,
@@ -496,14 +512,15 @@
 """Tests for JoinPublic with a Spark DataFrame as the public table."""
 
 
 def test_join_public_string_nan(spark):
     """Test that the string "NaN" is allowed in string-valued columns."""
     df = spark.createDataFrame(pd.DataFrame({"col": ["nan", "NaN", "NAN", "Nan"]}))
     query_expr = JoinPublic(PrivateSource("a"), df)
+    assert isinstance(query_expr.public_table, DataFrame)
     assert_frame_equal_with_sort(query_expr.public_table.toPandas(), df.toPandas())
 
 
 def test_join_public_dataframe_validation_column_type(spark):
     """Unsupported column types are rejected in JoinPublic."""
     data = [{"bytes": b"some bytes"}]
     schema = StructType([StructField("bytes", BinaryType(), False)])
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_query_expression_visitor.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_query_expression_visitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Tests for QueryExprVisitor."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # pylint: disable=no-self-use
 
 import pytest
 
 from tmlt.analytics._schema import Schema
+from tmlt.analytics.constraints import MaxRowsPerID
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.query_expr import (
     DropInfinity,
     DropNullAndNan,
+    EnforceConstraint,
     Filter,
     FlatMap,
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
     GroupByBoundedSum,
     GroupByBoundedVariance,
     GroupByCount,
@@ -69,14 +71,17 @@
 
     def visit_drop_infinity(self, expr):
         return "DropInfinity"
 
     def visit_drop_null_and_nan(self, expr):
         return "DropNullAndNan"
 
+    def visit_enforce_constraint(self, expr):
+        return "EnforceConstraint"
+
     def visit_groupby_count(self, expr):
         return "GroupByCount"
 
     def visit_groupby_count_distinct(self, expr):
         return "GroupByCountDistinct"
 
     def visit_groupby_quantile(self, expr):
@@ -101,15 +106,15 @@
         (PrivateSource("P"), "PrivateSource"),
         (Rename(PrivateSource("P"), {"A": "B"}), "Rename"),
         (Filter(PrivateSource("P"), "A<B"), "Filter"),
         (Select(PrivateSource("P"), ["A"]), "Select"),
         (Map(PrivateSource("P"), lambda r: r, Schema({"A": "VARCHAR"}), True), "Map"),
         (
             FlatMap(
-                PrivateSource("P"), lambda r: [r], 1, Schema({"A": "VARCHAR"}), True
+                PrivateSource("P"), lambda r: [r], Schema({"A": "VARCHAR"}), True, 1
             ),
             "FlatMap",
         ),
         (
             JoinPrivate(
                 PrivateSource("P"),
                 PrivateSource("Q"),
@@ -125,14 +130,15 @@
         ),
         (
             ReplaceInfinity(PrivateSource("P"), {"column": (-100.0, 100.0)}),
             "ReplaceInfinity",
         ),
         (DropInfinity(PrivateSource("P"), ["column"]), "DropInfinity"),
         (DropNullAndNan(PrivateSource("P"), ["column"]), "DropNullAndNan"),
+        (EnforceConstraint(PrivateSource("P"), MaxRowsPerID(5)), "EnforceConstraint"),
         (GroupByCount(PrivateSource("P"), KeySet.from_dict({})), "GroupByCount"),
         (
             GroupByCountDistinct(PrivateSource("P"), KeySet.from_dict({})),
             "GroupByCountDistinct",
         ),
         (
             GroupByQuantile(PrivateSource("P"), KeySet.from_dict({}), "A", 0.5, 0, 1),
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_schema.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for schema."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # pylint: disable=pointless-string-statement
 import re
 
 import pytest
 
 from tmlt.analytics._schema import ColumnDescriptor, ColumnType, Schema
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_schema_conversion.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_schema_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests conversion functions in :mod:`~tmlt.analytics._schema`."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # pylint: disable=no-self-use
 import datetime
 
 import pytest
 from pyspark.sql import types as spark_types
 
 from tmlt.analytics._schema import (
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_session.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_session.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,92 @@
-# type: ignore[attr-defined]
 """Unit tests for Session."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
+
 # pylint: disable=no-self-use, unidiomatic-typecheck, no-member
 
 import re
-from typing import Any, Dict, List, Tuple, Type, Union
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 from unittest.mock import ANY, Mock, patch
 
 import pandas as pd
 import pytest
 import sympy as sp
-from pyspark.sql import DataFrame, SparkSession
+from pyspark.sql import DataFrame
 from pyspark.sql.types import (
     BooleanType,
     DoubleType,
     FloatType,
     IntegerType,
     LongType,
     StringType,
     StructField,
     StructType,
 )
 from typeguard import check_type
 
+from tmlt.analytics._neighboring_relation import (
+    AddRemoveKeys,
+    AddRemoveRows,
+    AddRemoveRowsAcrossGroups,
+    Conjunction,
+    NeighboringRelation,
+)
 from tmlt.analytics._query_expr_compiler import QueryExprCompiler
 from tmlt.analytics._schema import (
     ColumnDescriptor,
     ColumnType,
     Schema,
     analytics_to_spark_columns_descriptor,
     spark_schema_to_analytics_columns,
 )
-from tmlt.analytics.privacy_budget import PrivacyBudget, PureDPBudget, RhoZCDPBudget
-from tmlt.analytics.protected_change import AddMaxRows, AddMaxRowsInMaxGroups, AddOneRow
+from tmlt.analytics._table_identifier import NamedTable, TableCollection
+from tmlt.analytics._table_reference import TableReference
+from tmlt.analytics.constraints import MaxRowsPerID
+from tmlt.analytics.privacy_budget import (
+    ApproxDPBudget,
+    PrivacyBudget,
+    PureDPBudget,
+    RhoZCDPBudget,
+)
+from tmlt.analytics.protected_change import (
+    AddMaxRows,
+    AddMaxRowsInMaxGroups,
+    AddOneRow,
+    AddRowsWithID,
+)
 from tmlt.analytics.query_builder import QueryBuilder
 from tmlt.analytics.query_expr import PrivateSource, QueryExpr
 from tmlt.analytics.session import Session
 from tmlt.core.domains.collections import DictDomain
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.domains.spark_domains import (
+    SparkDataFrameDomain,
+    SparkIntegerColumnDescriptor,
+    SparkStringColumnDescriptor,
+)
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.interactive_measurements import (
     PrivacyAccountant,
     PrivacyAccountantState,
     SequentialComposition,
     SequentialQueryable,
 )
 from tmlt.core.measures import Measure, PureDP, RhoZCDP
+from tmlt.core.metrics import AddRemoveKeys as CoreAddRemoveKeys
 from tmlt.core.metrics import (
     DictMetric,
     IfGroupedBy,
     Metric,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.transformations.chaining import ChainTT
-from tmlt.core.transformations.dictionary import GetValue
 from tmlt.core.transformations.spark_transformations.partition import PartitionByKeys
 from tmlt.core.utils.exact_number import ExactNumber
 
 from ..conftest import (  # pylint: disable=no-name-in-module
     assert_frame_equal_with_sort,
     create_mock_transformation,
 )
@@ -96,46 +120,85 @@
             "X": ColumnDescriptor(ColumnType.INTEGER, allow_null=True),
         }
     )
     request.cls.sdf_col_types = sdf_col_types
 
     sdf_input_domain = DictDomain(
         {
-            "private": SparkDataFrameDomain(
+            NamedTable("private"): SparkDataFrameDomain(
                 analytics_to_spark_columns_descriptor(Schema(sdf_col_types))
             )
         }
     )
     request.cls.sdf_input_domain = sdf_input_domain
 
     join_df = spark.createDataFrame(
         pd.DataFrame([["0", 0], ["0", 1], ["1", 1], ["1", 2]], columns=["A", "A+B"])
     )
 
     request.cls.join_df = join_df
 
+    join_df_col_types = Schema(
+        {
+            "A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True),
+            "A+B": ColumnDescriptor(ColumnType.INTEGER, allow_null=True),
+        }
+    )
+    request.cls.join_df_col_types = join_df_col_types
+
+    join_df_input_domain = DictDomain(
+        {
+            NamedTable("join_private"): SparkDataFrameDomain(
+                analytics_to_spark_columns_descriptor(Schema(join_df_col_types))
+            )
+        }
+    )
+    request.cls.join_df_input_domain = join_df_input_domain
+
     private_schema = {
         "A": ColumnDescriptor(ColumnType.VARCHAR),
         "B": ColumnDescriptor(ColumnType.INTEGER),
         "X": ColumnDescriptor(ColumnType.INTEGER),
     }
     request.cls.private_schema = private_schema
 
     public_schema = {
         "A": ColumnDescriptor(ColumnType.VARCHAR),
         "A+B": ColumnDescriptor(ColumnType.INTEGER),
     }
 
     request.cls.public_schema = public_schema
 
+    combined_input_domain = DictDomain(
+        {
+            NamedTable("private"): SparkDataFrameDomain(
+                analytics_to_spark_columns_descriptor(Schema(sdf_col_types))
+            ),
+            NamedTable("join_private"): SparkDataFrameDomain(
+                analytics_to_spark_columns_descriptor(Schema(join_df_col_types))
+            ),
+        }
+    )
+    request.cls.combined_input_domain = combined_input_domain
+
 
 @pytest.mark.usefixtures("test_data")
 class TestSession:
     """Tests for :class:`~tmlt.analytics.session.Session`."""
 
+    sdf: DataFrame
+    sdf_col_types: Schema
+    sdf_input_domain: DictDomain
+    join_df: DataFrame
+    join_col_types: Schema
+    join_input_domain: DictDomain
+    private_schema: Dict[str, ColumnDescriptor]
+    public_schema: Dict[str, ColumnDescriptor]
+    combined_input_domain: DictDomain
+
     @pytest.mark.parametrize(
         "budget_value,output_measure,expected_budget",
         [
             pytest.param(ExactNumber(10), PureDP(), PureDPBudget(10), id="puredp"),
             pytest.param(ExactNumber(10), RhoZCDP(), RhoZCDPBudget(10), id="zcdp"),
         ],
     )
@@ -242,55 +305,300 @@
             mock_composition_init.return_value = Mock(
                 spec_set=SequentialComposition,
                 return_value=Mock(spec_set=SequentialComposition),
             )
             mock_composition_init.return_value.privacy_budget = (
                 _privacy_budget_to_exact_number(budget)
             )
-            mock_composition_init.return_value.d_in = {"private": 21}
+            mock_composition_init.return_value.d_in = {NamedTable("private"): 21}
             mock_composition_init.return_value.output_measure = expected_output_measure
 
             Session.from_dataframe(
                 privacy_budget=budget,
                 source_id="private",
                 dataframe=self.sdf,
                 **from_dataframe_args,
             )
 
             mock_composition_init.assert_called_with(
                 input_domain=self.sdf_input_domain,
-                input_metric=DictMetric({"private": expected_metric}),
-                d_in={"private": 21},
+                input_metric=DictMetric({NamedTable("private"): expected_metric}),
+                d_in={NamedTable("private"): 21},
                 privacy_budget=sp.oo,
                 output_measure=expected_output_measure,
             )
             mock_composition_init.return_value.assert_called()
             assert_frame_equal_with_sort(
                 mock_composition_init.return_value.mock_calls[0][1][0][
-                    "private"
+                    NamedTable("private")
                 ].toPandas(),
                 self.sdf.toPandas(),
             )
             mock_session_init.assert_called_with(
                 self=ANY, accountant=ANY, public_sources=dict(), compiler=ANY
             )
 
+    @pytest.mark.parametrize(
+        "budget,expected_output_measure,expected_metric,from_dataframe_args",
+        [
+            pytest.param(
+                PureDPBudget(float("inf")),
+                PureDP(),
+                DictMetric(
+                    {
+                        TableCollection("default_id_space"): CoreAddRemoveKeys(
+                            {NamedTable("private"): "A"}
+                        )
+                    }
+                ),
+                {
+                    "stability": None,
+                    "grouping_column": None,
+                    "protected_change": AddRowsWithID("A"),
+                },
+                id="puredp-addrowswithID-protected_change",
+            )
+        ],
+    )
+    def test_from_dataframe_add_remove_keys(
+        self,
+        budget: Union[PureDPBudget, RhoZCDPBudget],
+        expected_output_measure: Union[PureDP, RhoZCDP],
+        expected_metric: Metric,
+        from_dataframe_args: Dict,
+    ) -> None:
+        """Test Session.from_dataframe for AddRemoveKeys.
+
+        AddRemoveKeys doesn't create a DictMetric because it's special.
+        """
+        with patch(
+            "tmlt.analytics.session.SequentialComposition", autospec=True
+        ) as mock_composition_init, patch.object(
+            Session, "__init__", autospec=True, return_value=None
+        ) as mock_session_init:
+            mock_composition_init.return_value = Mock(
+                spec_set=SequentialComposition,
+                return_value=Mock(spec_set=SequentialComposition),
+            )
+            mock_composition_init.return_value.privacy_budget = (
+                _privacy_budget_to_exact_number(budget)
+            )
+            expected_d_in = {TableCollection("default_id_space"): 1}
+            mock_composition_init.return_value.d_in = expected_d_in
+            mock_composition_init.return_value.output_measure = expected_output_measure
+
+            Session.from_dataframe(
+                privacy_budget=budget,
+                source_id="private",
+                dataframe=self.sdf,
+                **from_dataframe_args,
+            )
+
+            expected_input_domain = DictDomain(
+                {TableCollection("default_id_space"): self.sdf_input_domain}
+            )
+
+            mock_composition_init.assert_called_with(
+                input_domain=expected_input_domain,
+                input_metric=expected_metric,
+                d_in=expected_d_in,
+                privacy_budget=sp.oo,
+                output_measure=expected_output_measure,
+            )
+            mock_composition_init.return_value.assert_called()
+            assert_frame_equal_with_sort(
+                mock_composition_init.return_value.mock_calls[0][1][0][
+                    TableCollection("default_id_space")
+                ][NamedTable("private")].toPandas(),
+                self.sdf.toPandas(),
+            )
+            mock_session_init.assert_called_with(
+                self=ANY, accountant=ANY, public_sources=dict(), compiler=ANY
+            )
+
+    @pytest.mark.parametrize(
+        "budget,relation,expected_metric,expected_output_measure",
+        [
+            pytest.param(
+                PureDPBudget(float("inf")),
+                AddRemoveRows(table="private", n=6),
+                DictMetric(
+                    key_to_metric={NamedTable("private"): SymmetricDifference()}
+                ),
+                PureDP(),
+                id="addremoverows_session",
+            ),
+            pytest.param(
+                PureDPBudget(float("inf")),
+                AddRemoveRowsAcrossGroups(
+                    table="private", grouping_column="X", max_groups=3, per_group=2
+                ),
+                DictMetric(
+                    key_to_metric={
+                        NamedTable("private"): IfGroupedBy(
+                            column="X", inner_metric=SumOf(SymmetricDifference())
+                        )
+                    }
+                ),
+                PureDP(),
+                id="acrossgroupspuredp_session",
+            ),
+            pytest.param(
+                RhoZCDPBudget(float("inf")),
+                AddRemoveRowsAcrossGroups(
+                    table="private", grouping_column="X", max_groups=4, per_group=3
+                ),
+                DictMetric(
+                    key_to_metric={
+                        NamedTable("private"): IfGroupedBy(
+                            column="X",
+                            inner_metric=RootSumOfSquared(SymmetricDifference()),
+                        )
+                    }
+                ),
+                RhoZCDP(),
+                id="acrossgroupsrhozcdp_session",
+            ),
+        ],
+    )
+    def test_from_neighboring_relation_single(
+        self,
+        budget: Union[PureDPBudget, RhoZCDPBudget],
+        relation: NeighboringRelation,
+        expected_metric: DictMetric,
+        expected_output_measure: Union[PureDP, RhoZCDP],
+    ):
+        """Tests that :func:`Session._from_neighboring_relation` works as expected
+        with a single relation.
+        """
+
+        sess = Session._from_neighboring_relation(  # pylint: disable=protected-access
+            privacy_budget=budget,
+            private_sources={"private": self.sdf},
+            relation=relation,
+        )
+        # pylint: disable=protected-access
+        assert sess._input_domain == self.sdf_input_domain
+        assert sess._input_metric == expected_metric
+        assert sess._accountant.d_in == {NamedTable("private"): 6}
+        assert sess._accountant.privacy_budget == sp.oo
+        assert sess._accountant.output_measure == expected_output_measure
+        # pylint: enable=protected-access
+
+    @pytest.mark.parametrize(
+        "budget,relation,expected_metric,expected_output_measure",
+        [
+            pytest.param(
+                PureDPBudget(float("inf")),
+                AddRemoveKeys("private", {"private": "A"}, max_keys=5),
+                DictMetric(
+                    {
+                        TableCollection("private"): CoreAddRemoveKeys(
+                            {NamedTable("private"): "A"}
+                        )
+                    }
+                ),
+                PureDP(),
+                id="addremovekeys_puredp_session",
+            )
+        ],
+    )
+    def test_from_neighboring_relation_add_remove_keys(
+        self,
+        budget: Union[PureDPBudget, RhoZCDPBudget],
+        relation: NeighboringRelation,
+        expected_metric: DictMetric,
+        expected_output_measure: Union[PureDP, RhoZCDP],
+    ):
+        """Tests that :func:`Session._from_neighboring_relation` works as expected
+        with a single AddRemoveKeys relation.
+        """
+
+        sess = Session._from_neighboring_relation(  # pylint: disable=protected-access
+            privacy_budget=budget,
+            private_sources={"private": self.sdf},
+            relation=relation,
+        )
+        # pylint: disable=protected-access
+        assert sess._input_domain == DictDomain(
+            {TableCollection("private"): self.sdf_input_domain}
+        )
+        assert sess._input_metric == expected_metric
+        assert sess._accountant.d_in == {TableCollection("private"): 5}
+        assert sess._accountant.privacy_budget == sp.oo
+        assert sess._accountant.output_measure == expected_output_measure
+        # pylint: enable=protected-access
+
+    @pytest.mark.parametrize(
+        "budget,relation,expected_metric,expected_output_measure",
+        [
+            pytest.param(
+                PureDPBudget(float("inf")),
+                Conjunction(
+                    AddRemoveRows(table="private", n=6),
+                    AddRemoveRowsAcrossGroups(
+                        table="join_private",
+                        grouping_column="A+B",
+                        max_groups=3,
+                        per_group=3,
+                    ),
+                ),
+                DictMetric(
+                    key_to_metric={
+                        NamedTable("join_private"): IfGroupedBy(
+                            column="A+B", inner_metric=SumOf(SymmetricDifference())
+                        ),
+                        NamedTable("private"): SymmetricDifference(),
+                    }
+                ),
+                PureDP(),
+                id="conjunction_session",
+            )
+        ],
+    )
+    def test_from_neighboring_relation_conjunction(
+        self,
+        budget: Union[PureDPBudget, RhoZCDPBudget],
+        relation: NeighboringRelation,
+        expected_metric: DictMetric,
+        expected_output_measure: Union[PureDP, RhoZCDP],
+    ):
+        """Tests that :func:`Session._from_neighboring_relation` works as expected
+        when passed a conjunction.
+        """
+        sess = Session._from_neighboring_relation(  # pylint: disable=protected-access
+            privacy_budget=budget,
+            private_sources={"private": self.sdf, "join_private": self.join_df},
+            relation=relation,
+        )
+
+        # pylint: disable=protected-access
+        assert sess._input_domain == self.combined_input_domain
+        assert sess._input_metric == expected_metric
+        assert sess._accountant.d_in == {
+            NamedTable("private"): 6,
+            NamedTable("join_private"): 9,
+        }
+        assert sess._accountant.privacy_budget == sp.oo
+        assert sess._accountant.output_measure == expected_output_measure
+        # pylint: enable=protected-access
+
     def test_add_public_dataframe(self):
         """Tests that :func:`add_public_dataframe` works correctly."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant, patch(
             "tmlt.analytics.session.QueryExprCompiler"
         ) as mock_compiler:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
-                {"private": SymmetricDifference()}
+                {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = self.sdf_input_domain
-            mock_accountant.d_in = {"private": ExactNumber(1)}
+            mock_accountant.d_in = {NamedTable("private"): ExactNumber(1)}
             mock_compiler.output_measure = PureDP()
             session = Session(
                 accountant=mock_accountant,
                 public_sources=dict(),
                 compiler=mock_compiler,
             )
             session.add_public_dataframe(source_id="public", dataframe=self.join_df)
@@ -314,48 +622,62 @@
         ) as mock_accountant:
             mock_accountant.output_measure = PureDP()
             # Use RootSumOfSquared since SymmetricDifference
             # doesn't allow non-ints. Wrap
             # that in IfGroupedBy since RootSumOfSquared on its own is not valid in many
             # places in the framework.
             mock_accountant.input_metric = DictMetric(
-                {"private": IfGroupedBy("A", RootSumOfSquared(SymmetricDifference()))}
+                {
+                    NamedTable("private"): IfGroupedBy(
+                        "A", RootSumOfSquared(SymmetricDifference())
+                    )
+                }
             )
             mock_accountant.input_domain = self.sdf_input_domain
-            mock_accountant.d_in = {"private": ExactNumber(d_in)}
+            mock_accountant.d_in = {NamedTable("private"): ExactNumber(d_in)}
             view_transformation = create_mock_transformation(
                 input_domain=self.sdf_input_domain,
                 input_metric=DictMetric(
                     {
-                        "private": IfGroupedBy(
+                        NamedTable("private"): IfGroupedBy(
+                            "A", RootSumOfSquared(SymmetricDifference())
+                        )
+                    }
+                ),
+                output_domain=self.sdf_input_domain,
+                output_metric=DictMetric(
+                    {
+                        NamedTable("private"): IfGroupedBy(
                             "A", RootSumOfSquared(SymmetricDifference())
                         )
                     }
                 ),
-                output_domain=self.sdf_input_domain["private"],
-                output_metric=SymmetricDifference(),
                 stability_function_implemented=True,
                 stability_function_return_value=ExactNumber(13),
             )
-            mock_compiler_transform.return_value = view_transformation
-
+            mock_compiler_transform.return_value = (
+                view_transformation,
+                TableReference(path=[NamedTable("private")]),
+                [],
+            )
             session = Session(accountant=mock_accountant, public_sources=dict())
             session.create_view(
                 query_expr=PrivateSource("private"),
                 source_id="identity_transformation",
                 cache=False,
             )
 
             mock_compiler_transform.assert_called_with(
                 self=ANY,
                 query=PrivateSource("private"),
                 input_domain=mock_accountant.input_domain,
                 input_metric=mock_accountant.input_metric,
                 public_sources={},
                 catalog=ANY,
+                table_constraints=ANY,
             )
 
     @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
     def test_evaluate_puredp_session(self, spark, d_in):
         """Tests that :func:`evaluate` calls the right things given a puredp session."""
         with patch.object(
             QueryExprCompiler, "__call__", autospec=True
@@ -372,14 +694,36 @@
             )
             self._assert_test_evaluate_correctness(
                 session, mock_accountant, mock_compiler, 10
             )
             check_type("answer", answer, DataFrame)
 
     @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
+    def test_evaluate_puredp_session_approxdp_query(self, spark, d_in):
+        """Tests that :func:`evaluate` calls the right things given a puredp session."""
+        with patch.object(
+            QueryExprCompiler, "__call__", autospec=True
+        ) as mock_compiler, patch(
+            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
+        ) as mock_accountant:
+            self._setup_accountant_and_compiler(
+                spark, d_in, mock_accountant, mock_compiler
+            )
+            mock_accountant.privacy_budget = ExactNumber(10)
+            session = Session(accountant=mock_accountant, public_sources=dict())
+            answer = session.evaluate(
+                query_expr=PrivateSource("private"),
+                privacy_budget=ApproxDPBudget(10, 0.5),
+            )
+            self._assert_test_evaluate_correctness(
+                session, mock_accountant, mock_compiler, 10
+            )
+            check_type("answer", answer, DataFrame)
+
+    @pytest.mark.parametrize("d_in", [(sp.Integer(1)), (sp.sqrt(sp.Integer(2)))])
     def test_evaluate_with_zero_budget(self, spark, d_in):
         """Confirm that calling evaluate with a 'budget' of 0 fails."""
         with patch.object(
             QueryExprCompiler, "__call__", autospec=True
         ) as mock_compiler, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
@@ -484,38 +828,78 @@
             check_type("answer", answer, DataFrame)
 
     def _setup_accountant(
         self, mock_accountant, d_in=None, privacy_budget=None
     ) -> None:
         """Initialize only a mock accountant."""
         mock_accountant.output_measure = PureDP()
-        mock_accountant.input_metric = DictMetric({"private": SymmetricDifference()})
+        mock_accountant.input_metric = DictMetric(
+            {NamedTable("private"): SymmetricDifference()}
+        )
         mock_accountant.input_domain = self.sdf_input_domain
         if d_in is not None:
-            mock_accountant.d_in = {"private": d_in}
+            mock_accountant.d_in = {NamedTable("private"): d_in}
         else:
-            mock_accountant.d_in = {"private": ExactNumber(1)}
+            mock_accountant.d_in = {NamedTable("private"): ExactNumber(1)}
+        if privacy_budget is not None:
+            mock_accountant.privacy_budget = privacy_budget
+        else:
+            mock_accountant.privacy_budget = ExactNumber(10)
+
+    def _setup_accountant_with_id(self, mock_accountant, privacy_budget=None) -> None:
+        mock_accountant.output_measure = PureDP()
+        mock_accountant.input_metric = DictMetric(
+            key_to_metric={
+                TableCollection(name="identifier_A"): CoreAddRemoveKeys(
+                    df_to_key_column={NamedTable(name="private"): "A"}
+                )
+            }
+        )
+        mock_accountant.input_domain = DictDomain(
+            key_to_domain={
+                TableCollection(name="identifier_A"): DictDomain(
+                    key_to_domain={
+                        NamedTable(name="private"): SparkDataFrameDomain(
+                            schema={
+                                "A": SparkStringColumnDescriptor(allow_null=True),
+                                "B": SparkIntegerColumnDescriptor(
+                                    allow_null=True, size=64
+                                ),
+                                "X": SparkIntegerColumnDescriptor(
+                                    allow_null=True, size=64
+                                ),
+                            }
+                        )
+                    }
+                )
+            }
+        )
+        mock_accountant.d_in = {TableCollection(name="identifier_A"): 1}
         if privacy_budget is not None:
             mock_accountant.privacy_budget = privacy_budget
         else:
             mock_accountant.privacy_budget = ExactNumber(10)
 
     def _setup_accountant_and_compiler(
         self, spark, d_in, mock_accountant, mock_compiler
     ):
         """Initialize the mocks for testing :func:`evaluate`."""
         mock_accountant.output_measure = PureDP()
         # Use RootSumOfSquared since SymmetricDifference doesn't allow non-ints. Wrap
         # that in IfGroupedBy since RootSumOFSquared on its own is not valid in many
         # places in the framework.
         mock_accountant.input_metric = DictMetric(
-            {"private": IfGroupedBy("A", RootSumOfSquared(SymmetricDifference()))}
+            {
+                NamedTable("private"): IfGroupedBy(
+                    "A", RootSumOfSquared(SymmetricDifference())
+                )
+            }
         )
         mock_accountant.input_domain = self.sdf_input_domain
-        mock_accountant.d_in = {"private": d_in}
+        mock_accountant.d_in = {NamedTable("private"): d_in}
         # The accountant's measure method will return a list
         # containing 1 empty dataframe
         mock_accountant.measure.return_value = [
             spark.createDataFrame(spark.sparkContext.emptyRDD(), StructType([]))
         ]
         mock_compiler.output_measure = PureDP()
         mock_compiler.return_value = Mock(spec_set=Measurement)
@@ -532,14 +916,15 @@
             queries=[PrivateSource("private")],
             stability=mock_accountant.d_in,
             input_domain=mock_accountant.input_domain,
             input_metric=mock_accountant.input_metric,
             privacy_budget=sp.Integer(budget),
             public_sources={},
             catalog=ANY,
+            table_constraints={t: [] for t in mock_accountant.d_in.keys()},
         )
 
         mock_accountant.measure.assert_called_with(
             mock_compiler.return_value, d_out=ExactNumber(budget)
         )
 
     def test_partition_and_create(self):
@@ -561,77 +946,40 @@
                     input_domain=self.sdf_input_domain,
                     output_measure=PureDP(),
                 ),
             ]
 
             session = Session(accountant=mock_accountant, public_sources=dict())
 
-        # Test that you need exactly one of column, attr_name
-        with pytest.raises(ValueError, match="Please specify a column"):
-            session.partition_and_create(
-                source_id="private",
-                privacy_budget=PureDPBudget(10),
-                splits={"part0": "0", "part1": "1"},
-            )
-        with pytest.raises(
-            ValueError, match="You cannot specify both a column and an attr_name"
-        ):
-            session.partition_and_create(
-                source_id="private",
-                privacy_budget=PureDPBudget(10),
-                column="A",
-                attr_name="A",
-                splits={"part0": "0", "part1": "1"},
-            )
         # Test that you need to provide splits
         with pytest.raises(
             ValueError,
             match=re.escape(
                 "You must provide a dictionary mapping split names (new source_ids) to"
                 " values on which to partition"
             ),
         ):
             session.partition_and_create(
                 source_id="private", privacy_budget=PureDPBudget(10), column="A"
             )
 
-        # Make a new session so that testing for warnings doesn't
-        # impact the later tests
-        warn_session = Session(accountant=mock_accountant, public_sources=dict())
-        with pytest.warns(DeprecationWarning, match="attr_name argument is deprecated"):
-            warn_session.partition_and_create(
-                source_id="private",
-                privacy_budget=PureDPBudget(10),
-                attr_name="A",
-                splits={"part0": "0", "part1": "1"},
-            )
-
         new_sessions = session.partition_and_create(
             source_id="private",
             privacy_budget=PureDPBudget(10),
             column="A",
             splits={"part0": "0", "part1": "1"},
         )
 
         partition_query = mock_accountant.mock_calls[-1][1][0]
-        assert isinstance(partition_query, Transformation)
         assert isinstance(partition_query, ChainTT)
 
-        assert isinstance(partition_query.transformation1, GetValue)
-        assert (
-            partition_query.transformation1.input_domain == mock_accountant.input_domain
-        )
-        assert (
-            partition_query.transformation1.input_metric == mock_accountant.input_metric
-        )
-        assert partition_query.transformation1.key == "private"
         assert isinstance(partition_query.transformation2, PartitionByKeys)
         assert (
             partition_query.transformation2.input_domain
-            == self.sdf_input_domain["private"]
+            == self.sdf_input_domain[NamedTable("private")]
         )
         assert partition_query.transformation2.input_metric == SymmetricDifference()
         assert partition_query.transformation2.output_metric == SumOf(
             SymmetricDifference()
         )
         assert partition_query.transformation2.keys == ["A"]
         assert partition_query.transformation2.list_values == [("0",), ("1",)]
@@ -641,14 +989,216 @@
         )
 
         assert isinstance(new_sessions, dict)
         for new_session_name, new_session in new_sessions.items():
             assert isinstance(new_session_name, str)
             assert isinstance(new_session, Session)
 
+    def test_describe(self, spark):
+        """Test that :func:`_describe` works correctly."""
+        with patch("builtins.print") as mock_print, patch(
+            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
+        ) as mock_accountant:
+            self._setup_accountant(mock_accountant, privacy_budget=ExactNumber(10))
+            mock_accountant.state = PrivacyAccountantState.ACTIVE
+
+            public_df_1 = spark.createDataFrame(
+                pd.DataFrame([["blah", 1], ["blah", 2]], columns=["A", "B"])
+            )
+            public_df_2 = spark.createDataFrame(
+                pd.DataFrame(
+                    {
+                        "X": [1.1, 2.2, 3.3],
+                        "very_long_column_name": ["blah", "blah", "blah"],
+                    }
+                )
+            )
+            session = Session(
+                accountant=mock_accountant,
+                public_sources={"public1": public_df_1, "public2": public_df_2},
+            )
+            # pylint: disable=line-too-long
+            expected = f"""The session has a remaining privacy budget of {PureDPBudget(10)}.
+The following private tables are available:
+Table 'private' (no constraints):
+\tColumns:
+\t\t- 'A'  VARCHAR
+\t\t- 'B'  INTEGER
+\t\t- 'X'  INTEGER
+The following public tables are available:
+Public table 'public1':
+\tColumns:
+\t\t- 'A'  VARCHAR
+\t\t- 'B'  INTEGER
+Public table 'public2':
+\tColumns:
+\t\t- 'X'                      DECIMAL
+\t\t- 'very_long_column_name'  VARCHAR"""
+            # pylint: enable=line-too-long
+            session.describe()
+            mock_print.assert_called_with(expected)
+
+    def test_describe_with_constraints(self, spark):
+        """Test :func:`_describe` with a table with constraints."""
+        with patch("builtins.print") as mock_print, patch(
+            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
+        ) as mock_accountant:
+            self._setup_accountant(mock_accountant, privacy_budget=ExactNumber(10))
+            mock_accountant.state = PrivacyAccountantState.ACTIVE
+
+            public_df_1 = spark.createDataFrame(
+                pd.DataFrame([["blah", 1], ["blah", 2]], columns=["A", "B"])
+            )
+            public_df_2 = spark.createDataFrame(
+                pd.DataFrame(
+                    {
+                        "X": [1.1, 2.2, 3.3],
+                        "very_long_column_name": ["blah", "blah", "blah"],
+                    }
+                )
+            )
+
+            session = Session(
+                accountant=mock_accountant,
+                public_sources={"public1": public_df_1, "public2": public_df_2},
+            )
+
+            # pylint: disable=protected-access
+            session._table_constraints[NamedTable("private")] = [MaxRowsPerID(5)]
+            # pylint: enable=protected-access
+            # pylint: disable=line-too-long
+            expected = f"""The session has a remaining privacy budget of {PureDPBudget(10)}.
+The following private tables are available:
+Table 'private':
+\tColumns:
+\t\t- 'A'  VARCHAR
+\t\t- 'B'  INTEGER
+\t\t- 'X'  INTEGER
+\tConstraints:
+\t\t- MaxRowsPerID(max=5)
+The following public tables are available:
+Public table 'public1':
+\tColumns:
+\t\t- 'A'  VARCHAR
+\t\t- 'B'  INTEGER
+Public table 'public2':
+\tColumns:
+\t\t- 'X'                      DECIMAL
+\t\t- 'very_long_column_name'  VARCHAR"""
+            session.describe()
+            # pylint: enable=line-too-long
+            mock_print.assert_called_with(expected)
+
+    def test_describe_with_id_column(self, spark):
+        """Test :func:`_describe` with a table with an ID column."""
+
+        with patch("builtins.print") as mock_print, patch(
+            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
+        ) as mock_accountant:
+            self._setup_accountant_with_id(
+                mock_accountant, privacy_budget=ExactNumber(10)
+            )
+            mock_accountant.state = PrivacyAccountantState.ACTIVE
+
+            public_df_1 = spark.createDataFrame(
+                pd.DataFrame([["blah", 1], ["blah", 2]], columns=["A", "B"])
+            )
+            public_df_2 = spark.createDataFrame(
+                pd.DataFrame(
+                    {
+                        "X": [1.1, 2.2, 3.3],
+                        "very_long_column_name": ["blah", "blah", "blah"],
+                    }
+                )
+            )
+
+            session = Session(
+                accountant=mock_accountant,
+                public_sources={"public1": public_df_1, "public2": public_df_2},
+            )
+            # pylint: disable=line-too-long
+            expected = f"""The session has a remaining privacy budget of {PureDPBudget(10)}.
+The following private tables are available:
+Table 'private' (no constraints):
+\tColumns:
+\t\t- 'A'  VARCHAR, ID column (in ID space identifier_A)
+\t\t- 'B'  INTEGER
+\t\t- 'X'  INTEGER
+The following public tables are available:
+Public table 'public1':
+\tColumns:
+\t\t- 'A'  VARCHAR
+\t\t- 'B'  INTEGER
+Public table 'public2':
+\tColumns:
+\t\t- 'X'                      DECIMAL
+\t\t- 'very_long_column_name'  VARCHAR"""
+            # pylint: enable=line-too-long
+            session.describe()
+            mock_print.assert_called_with(expected)
+
+    @pytest.mark.parametrize(
+        "query,expected_output",
+        [
+            pytest.param(
+                "private",
+                """Columns:
+\t- 'A'  VARCHAR
+\t- 'B'  INTEGER
+\t- 'X'  INTEGER""",
+                id="table_name",
+            ),
+            pytest.param(
+                PrivateSource("private"),
+                """Columns:
+\t- 'A'  VARCHAR
+\t- 'B'  INTEGER
+\t- 'X'  INTEGER""",
+                id="private_source_query",
+            ),
+            pytest.param(
+                QueryBuilder("private"),
+                """Columns:
+\t- 'A'  VARCHAR
+\t- 'B'  INTEGER
+\t- 'X'  INTEGER""",
+                id="query_builder_private_source",
+            ),
+            pytest.param(
+                QueryBuilder("private").drop_null_and_nan(["A", "B", "X"]),
+                """Columns:
+\t- 'A'  VARCHAR, not null
+\t- 'B'  INTEGER, not null
+\t- 'X'  INTEGER, not null""",
+                id="query_builder_drop_null",
+            ),
+        ],
+    )
+    def test_describe_query(
+        self, spark, query: Union[str, QueryBuilder, QueryExpr], expected_output: str
+    ):
+        """Test :func:`_describe` with a QueryExpr, QueryBuilder, or table name."""
+        with patch("builtins.print") as mock_print, patch(
+            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
+        ) as mock_accountant:
+            self._setup_accountant(mock_accountant, privacy_budget=ExactNumber(10))
+            mock_accountant.state = PrivacyAccountantState.ACTIVE
+
+            public_df_1 = spark.createDataFrame(
+                pd.DataFrame([["blah", 1], ["blah", 2]], columns=["A", "B"])
+            )
+            public_df_2 = spark.createDataFrame(pd.DataFrame({"X": [1.1, 2.2, 3.3]}))
+            session = Session(
+                accountant=mock_accountant,
+                public_sources={"public1": public_df_1, "public2": public_df_2},
+            )
+
+            session.describe(query)
+            mock_print.assert_called_with(expected_output)
+
     def test_supported_spark_types(self, spark):
         """Session works with supported Spark data types."""
         alltypes_sdf = spark.createDataFrame(
             pd.DataFrame(
                 [[1.2, 3.4, 17, 42, "blah"]], columns=["A", "B", "C", "D", "E"]
             ),
             schema=StructType(
@@ -725,15 +1275,15 @@
                     "This session is no longer active, and no new queries can be"
                     " performed"
                 ),
             ):
                 session.partition_and_create(
                     "private",
                     privacy_budget=PureDPBudget(1),
-                    attr_name="A",
+                    column="A",
                     splits={"part0": 0, "part1": 1},
                 )
 
 
 @pytest.fixture(name="test_data_invalid", scope="class")
 def setup_invalid_session_data(spark, request) -> None:
     """Set up test data for invalid session tests."""
@@ -765,34 +1315,44 @@
     request.cls.schema = schema
 
 
 @pytest.mark.usefixtures("test_data_invalid")
 class TestInvalidSession:
     """Unit tests for invalid session."""
 
-    spark: SparkSession
+    pdf: pd.DataFrame
+    sdf: DataFrame
+    sdf_col_types: Dict[str, ColumnDescriptor]
+    sdf_input_domain: SparkDataFrameDomain
+    schema: Dict[str, ColumnDescriptor]
 
     def _setup_accountant(self, mock_accountant) -> None:
         mock_accountant.output_measure = PureDP()
-        mock_accountant.input_metric = DictMetric({"private": SymmetricDifference()})
-        mock_accountant.input_domain = DictDomain({"private": self.sdf_input_domain})
-        mock_accountant.d_in = {"private": sp.Integer(1)}
+        mock_accountant.input_metric = DictMetric(
+            {NamedTable("private"): SymmetricDifference()}
+        )
+        mock_accountant.input_domain = DictDomain(
+            {NamedTable("private"): self.sdf_input_domain}
+        )
+        mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
 
     def test_invalid_compiler_initialization(self):
         """session errors if compiler is not a QueryExprCompiler."""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             with pytest.raises(
                 TypeError,
                 match=r"type of compiler must be one of "
                 r"\(QueryExprCompiler, NoneType\); got list instead",
             ):
                 self._setup_accountant(mock_accountant)
-                Session(accountant=mock_accountant, public_sources=dict(), compiler=[])
+                Session(
+                    mock_accountant, public_sources=dict(), compiler=[]  # type: ignore
+                )
 
     def test_invalid_dataframe_initialization(self):
         """session raises error on invalid dataframe type"""
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             # Private
@@ -842,23 +1402,22 @@
             # source_id not existent
             with pytest.raises(KeyError):
                 session.get_schema("view")
             with pytest.raises(KeyError):
                 session.get_grouping_column("view")
 
             # public source_id doesn't have a grouping_column
-            source_id = "public"
             with pytest.raises(
                 ValueError,
                 match=(
-                    f"'{source_id}' does not have a grouping column, "
-                    "because it is not a private table."
+                    "Table 'public' is a public table, which cannot "
+                    "have a grouping column."
                 ),
             ):
-                session.get_grouping_column(source_id)
+                session.get_grouping_column("public")
 
     def test_invalid_column_name(self, spark) -> None:
         """Builder raises an error if a column is named "".
 
         Columns named "" (empty string) are not allowed.
         """
         with patch(
@@ -941,14 +1500,30 @@
                 "^Grouping column 'F' is not of a type on which grouping is supported.*"
             ),
         ):
             Session.from_dataframe(
                 PureDPBudget(1), "private", float_df, grouping_column="F"
             )
 
+    def test_invalid_key_column(self) -> None:  # pylint: disable=unused-argument
+        """Builder raises an error if table's key column is not in dataframe."""
+        with pytest.raises(
+            ValueError,
+            match=(
+                "^Key column 'not_a_column' does not exist in the input. Available"
+                " columns: A, B, X$"
+            ),
+        ):
+            Session.from_dataframe(
+                PureDPBudget(1),
+                "private",
+                self.sdf,
+                protected_change=AddRowsWithID("not_a_column", "random_id"),
+            )
+
     @pytest.mark.parametrize(
         "source_id,exception_type,expected_error_msg",
         [
             (2, TypeError, 'type of argument "source_id" must be str; got int instead'),
             ("@str", ValueError, "source_id must be a valid Python identifier."),
         ],
     )
@@ -959,20 +1534,20 @@
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant, patch(
             "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
         ) as mock_compiler:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
-                {"private": SymmetricDifference()}
+                {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
-                {"private": self.sdf_input_domain}
+                {NamedTable("private"): self.sdf_input_domain}
             )
-            mock_accountant.d_in = {"private": sp.Integer(1)}
+            mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             #### from spark dataframe ####
             # Private
             with pytest.raises(exception_type, match=expected_error_msg):
                 Session.from_dataframe(
                     privacy_budget=PureDPBudget(1),
@@ -997,38 +1572,34 @@
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant, patch(
             "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
         ) as mock_compiler:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
-                {"private": SymmetricDifference()}
+                {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
-                {"private": self.sdf_input_domain}
+                {NamedTable("private"): self.sdf_input_domain}
             )
-            mock_accountant.d_in = {"private": sp.Integer(1)}
+            mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             session = Session(
                 accountant=mock_accountant,
                 compiler=mock_compiler,
                 public_sources=dict(),
             )
 
             # This should work
             session.add_public_dataframe("public_df", dataframe=self.sdf)
 
             # But this should not
             with pytest.raises(
-                ValueError,
-                match=(
-                    "This session already has a public source with the source_id"
-                    " public_df"
-                ),
+                ValueError, match="This session already has a table named 'public_df'."
             ):
                 session.add_public_dataframe("public_df", dataframe=self.sdf)
 
     @pytest.mark.parametrize(
         "query_expr", [(["filter private A == 0"]), ([PrivateSource("private")])]
     )
     def test_invalid_queries_evaluate(self, query_expr: Any):
@@ -1036,20 +1607,20 @@
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant, patch(
             "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
         ) as mock_compiler:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
-                {"private": SymmetricDifference()}
+                {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
-                {"private": self.sdf_input_domain}
+                {NamedTable("private"): self.sdf_input_domain}
             )
-            mock_accountant.d_in = {"private": sp.Integer(1)}
+            mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             session = Session(
                 accountant=mock_accountant,
                 public_sources=dict(),
                 compiler=mock_compiler,
             )
@@ -1083,20 +1654,20 @@
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant, patch(
             "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
         ) as mock_compiler:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
-                {"private": SymmetricDifference()}
+                {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
-                {"private": self.sdf_input_domain}
+                {NamedTable("private"): self.sdf_input_domain}
             )
-            mock_accountant.d_in = {"private": sp.Integer(1)}
+            mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             session = Session(
                 accountant=mock_accountant,
                 public_sources=dict(),
                 compiler=mock_compiler,
             )
@@ -1108,20 +1679,20 @@
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant, patch(
             "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
         ) as mock_compiler:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
-                {"private": SymmetricDifference()}
+                {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
-                {"private": self.sdf_input_domain}
+                {NamedTable("private"): self.sdf_input_domain}
             )
-            mock_accountant.d_in = {"private": sp.Integer(1)}
+            mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             mock_compiler.build_transformation.return_value = (
                 Mock(
                     spec_set=Transformation,
                     output_domain=self.sdf_input_domain,
                     output_metric=SymmetricDifference(),
@@ -1160,20 +1731,20 @@
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant, patch(
             "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
         ) as mock_compiler:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
-                {"private": SymmetricDifference()}
+                {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
-                {"private": self.sdf_input_domain}
+                {NamedTable("private"): self.sdf_input_domain}
             )
-            mock_accountant.d_in = {"private": sp.Integer(1)}
+            mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             mock_compiler.build_transformation.return_value = (
                 Mock(
                     spec_set=Transformation,
                     output_domain=self.sdf_input_domain,
                     output_metric=SymmetricDifference(),
@@ -1205,20 +1776,20 @@
         with patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant, patch(
             "tmlt.analytics._query_expr_compiler.QueryExprCompiler"
         ) as mock_compiler:
             mock_accountant.output_measure = PureDP()
             mock_accountant.input_metric = DictMetric(
-                {"private": SymmetricDifference()}
+                {NamedTable("private"): SymmetricDifference()}
             )
             mock_accountant.input_domain = DictDomain(
-                {"private": self.sdf_input_domain}
+                {NamedTable("private"): self.sdf_input_domain}
             )
-            mock_accountant.d_in = {"private": sp.Integer(1)}
+            mock_accountant.d_in = {NamedTable("private"): sp.Integer(1)}
             mock_compiler.output_measure = PureDP()
 
             mock_compiler.build_transformation.return_value = (
                 Mock(
                     spec_set=Transformation,
                     output_domain=self.sdf_input_domain,
                     output_metric=SymmetricDifference(),
@@ -1299,22 +1870,25 @@
 
 
 @pytest.fixture(name="session_builder_data", scope="class")
 def setup_session_build_data(spark, request):
     """Setup for tests."""
     df1 = spark.createDataFrame([(1, 2, "A"), (3, 4, "B")], schema=["A", "B", "C"])
     df2 = spark.createDataFrame([("X", "A"), ("Y", "B"), ("Z", "B")], schema=["K", "C"])
+    df3 = spark.createDataFrame([(1, 1, "A"), (2, 2, "B")], schema=["A", "Y", "Z"])
 
-    request.cls.dataframes = {"df1": df1, "df2": df2}
+    request.cls.dataframes = {"df1": df1, "df2": df2, "df3": df3}
 
 
 @pytest.mark.usefixtures("session_builder_data")
 class TestSessionBuilder:
     """Tests for :class:`~tmlt.analytics.session.Session.Builder`."""
 
+    dataframes: Dict[str, DataFrame]
+
     @pytest.mark.parametrize(
         "builder,error_msg",
         [
             (
                 Session.Builder(),
                 "Privacy budget must be specified.",
             ),  # No Privacy Budget
@@ -1336,14 +1910,49 @@
                 source_id="df1", dataframe=self.dataframes["df1"], stability=0
             )
         with pytest.raises(ValueError, match="Stability must be a positive integer"):
             Session.Builder().with_private_dataframe(
                 source_id="df1", dataframe=self.dataframes["df1"], stability=-1
             )
 
+    @pytest.mark.parametrize(
+        "stability,grouping_column,error_msg",
+        [
+            (None, None, "Using a default for protected_change is deprecated"),
+            (
+                None,
+                "A",
+                "Providing a grouping_column parameter instead of a"
+                " protected_change parameter is deprecated",
+            ),
+            (
+                1,
+                None,
+                "Providing a stability instead of a protected_change is deprecated",
+            ),
+            (
+                1,
+                "A",
+                "Providing a grouping_column parameter instead of a"
+                " protected_change parameter is deprecated",
+            ),
+        ],
+    )
+    def test_stability_deprecation(
+        self, stability: Optional[int], grouping_column: Optional[str], error_msg: str
+    ):
+        """Test that stability and grouping_column give deprecation warnings."""
+        with pytest.warns(DeprecationWarning, match=error_msg):
+            Session.Builder().with_private_dataframe(
+                source_id="df1",
+                dataframe=self.dataframes["df1"],
+                stability=stability,
+                grouping_column=grouping_column,
+            )
+
     @pytest.mark.parametrize("initial_budget", [(PureDPBudget(1)), (RhoZCDPBudget(1))])
     def test_invalid_to_add_budget_twice(self, initial_budget: PrivacyBudget):
         """Test that you can't call ``with_privacy_budget()`` twice."""
         builder = Session.Builder().with_privacy_budget(initial_budget)
         with pytest.raises(
             ValueError, match="This Builder already has a privacy budget"
         ):
@@ -1363,26 +1972,98 @@
                 source_id="A", dataframe=self.dataframes["df2"], stability=2
             )
         with pytest.raises(ValueError, match="Duplicate source id: 'A'"):
             builder.with_public_dataframe(
                 source_id="A", dataframe=self.dataframes["df2"]
             )
 
+    def test_build_invalid_identifier(self):
+        """Tests that build fails if protected change does
+        not have associated ID space."""
+        builder = (
+            Session.Builder()
+            .with_private_dataframe(
+                source_id="A",
+                dataframe=self.dataframes["df1"],
+                protected_change=AddRowsWithID("A", "random_id"),
+            )
+            .with_privacy_budget(PureDPBudget(1))
+        )
+
+        assert len(builder._id_spaces) == 0  # pylint: disable=protected-access
+
+        with pytest.raises(
+            ValueError,
+            match=(
+                "An AddRowsWithID protected change was specified without an "
+                "associated identifier space"
+            ),
+        ):
+            builder.build()
+
+        builder.with_id_space("not_random_id")
+        with pytest.raises(
+            ValueError,
+            match=(
+                "An AddRowsWithID protected change was specified without an "
+                "associated identifier space"
+            ),
+        ):
+            builder.build()
+        ### build should succeed when the identifier space is added
+        builder = builder.with_id_space("random_id")
+        with pytest.raises(ValueError, match="This Builder already has an ID space"):
+            builder.with_id_space("random_id")
+        assert len(builder._id_spaces) == 2  # pylint: disable=protected-access
+        builder.build()
+
+    def test_build_multiple_ids(self):
+        """Tests that build succeeds with multiple ID spaces."""
+        builder = (
+            Session.Builder()
+            .with_private_dataframe(
+                source_id="private1",
+                dataframe=self.dataframes["df1"],
+                protected_change=AddRowsWithID("A", "id_space_1"),
+            )
+            .with_id_space("id_space_1")
+        )
+        builder.with_private_dataframe(
+            source_id="private2",
+            dataframe=self.dataframes["df2"],
+            protected_change=AddRowsWithID("C", "id_space_2"),
+        ).with_id_space("id_space_2")
+
+        builder.with_private_dataframe(
+            source_id="private3",
+            dataframe=self.dataframes["df3"],
+            protected_change=AddRowsWithID("Y", "id_space_1"),
+        )
+
+        builder.with_privacy_budget(PureDPBudget(1)).build()
+
     @pytest.mark.parametrize(
         "builder,expected_sympy_budget,expected_output_measure,"
         + "private_dataframes,public_dataframes",
         [
             (
                 Session.Builder().with_privacy_budget(PureDPBudget(10)),
                 sp.Integer(10),
                 PureDP(),
                 [("df1", 1)],
                 [],
             ),
             (
+                Session.Builder().with_privacy_budget(ApproxDPBudget(10, 0.5)),
+                sp.Integer(10),
+                PureDP(),
+                [("df1", 1)],
+                [],
+            ),
+            (
                 Session.Builder().with_privacy_budget(PureDPBudget(1.5)),
                 sp.Rational("1.5"),
                 PureDP(),
                 [("df1", 1)],
                 [],
             ),
             (
@@ -1406,73 +2087,65 @@
         builder: Session.Builder,
         expected_sympy_budget: sp.Expr,
         expected_output_measure: Measure,
         private_dataframes: List[Tuple[str, int]],
         public_dataframes: List[str],
     ):
         """Tests that building a Session works correctly."""
-        with patch.object(
-            Session, "__init__", autospec=True, return_value=None
-        ) as mock_session_init:
-            # Set up the builder.
-            expected_private_sources, expected_public_sources = dict(), dict()
-            expected_stabilities = dict()
-            for source_id, stability in private_dataframes:
-                builder = builder.with_private_dataframe(
-                    source_id=source_id,
-                    dataframe=self.dataframes[source_id],
-                    protected_change=AddMaxRows(stability),
-                )
-                expected_private_sources[source_id] = self.dataframes[source_id]
-                expected_stabilities[source_id] = stability
+        # Set up the builder.
+        expected_private_sources, expected_public_sources = dict(), dict()
+        expected_stabilities = dict()
+        for source_id, stability in private_dataframes:
+            builder = builder.with_private_dataframe(
+                source_id=source_id,
+                dataframe=self.dataframes[source_id],
+                protected_change=AddMaxRows(stability),
+            )
+            expected_private_sources[NamedTable(source_id)] = self.dataframes[source_id]
+            expected_stabilities[NamedTable(source_id)] = stability
+
+        for source_id in public_dataframes:
+            builder = builder.with_public_dataframe(
+                source_id=source_id, dataframe=self.dataframes[source_id]
+            )
+            expected_public_sources[source_id] = self.dataframes[source_id]
+
+        # Build the session and verify that it worked.
+        session = builder.build()
+        # pylint: disable=protected-access
+        accountant = session._accountant
+        assert isinstance(accountant, PrivacyAccountant)
+        assert (
+            accountant.privacy_budget
+            == expected_sympy_budget
+            == accountant.privacy_budget
+        )
+        assert accountant.output_measure == expected_output_measure
 
-            for source_id in public_dataframes:
-                builder = builder.with_public_dataframe(
-                    source_id=source_id, dataframe=self.dataframes[source_id]
-                )
-                expected_public_sources[source_id] = self.dataframes[source_id]
+        for table_id in expected_private_sources:
+            assert accountant._queryable is not None
+            assert isinstance(accountant._queryable, SequentialQueryable)
+            assert_frame_equal_with_sort(
+                accountant._queryable._data[table_id].toPandas(),
+                expected_private_sources[table_id].toPandas(),
+            )
 
-            # Build the session and verify that it worked.
-            builder.build()
+        assert accountant.d_in == expected_stabilities
+
+        public_sources = session._public_sources
+        assert public_sources.keys() == expected_public_sources.keys()
+        for key in public_sources:
+            assert_frame_equal_with_sort(
+                public_sources[key].toPandas(), expected_public_sources[key].toPandas()
+            )
 
-            session_init_kwargs = mock_session_init.call_args[1]
-            assert all(
-                key in session_init_kwargs
-                for key in ["accountant", "public_sources", "compiler"]
-            )
-            accountant = session_init_kwargs["accountant"]
-            assert isinstance(accountant, PrivacyAccountant)
-            assert (
-                accountant.privacy_budget
-                == expected_sympy_budget
-                == accountant.privacy_budget
-            )
-            assert accountant.output_measure == expected_output_measure
-            for source_id in expected_private_sources:
-                # pylint: disable=protected-access
-                assert accountant._queryable is not None
-                assert isinstance(accountant._queryable, SequentialQueryable)
-                assert_frame_equal_with_sort(
-                    accountant._queryable._data[source_id].toPandas(),
-                    expected_private_sources[source_id].toPandas(),
-                )
-                # pylint: enable=protected-access
-            assert accountant.d_in == expected_stabilities
-
-            public_sources = session_init_kwargs["public_sources"]
-            assert public_sources.keys() == expected_public_sources.keys()
-            for key in public_sources:
-                assert_frame_equal_with_sort(
-                    public_sources[key].toPandas(),
-                    expected_public_sources[key].toPandas(),
-                )
-
-            compiler = session_init_kwargs["compiler"]
-            assert isinstance(compiler, QueryExprCompiler)
-            assert compiler.output_measure == expected_output_measure
+        compiler = session._compiler
+        # pylint: enable=protected-access
+        assert isinstance(compiler, QueryExprCompiler)
+        assert compiler.output_measure == expected_output_measure
 
     @pytest.mark.parametrize("nullable", [(True), (False)])
     def test_builder_with_dataframe_keep_nullable_status(self, spark, nullable: bool):
         """with_dataframe methods use the nullable status of the dataframe."""
         builder = Session.Builder()
         builder = builder.with_private_dataframe(
             source_id="private_df",
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_truncation_strategy.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_truncation_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for TruncationStrategy."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # pylint: disable=pointless-string-statement
 
 import pytest
 
 from tmlt.analytics.truncation_strategy import TruncationStrategy
```

### Comparing `tmlt_analytics-0.6.1/test/unit/test_utils.py` & `tmlt_analytics-0.7.0rc1/test/unit/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Unit tests for :mod:`~tmlt.analytics.utils`."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 from tmlt.analytics.utils import check_installation
 
 
 ### Test for tmlt.analytics.utils.check_installation()
 # We want the `spark` argument here so that the test will use the
 # (session-wide, pytest-provided) spark session.
 def test_check_installation(spark) -> None:  # pylint: disable=unused-argument
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/_coerce_spark_schema.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_coerce_spark_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Logic for coercing Spark dataframes into forms usable by Tumult Analytics."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 from typing import Dict
 
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import (
     DataType,
     DateType,
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/_neighboring_relation_visitor.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation_visitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,135 +1,158 @@
 """Module to define NeighboringRelationVisitors."""
-from typing import Any, Dict, Tuple, Union
+
+# SPDX-License-Identifier: Apache-2.0
+# Copyright Tumult Labs 2022
+
+from typing import Any, Dict, NamedTuple, Union
 
 import sympy as sp
 from pyspark.sql import DataFrame
 
-from tmlt.analytics._neighboring_relations import (
+from tmlt.analytics._neighboring_relation import (
+    AddRemoveKeys,
     AddRemoveRows,
     AddRemoveRowsAcrossGroups,
     Conjunction,
     NeighboringRelationVisitor,
 )
+from tmlt.analytics._table_identifier import Identifier, NamedTable, TableCollection
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain
-from tmlt.core.measures import PureDP, RhoZCDP
+from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
+from tmlt.core.metrics import AddRemoveKeys as CoreAddRemoveKeys
 from tmlt.core.metrics import (
     DictMetric,
     IfGroupedBy,
     Metric,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
 from tmlt.core.utils.exact_number import ExactNumber
 
 
+class _RelationIDVisitor(NeighboringRelationVisitor):
+    """Generate identifiers for neighboring relations."""
+
+    def visit_add_remove_rows(self, relation: AddRemoveRows) -> Identifier:
+        return NamedTable(relation.table)
+
+    def visit_add_remove_rows_across_groups(
+        self, relation: AddRemoveRowsAcrossGroups
+    ) -> Identifier:
+        return NamedTable(relation.table)
+
+    def visit_str(self, s: str) -> Identifier:  # pylint: disable=no-self-use
+        """Visit a string.
+
+        Helper method for relations like AddRemoveKeys that need to get
+        identifiers from strings.
+        """
+        return NamedTable(s)
+
+    def visit_add_remove_keys(self, relation: AddRemoveKeys) -> Identifier:
+        return TableCollection(relation.id_space)
+
+    def visit_conjunction(self, relation: Conjunction) -> Identifier:
+        # Since conjunctions are automatically flattened, they should never need names.
+        raise AssertionError(
+            "Conjunctions should never appear as sub-relations. "
+            "This is a bug, please let us know so we can fix it!"
+        )
+
+
 class NeighboringRelationCoreVisitor(NeighboringRelationVisitor):
-    """Defines a Neighboring Relation Core Visitor."""
+    """A visitor for generating an initial Core state from a neighboring relation."""
+
+    class Output(NamedTuple):
+        """A container for the outputs of the visitor."""
+
+        domain: Domain
+        metric: Metric
+        distance: Any
+        data: Any
 
     def __init__(
         self, tables: Dict[str, DataFrame], output_measure: Union[PureDP, RhoZCDP]
     ):
         """Constructor."""
         self.tables = tables
         self.output_measure = output_measure
 
-    def visit_add_remove_rows(
-        self, relation: AddRemoveRows
-    ) -> Tuple[Domain, Metric, Any, Any]:
-        """Returns an input domain, input metric, distance, and input data.
-
-        Relation:
-        :class:`~tmlt.analytics._neighboring_relations.AddRemoveRows`
-        NeighboringRelation.
-        """
-        input_metric = SymmetricDifference()
+    def visit_add_remove_rows(self, relation: AddRemoveRows) -> Output:
+        """Build Core state from ``AddRemoveRows`` neighboring relation."""
+        metric = SymmetricDifference()
         distance = ExactNumber(relation.n)
-        input_table = self.tables[relation.table]
-        # convert table data to domain schema
-        input_domain = SparkDataFrameDomain.from_spark_schema(input_table.schema)
-        return input_domain, input_metric, distance, input_table
+        data = self.tables[relation.table]
+        domain = SparkDataFrameDomain.from_spark_schema(data.schema)
+        return self.Output(domain, metric, distance, data)
 
     def visit_add_remove_rows_across_groups(
         self, relation: AddRemoveRowsAcrossGroups
-    ) -> Tuple[Domain, Metric, Any, Any]:
-        """Returns an input domain, input metric, distance, and input data.
-
-        Relation:
-        :class:`~tmlt.analytics._neighboring_relations.AddRemoveRowsAcrossGroups`
-        NeighboringRelation.
-        """
+    ) -> Output:
+        """Build Core state from ``AddRemoveRowsAcrossGroups`` neighboring relation."""
         # This is needed because it's currently allowed to pass float-valued
         # stabilities in the per_group parameter (for backwards compatibility).
         # TODO(#2272): Remove this.
         per_group = (
             sp.Rational(relation.per_group)
             if isinstance(relation.per_group, float)
             else relation.per_group
         )
         agg_metric: Union[RootSumOfSquared, SumOf]
         if isinstance(self.output_measure, RhoZCDP):
             agg_metric = RootSumOfSquared(SymmetricDifference())
             distance = ExactNumber(
                 per_group * ExactNumber(sp.sqrt(relation.max_groups))
             )
-        elif isinstance(self.output_measure, PureDP):
+        elif isinstance(self.output_measure, (PureDP, ApproxDP)):
             agg_metric = SumOf(SymmetricDifference())
             distance = ExactNumber(per_group * relation.max_groups)
         else:
             raise TypeError(
                 f"The provided output measure {self.output_measure} for this visitor is"
                 " not supported."
             )
 
-        input_metric = IfGroupedBy(relation.grouping_column, agg_metric)
-        input_table = self.tables[relation.table]
-        input_domain = SparkDataFrameDomain.from_spark_schema(input_table.schema)
-        return input_domain, input_metric, distance, input_table
-
-    def visit_conjunction(
-        self, relation: Conjunction
-    ) -> Tuple[Domain, Metric, Any, Any]:
-        """Returns an input domain, input metric, distance, and input data.
-
-        Relation:
-        :class:`~tmlt.analytics._neighboring_relations.Conjunction`
-        NeighboringRelation.
-        """
-        domain_dict: Dict[Union[str, int], Any] = {}
-        # map names of children to their child domain
-        metric_dict: Dict[Union[str, int], Any] = {}
-        # map child names to child input metrics
-        distance_dict: Dict[Union[str, int], Any] = {}
-        # map child names to child input distances
-        input_table_dict: Dict[Union[str, int], Any] = {}
-        # map child names to inputs for their respective relations
-        # Assign numerical indices here instead of using table names
-        # because some indices will be table names, whereas others will be
-        # dictionaries mapping table names to DataFrames (e.g. with AddRemoveKeys)
-        # in the future.
-        for index, child in enumerate(relation.children, 1):
-            child_visitor = child.accept(self)
-            # if the child returns a SparkDataFrameDomain,
-            # we know we can use the table name as index
-            if isinstance(child_visitor[0], SparkDataFrameDomain):
-                source_id = "".join(
-                    child._validate(self.tables)  # pylint: disable=protected-access
-                )
-                domain_dict[source_id] = child_visitor[0]
-                metric_dict[source_id] = child_visitor[1]
-                distance_dict[source_id] = child_visitor[2]
-                input_table_dict[source_id] = child_visitor[3]
-            # otherwise we should use a numerical index
-            else:
-                domain_dict[index] = child_visitor[0]
-                metric_dict[index] = child_visitor[1]
-                distance_dict[index] = child_visitor[2]
-                input_table_dict[index] = child_visitor[3]
-        distance = distance_dict
-        input_metric = DictMetric(metric_dict)
-        input_table = input_table_dict
-        input_domain = DictDomain(domain_dict)
+        metric = IfGroupedBy(relation.grouping_column, agg_metric)
+        data = self.tables[relation.table]
+        domain = SparkDataFrameDomain.from_spark_schema(data.schema)
+        return self.Output(domain, metric, distance, data)
+
+    def visit_add_remove_keys(self, relation: AddRemoveKeys) -> Output:
+        """Build Core state from ``AddRemoveKeys`` neighboring relation."""
+        distance = ExactNumber(relation.max_keys)
+        metric_dict: Dict[Identifier, str] = {}
+        data_dict: Dict[Identifier, Any] = {}
+        domain_dict: Dict[Identifier, Any] = {}
+        for table_name, key_column in relation.table_to_key_column.items():
+            table_id = _RelationIDVisitor().visit_str(table_name)
+            data = self.tables[table_name]
+            domain_dict[table_id] = SparkDataFrameDomain.from_spark_schema(data.schema)
+            metric_dict[table_id] = key_column
+            data_dict[table_id] = data
+
+        return self.Output(
+            DictDomain(domain_dict), CoreAddRemoveKeys(metric_dict), distance, data_dict
+        )
+
+    def visit_conjunction(self, relation: Conjunction) -> Output:
+        """Build Core state from ``Conjunction`` neighboring relation."""
+        domain_dict: Dict[Identifier, Any] = {}
+        metric_dict: Dict[Identifier, Any] = {}
+        distance_dict: Dict[Identifier, Any] = {}
+        data_dict: Dict[Identifier, Any] = {}
+
+        for child in relation.children:
+            child_id = child.accept(_RelationIDVisitor())
+            child_output = child.accept(self)
+
+            domain_dict[child_id] = child_output.domain
+            metric_dict[child_id] = child_output.metric
+            distance_dict[child_id] = child_output.distance
+            data_dict[child_id] = child_output.data
 
-        return input_domain, input_metric, distance, input_table
+        return self.Output(
+            DictDomain(domain_dict), DictMetric(metric_dict), distance_dict, data_dict
+        )
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/_neighboring_relations.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_neighboring_relation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module containing supported variants of neighboring relations."""
 # pylint: disable=useless-super-delegation, protected-access, no-self-use
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 
 from pyspark.sql import DataFrame
 from pyspark.sql.types import DateType, IntegerType, LongType, StringType
 from typeguard import check_type
 
 from tmlt.analytics._coerce_spark_schema import coerce_spark_schema_or_fail
 
@@ -50,15 +50,15 @@
     Two tables are considered neighbors under this relation if
     they differ by at most n rows.
     """
 
     table: str
     """The name of the table in this relation."""
     n: int = field(default=1)
-    """The max number of rows wich may be differ for two instances of the table to
+    """The max number of rows which may be differ for two instances of the table to
      be neighbors.
      """
 
     def __post_init__(self) -> None:
         """Checks arguments to constructor."""
         check_type("source_id", self.table, str)
         check_type("n", self.n, int)
@@ -185,14 +185,115 @@
         return [self.table]
 
     def accept(self, visitor: "NeighboringRelationVisitor") -> Any:
         """Visit this NeighboringRelation with a Visitor."""
         return visitor.visit_add_remove_rows_across_groups(self)
 
 
+@dataclass(frozen=True)
+class AddRemoveKeys(NeighboringRelation):
+    """A relation of tables differing by a certain number of keys.
+
+    Two tables are considered neighbors under this definition if they
+    differ only by the addition/removal of all rows with max_keys distinct values under
+    the columns indicated.
+
+    Note that AddRemoveKeys is a neighboring relation that covers *multiple*
+    tables.
+    """
+
+    id_space: str
+    """The identifier space protected in the relation."""
+    table_to_key_column: Dict[str, str]
+    """A dictionary mapping table names to key columns."""
+    max_keys: int = field(default=1)
+    """The maximum number of keys which may differ for two instances of the table
+    to be neighbors.
+    """
+
+    def __post_init__(self) -> None:
+        """Checks arguments to constructor."""
+        check_type("id_space", self.id_space, str)
+        check_type("table_to_key_column", self.table_to_key_column, Dict[str, str])
+        check_type("max_keys", self.max_keys, int)
+        if self.id_space == "":
+            raise ValueError("id space must be non-empty")
+        if len(self.table_to_key_column) == 0:
+            raise ValueError("table_to_key_column must contain at least one table")
+        if self.max_keys < 1:
+            raise ValueError("max_keys must be positive")
+
+    def validate_input(self, dfs: Dict[str, DataFrame]) -> bool:
+        """Does nothing if input is valid, otherwise raises an informative exception.
+
+        Used only for top-level validation.
+        """
+        self._validate(dfs)
+        return True
+
+    def _validate(self, dfs: Dict[str, DataFrame]) -> List[str]:
+        """Private validation checks.
+
+        These are the validation checks to be done in all cases
+        (regardless of whether the relation is top level).
+        """
+        # checks needed here:
+        # - input type
+        check_type("dfs", dfs, Dict[str, DataFrame])
+        # - all tables present in table_to_key_column are in the input tables
+        difference = set(self.table_to_key_column.keys()).difference(set(dfs.keys()))
+        if difference:
+            raise ValueError(
+                "It appears that the list of input tables doesn't contain some of the"
+                " tables used in the relation. Tables that appear only in the relation:"
+                f" {difference}"
+            )
+        allowed_types = [LongType(), StringType(), DateType()]
+        key_type: Optional[Union[LongType, StringType, DateType]] = None
+        for table_name, df in dfs.items():
+            # check that each table has the requisite column
+            # and that the column is the requisite type
+            if table_name in self.table_to_key_column:
+                key_column = self.table_to_key_column[table_name]
+                if key_column not in df.columns:
+                    raise ValueError(
+                        f"Key column '{key_column}' does not exist in the input."
+                        f" Available columns: {', '.join(df.columns)}"
+                    )
+                coerced_df = coerce_spark_schema_or_fail(df)
+                for df_field in coerced_df.schema:
+                    if not df_field.name == key_column:
+                        continue
+                    if df_field.dataType not in allowed_types:
+                        raise ValueError(
+                            f"Key column '{key_column}' is not of a type allowed for"
+                            " keys. Supported types are: LongType(),"
+                            " StringType(), DateType(), IntegerType()."
+                        )
+                    if key_type is None:
+                        assert isinstance(
+                            df_field.dataType, (LongType, StringType, DateType)
+                        )
+                        key_type = df_field.dataType
+                    else:
+                        if not df_field.dataType == key_type:
+                            raise ValueError(
+                                f"Key column '{key_column}' has type "
+                                f"{df_field.dataType}, but in another"
+                                f" table it has type {key_type}. Key types"
+                                " must match across tables"
+                            )
+
+        return list(self.table_to_key_column.keys())
+
+    def accept(self, visitor: "NeighboringRelationVisitor") -> Any:
+        """Visit this NeighboringRelation with a Visitor."""
+        return visitor.visit_add_remove_keys(self)
+
+
 @dataclass(init=False, frozen=True)
 class Conjunction(NeighboringRelation):
     """A conjunction composed of other neighboring relations."""
 
     children: List[NeighboringRelation]
     """Other neighboring relations to build the Conjunction.
      Args can be provided as a single list or as separate arguments.
@@ -204,14 +305,17 @@
         """Constructor."""
         # flatten the (potentially) nested list
         # since frozen is set to True, we need to subvert it to flatten.
         if isinstance(children[0], list):
             object.__setattr__(self, "children", self._flatten(children[0]))
         else:
             object.__setattr__(self, "children", self._flatten(list(children)))
+        # post_init is not automatically called if a dataclass has
+        # init=False in its decorator
+        self.__post_init__()
 
     def __post_init__(self):
         """Checks arguments to constructor."""
         check_type("children", self.children, List[NeighboringRelation])
 
     def validate_input(self, dfs: Dict[str, DataFrame]) -> bool:
         """Does nothing if input is valid, otherwise raises an informative exception."""
@@ -278,9 +382,13 @@
     @abstractmethod
     def visit_add_remove_rows_across_groups(
         self, relation: AddRemoveRowsAcrossGroups
     ) -> Any:
         """Visit a :class:`AddRemoveRowsAcrossGroups`."""
 
     @abstractmethod
+    def visit_add_remove_keys(self, relation: AddRemoveKeys) -> Any:
+        """Visit a :class:`AddRemoveKeys`."""
+
+    @abstractmethod
     def visit_conjunction(self, relation: Conjunction) -> Any:
         """Visit a :class:`Conjunction`."""
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/_noise_info.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_noise_info.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_privacy_budget_rounding_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Helper functions for dealing with budget floating point imprecision."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 from typing import Union
 
 import sympy as sp
 from typeguard import typechecked
 
 from tmlt.core.utils.exact_number import ExactNumber
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/_query_expr_compiler/_compiler.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_compiler.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,33 @@
 """  # pylint: disable=line-too-long
 # TODO(#746): Check for UnaryExpr.
 # TODO(#1044): Put the PureDPToZCDP converter directly on Vector measurements.
 # TODO(#1547): Associate metric with output measure instead of algorithm for
 #              adding noise.
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
-from typing import Dict, List, Sequence, Union
+from typing import Any, Dict, List, Sequence, Tuple, Union
 
 import sympy as sp
 from pyspark.sql import DataFrame
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler._measurement_visitor import MeasurementVisitor
 from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
     OutputSchemaVisitor,
 )
 from tmlt.analytics._query_expr_compiler._transformation_visitor import (
     TransformationVisitor,
 )
+from tmlt.analytics._schema import Schema
+from tmlt.analytics._table_identifier import Identifier
+from tmlt.analytics._table_reference import TableReference
+from tmlt.analytics.constraints import Constraint
 from tmlt.analytics.query_expr import QueryExpr
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.measurements.aggregations import NoiseMechanism as CoreNoiseMechanism
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.composition import Composition
 from tmlt.core.measures import PureDP, RhoZCDP
 from tmlt.core.metrics import DictMetric
@@ -97,34 +101,48 @@
         self._mechanism = value
 
     @property
     def output_measure(self) -> Union[PureDP, RhoZCDP]:
         """Return the distance measure for the measurement's output."""
         return self._output_measure
 
+    @staticmethod
+    def query_schema(query: QueryExpr, catalog: Catalog) -> Schema:
+        """Return the schema created by a given query."""
+        result = query.accept(OutputSchemaVisitor(catalog=catalog))
+        assert isinstance(result, Schema), (
+            f"schema for this query is not a Schema but is instead a(n) {type(result)}."
+            " This is probably a bug; please let us know about it so we can fix it!"
+        )
+        return result
+
+    # pylint: enable=no-self-use
+
     def __call__(
         self,
         queries: Sequence[QueryExpr],
         privacy_budget: sp.Expr,
-        stability: Dict[str, sp.Expr],
+        stability: Any,
         input_domain: DictDomain,
         input_metric: DictMetric,
         public_sources: Dict[str, DataFrame],
         catalog: Catalog,
+        table_constraints: Dict[Identifier, List[Constraint]],
     ) -> Measurement:
         """Returns a compiled DP measurement.
 
         Args:
             queries: Queries representing measurements to compile.
             privacy_budget: The total privacy budget for answering the queries.
             stability: The stability of the input to compiled query.
             input_domain: The input domain of the compiled query.
             input_metric: The input metric of the compiled query.
             public_sources: Public data sources for the queries.
             catalog: The catalog, used only for query validation.
+            table_constraints: A mapping of tables to the existing constraints on them.
         """
         if len(queries) == 0:
             raise ValueError("At least one query needs to be provided")
 
         measurements: List[Measurement] = []
         per_query_privacy_budget = privacy_budget / len(queries)
         visitor = MeasurementVisitor(
@@ -132,14 +150,15 @@
             stability=stability,
             input_domain=input_domain,
             input_metric=input_metric,
             output_measure=self._output_measure,
             default_mechanism=self._mechanism,
             public_sources=public_sources,
             catalog=catalog,
+            table_constraints=table_constraints,
         )
         for query in queries:
             query_measurement = query.accept(visitor)
             if not isinstance(query_measurement, Measurement):
                 raise AssertionError(
                     "This query did not create a measurement. "
                     "This is probably a bug; please let us know so we can fix it!"
@@ -167,16 +186,17 @@
     def build_transformation(
         self,
         query: QueryExpr,
         input_domain: DictDomain,
         input_metric: DictMetric,
         public_sources: Dict[str, DataFrame],
         catalog: Catalog,
-    ) -> Transformation:
-        r"""Returns a transformation for the query.
+        table_constraints: Dict[Identifier, List[Constraint]],
+    ) -> Tuple[Transformation, TableReference, List[Constraint]]:
+        r"""Returns a transformation and reference for the query.
 
         Supported
         :class:`~tmlt.analytics.query_expr.QueryExpr`\ s:
 
         * :class:`~tmlt.analytics.query_expr.Filter`
         * :class:`~tmlt.analytics.query_expr.FlatMap`
         * :class:`~tmlt.analytics.query_expr.JoinPrivate`
@@ -188,24 +208,28 @@
 
         Args:
             query: A query representing a transformation to compile.
             input_domain: The input domain of the compiled query.
             input_metric: The input metric of the compiled query.
             public_sources: Public data sources for the queries.
             catalog: The catalog, used only for query validation.
+            table_constraints: A mapping of tables to the existing constraints on them.
         """
         query.accept(OutputSchemaVisitor(catalog))
 
         transformation_visitor = TransformationVisitor(
             input_domain=input_domain,
             input_metric=input_metric,
             mechanism=self.mechanism,
             public_sources=public_sources,
+            table_constraints=table_constraints,
         )
-        transformation = query.accept(transformation_visitor)
+        transformation, reference, constraints = query.accept(transformation_visitor)
         if not isinstance(transformation, Transformation):
             raise AssertionError(
                 "Unable to create transformation. This is probably "
                 "a bug; please let us know about it so we can fix it!"
             )
-        transformation_visitor.validate_transformation(query, transformation, catalog)
-        return transformation
+        transformation_visitor.validate_transformation(
+            query, transformation, reference, catalog
+        )
+        return transformation, reference, constraints
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Defines a visitor for creating noisy measurements from query expressions."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 import dataclasses
+import math
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import sympy as sp
 from pyspark.sql import DataFrame
 
 from tmlt.analytics._catalog import Catalog
 from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
@@ -17,40 +18,39 @@
     TransformationVisitor,
 )
 from tmlt.analytics._schema import (
     ColumnType,
     Schema,
     analytics_to_spark_columns_descriptor,
 )
+from tmlt.analytics._table_identifier import Identifier
+from tmlt.analytics._table_reference import TableReference
+from tmlt.analytics._transformation_utils import get_table_from_ref
+from tmlt.analytics.constraints import (
+    Constraint,
+    MaxGroupsPerID,
+    MaxRowsPerGroupPerID,
+    MaxRowsPerID,
+)
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountDistinctMechanism,
     CountMechanism,
-    DropInfinity,
     DropNullAndNan,
-    Filter,
-    FlatMap,
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
     GroupByBoundedSum,
     GroupByBoundedVariance,
     GroupByCount,
     GroupByCountDistinct,
     GroupByQuantile,
-    JoinPrivate,
-    JoinPublic,
-    Map,
-    PrivateSource,
     QueryExpr,
     QueryExprVisitor,
-    Rename,
     ReplaceInfinity,
-    ReplaceNullAndNan,
-    Select,
     StdevMechanism,
     SumMechanism,
     VarianceMechanism,
 )
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import (
     SparkColumnDescriptor,
@@ -74,14 +74,17 @@
     DictMetric,
     HammingDistance,
     IfGroupedBy,
     SymmetricDifference,
 )
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.transformations.spark_transformations.groupby import GroupBy
+from tmlt.core.transformations.spark_transformations.select import (
+    Select as SelectTransformation,
+)
 from tmlt.core.utils.exact_number import ExactNumber
 
 
 def _get_query_bounds(
     query: Union[
         GroupByBoundedAverage,
         GroupByBoundedSTDEV,
@@ -95,72 +98,175 @@
         bound = ExactNumber.from_float(query.high, round_up=True)
         return (bound, bound)
     lower_ceiling = ExactNumber.from_float(query.low, round_up=True)
     upper_floor = ExactNumber.from_float(query.high, round_up=False)
     return (lower_ceiling, upper_floor)
 
 
+def _get_truncatable_constraints(
+    constraints: List[Constraint],
+) -> List[Tuple[Constraint, ...]]:
+    """Get sets of constraints that produce a finite aggregation stability."""
+    # Because of constraint simplification, there should be at most one
+    # MaxRowsPerID constraint, and at most one MaxGroupsPerID and
+    # MaxRowsPerGroupPerID each per column.
+    max_rows_per_id = next(
+        (c for c in constraints if isinstance(c, MaxRowsPerID)), None
+    )
+    max_groups_per_id = {
+        c.grouping_column: c for c in constraints if isinstance(c, MaxGroupsPerID)
+    }
+    max_rows_per_group_per_id = {
+        c.grouping_column: c for c in constraints if isinstance(c, MaxRowsPerGroupPerID)
+    }
+
+    ret: List[Tuple[Constraint, ...]] = [
+        (max_groups_per_id[col], max_rows_per_group_per_id[col])
+        for col in set(max_groups_per_id) & set(max_rows_per_group_per_id)
+    ]
+    if max_rows_per_id:
+        ret.append((max_rows_per_id,))
+    return ret
+
+
+def _constraint_stability(
+    constraints: Tuple[Constraint, ...],
+    output_measure: Union[PureDP, RhoZCDP],
+    grouping_columns: List[str],
+) -> float:
+    """Compute the transformation stability of applying the given constraints.
+
+    The values produced by this method are not intended for use doing actual
+    stability calculations, they are just to provide an easy way to evaluate the
+    relative stabilities of different possible truncations.
+    """
+    if len(constraints) == 1 and isinstance(constraints[0], MaxRowsPerID):
+        return constraints[0].max
+    elif (
+        len(constraints) == 2
+        and isinstance(constraints[0], MaxGroupsPerID)
+        and isinstance(constraints[1], MaxRowsPerGroupPerID)
+    ):
+        if (
+            output_measure == PureDP()
+            or constraints[0].grouping_column not in grouping_columns
+        ):
+            return constraints[0].max * constraints[1].max
+        elif output_measure == RhoZCDP():
+            return math.sqrt(constraints[0].max) * constraints[1].max
+        else:
+            raise AssertionError(
+                f"Unknown output measure {output_measure}. "
+                "This is probably a bug; please let us know about it so we can fix it!"
+            )
+    else:
+        raise AssertionError(
+            f"Constraints {constraints} are not a combination for which a stability "
+            "can be computed. This is probably a bug; please let us know about it "
+            "so we can fix it!"
+        )
+
+
 class MeasurementVisitor(QueryExprVisitor):
     """A visitor to create a measurement from a query expression."""
 
     def __init__(
         self,
         per_query_privacy_budget: sp.Expr,
-        stability: Dict[str, sp.Expr],
+        stability: Any,
         input_domain: DictDomain,
         input_metric: DictMetric,
         output_measure: Union[PureDP, RhoZCDP],
         default_mechanism: NoiseMechanism,
         public_sources: Dict[str, DataFrame],
         catalog: Catalog,
+        table_constraints: Dict[Identifier, List[Constraint]],
     ):
         """Constructor for MeasurementVisitor."""
         self.budget = per_query_privacy_budget
         self.stability = stability
         self.input_domain = input_domain
         self.input_metric = input_metric
         self.default_mechanism = default_mechanism
         self.public_sources = public_sources
         self.output_measure = output_measure
         self.catalog = catalog
+        self.table_constraints = table_constraints
 
     def _visit_child_transformation(
         self, expr: QueryExpr, mechanism: NoiseMechanism
-    ) -> Transformation:
+    ) -> Tuple[Transformation, TableReference, List[Constraint]]:
         """Visit a child transformation, producing a transformation."""
         tv = TransformationVisitor(
             input_domain=self.input_domain,
             input_metric=self.input_metric,
             mechanism=mechanism,
             public_sources=self.public_sources,
+            table_constraints=self.table_constraints,
         )
-        transformation = expr.accept(tv)
-        if not isinstance(transformation, Transformation):
-            raise AssertionError(
-                "Expression failed to produce a transformation. "
-                "This is probably a bug; please let us know about it "
-                "so we can fix it!"
-            )
-        tv.validate_transformation(expr, transformation, self.catalog)
+        child, reference, constraints = expr.accept(tv)
 
-        if not isinstance(
-            transformation.output_metric,
-            (SymmetricDifference, HammingDistance, IfGroupedBy),
+        tv.validate_transformation(expr, child, reference, self.catalog)
+
+        return child, reference, constraints
+
+    def _truncate_table(
+        self,
+        transformation: Transformation,
+        reference: TableReference,
+        constraints: List[Constraint],
+        grouping_columns: List[str],
+    ) -> Tuple[Transformation, TableReference]:
+        table_transformation = get_table_from_ref(transformation, reference)
+        table_metric = table_transformation.output_metric
+        if (
+            isinstance(table_metric, IfGroupedBy)
+            and table_metric.inner_metric == SymmetricDifference()
         ):
-            raise AssertionError(
-                "Unrecognized output metric. This is probably a bug; "
-                "please let us know about it so we can fix it!"
-            )
-        if not isinstance(transformation.output_domain, SparkDataFrameDomain):
-            raise AssertionError(
-                "Unrecognized output domain. This is probably a bug; "
-                "please let us know about it so we can fix it!"
+            truncatable_constraints = _get_truncatable_constraints(constraints)
+            truncatable_constraints.sort(
+                key=lambda cs: _constraint_stability(
+                    cs, self.output_measure, grouping_columns
+                )
             )
+            if not truncatable_constraints:
+                raise RuntimeError(
+                    "A constraint on the number of rows contributed by each ID "
+                    "is needed to perform this query (e.g. MaxRowsPerID)."
+                )
+
+            for c in truncatable_constraints[0]:
+                assert isinstance(
+                    c, (MaxRowsPerID, MaxGroupsPerID, MaxRowsPerGroupPerID)
+                )
+                if isinstance(c, MaxGroupsPerID):
+                    # Taking advantage of the L2 noise behavior only works for
+                    # RhoZCDP Sessions, and then only when the grouping column
+                    # of the constraints is being grouped on.
+                    use_l2 = (
+                        isinstance(self.output_measure, RhoZCDP)
+                        and c.grouping_column in grouping_columns
+                    )
+                    # pylint: disable=protected-access
+                    transformation, reference = c._enforce(
+                        transformation, reference, update_metric=True, use_l2=use_l2
+                    )
+                    # pylint: enable=protected-access
+                else:
+                    (
+                        transformation,
+                        reference,
+                    ) = c._enforce(  # pylint: disable=protected-access
+                        transformation, reference, update_metric=True
+                    )
+            return transformation, reference
 
-        return transformation
+        else:
+            # Tables without IDs don't need truncation
+            return transformation, reference
 
     def _pick_noise_for_count(
         self, query: Union[GroupByCount, GroupByCountDistinct]
     ) -> NoiseMechanism:
         """Pick the noise mechanism to use for a count or count-distinct query."""
         requested_mechanism: NoiseMechanism
         if query.mechanism in (CountMechanism.DEFAULT, CountDistinctMechanism.DEFAULT):
@@ -310,15 +416,14 @@
 
         mechanism: NoiseMechanism
         transformation: Transformation
         mid_stability: sp.Expr
         groupby: GroupBy
         lower_bound: ExactNumber
         upper_bound: ExactNumber
-        new_child: Optional[QueryExpr]
 
     def _build_common(
         self,
         query: Union[
             GroupByBoundedAverage,
             GroupByBoundedSTDEV,
             GroupByBoundedSum,
@@ -339,14 +444,15 @@
         # so check for those
         try:
             measure_desc = expected_schema[query.measure_column]
         except KeyError:
             raise KeyError(
                 f"Measure column {query.measure_column} is not in the input schema."
             )
+
         new_child: Optional[QueryExpr] = None
         # If null or NaN values are allowed ...
         if measure_desc.allow_null or (
             measure_desc.column_type == ColumnType.DECIMAL and measure_desc.allow_nan
         ):
             # then drop those values
             # (but don't mutate the original query)
@@ -368,15 +474,19 @@
 
         expected_output_domain = SparkDataFrameDomain(
             analytics_to_spark_columns_descriptor(expected_schema)
         )
         measure_column_type = expected_output_domain[query.measure_column]
 
         mechanism = self._pick_noise_for_non_count(query, measure_column_type)
-        transformation = self._visit_child_transformation(query.child, mechanism)
+        child_transformation, table_ref = self._truncate_table(
+            *self._visit_child_transformation(query.child, mechanism),
+            grouping_columns=query.groupby_keys.dataframe().columns,
+        )
+        transformation = get_table_from_ref(child_transformation, table_ref)
         # _visit_child_transformation already raises an error if these aren't true
         # these assert statements are just here for MyPy's benefit
         assert isinstance(transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
@@ -390,15 +500,14 @@
         return MeasurementVisitor._AggInfo(
             mechanism=mechanism,
             transformation=transformation,
             mid_stability=mid_stability,
             groupby=groupby,
             lower_bound=lower_bound,
             upper_bound=upper_bound,
-            new_child=new_child,
         )
 
     def _validate_measurement(self, measurement: Measurement, mid_stability: sp.Expr):
         """Validate a measurement."""
         if measurement.privacy_function(mid_stability) != self.budget:
             raise AssertionError(
                 "Privacy function does not match per-query privacy budget. "
@@ -407,15 +516,20 @@
             )
 
     def visit_groupby_count(self, query: GroupByCount) -> Measurement:
         """Create a measurement from a GroupByCount query expression."""
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_count(query)
         mechanism = self._pick_noise_for_count(query)
-        transformation = self._visit_child_transformation(query.child, mechanism)
+        child_transformation, child_ref = self._truncate_table(
+            *self._visit_child_transformation(query.child, mechanism),
+            grouping_columns=query.groupby_keys.dataframe().columns,
+        )
+
+        transformation = get_table_from_ref(child_transformation, child_ref)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
@@ -438,41 +552,44 @@
             count_column=query.output_column,
         )
         self._validate_measurement(agg, mid_stability)
         return transformation | agg
 
     def visit_groupby_count_distinct(self, query: GroupByCountDistinct) -> Measurement:
         """Create a measurement from a GroupByCountDistinct query expression."""
-        # Yes, you need both of these:
-        # columns_to_count=[] means something different from
-        # columns_to_count=None
-        if query.columns_to_count is not None and len(query.columns_to_count) > 0:
-            # select all relevant columns
-            groupby_columns: List[str] = list(query.groupby_keys.schema().keys())
-            # select_cols = all columns to count + groupby_columns
-            select_query = Select(
-                child=query.child, columns=query.columns_to_count + groupby_columns
-            )
-            # Use of dataclasses.replace guarantees that a copy is created,
-            # rather than mutating the original QueryExpr.
-            query = dataclasses.replace(
-                query, child=select_query, columns_to_count=None
-            )
-
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_count_distinct(query)
         mechanism = self._pick_noise_for_count(query)
-        transformation = self._visit_child_transformation(query.child, mechanism)
+        child_transformation, child_ref = self._truncate_table(
+            *self._visit_child_transformation(query.child, mechanism),
+            grouping_columns=query.groupby_keys.dataframe().columns,
+        )
+        transformation = get_table_from_ref(child_transformation, child_ref)
+
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
+        # If not counting all columns, drop the ones that are neither counted
+        # nor grouped on.
+        if query.columns_to_count:
+            groupby_columns = list(query.groupby_keys.schema().keys())
+            transformation |= SelectTransformation(
+                transformation.output_domain,
+                transformation.output_metric,
+                query.columns_to_count + groupby_columns,
+            )
+        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
+        assert isinstance(
+            transformation.output_metric,
+            (IfGroupedBy, HammingDistance, SymmetricDifference),
+        )
 
         mid_stability = transformation.stability_function(self.stability)
         groupby = self._build_groupby(
             transformation.output_domain,
             transformation.output_metric,
             query.groupby_keys,
             mechanism,
@@ -527,17 +644,19 @@
                 replace_with={query.measure_column: (query.low, query.high)},
             )
             query = dataclasses.replace(query, child=replace_infinity_query)
 
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_quantile(query)
 
-        transformation = self._visit_child_transformation(
-            query.child, self.default_mechanism
+        child_transformation, child_ref = self._truncate_table(
+            *self._visit_child_transformation(query.child, self.default_mechanism),
+            grouping_columns=query.groupby_keys.dataframe().columns,
         )
+        transformation = get_table_from_ref(child_transformation, child_ref)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
@@ -567,16 +686,14 @@
 
     def visit_groupby_bounded_sum(self, query: GroupByBoundedSum) -> Measurement:
         """Create a measurement from a GroupByBoundedSum query expression."""
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_bounded_sum(query)
 
         info = self._build_common(query)
-        if info.new_child is not None:
-            query = dataclasses.replace(query, child=info.new_child)
         # _build_common already checks these;
         # these asserts are just for mypy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             info.transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
@@ -600,16 +717,14 @@
     def visit_groupby_bounded_average(
         self, query: GroupByBoundedAverage
     ) -> Measurement:
         """Create a measurement from a GroupByBoundedAverage query expression."""
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_bounded_average(query)
         info = self._build_common(query)
-        if info.new_child is not None:
-            query = dataclasses.replace(query, child=info.new_child)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             info.transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
@@ -633,16 +748,14 @@
     def visit_groupby_bounded_variance(
         self, query: GroupByBoundedVariance
     ) -> Measurement:
         """Create a measurement from a GroupByBoundedVariance query expression."""
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_bounded_variance(query)
         info = self._build_common(query)
-        if info.new_child is not None:
-            query = dataclasses.replace(query, child=info.new_child)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             info.transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
@@ -664,16 +777,14 @@
         return info.transformation | agg
 
     def visit_groupby_bounded_stdev(self, query: GroupByBoundedSTDEV) -> Measurement:
         """Create a measurement from a GroupByBoundedStdev query expression."""
         # Peek at the schema, to see if there are errors there
         OutputSchemaVisitor(self.catalog).visit_groupby_bounded_stdev(query)
         info = self._build_common(query)
-        if info.new_child is not None:
-            query = dataclasses.replace(query, child=info.new_child)
         # _visit_child_transformation already raises an error if these aren't true
         # these are just here for MyPy's benefit
         assert isinstance(info.transformation.output_domain, SparkDataFrameDomain)
         assert isinstance(
             info.transformation.output_metric,
             (IfGroupedBy, HammingDistance, SymmetricDifference),
         )
@@ -687,58 +798,63 @@
             noise_mechanism=info.mechanism,
             d_in=info.mid_stability,
             d_out=self.budget,
             output_measure=self.output_measure,
             groupby_transformation=info.groupby,
             standard_deviation_column=query.output_column,
         )
+
         self._validate_measurement(agg, info.mid_stability)
         return info.transformation | agg
 
     # None of these produce measurements, so they all return a NotImplementedError
-    def visit_private_source(self, expr: PrivateSource) -> Any:
+    def visit_private_source(self, expr) -> Any:
         """Visit a PrivateSource query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_rename(self, expr: Rename) -> Any:
+    def visit_rename(self, expr) -> Any:
         """Visit a Rename query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_filter(self, expr: Filter) -> Any:
+    def visit_filter(self, expr) -> Any:
         """Visit a Filter query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_select(self, expr: Select) -> Any:
+    def visit_select(self, expr) -> Any:
         """Visit a Select query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_map(self, expr: Map) -> Any:
+    def visit_map(self, expr) -> Any:
         """Visit a Map query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_flat_map(self, expr: FlatMap) -> Any:
+    def visit_flat_map(self, expr) -> Any:
         """Visit a FlatMap query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_join_private(self, expr: JoinPrivate) -> Any:
+    def visit_join_private(self, expr) -> Any:
         """Visit a JoinPrivate query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_join_public(self, expr: JoinPublic) -> Any:
+    def visit_join_public(self, expr) -> Any:
         """Visit a JoinPublic query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_replace_null_and_nan(self, expr: ReplaceNullAndNan) -> Any:
+    def visit_replace_null_and_nan(self, expr) -> Any:
         """Visit a ReplaceNullAndNan query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_replace_infinity(self, expr: ReplaceInfinity) -> Any:
+    def visit_replace_infinity(self, expr) -> Any:
         """Visit a ReplaceInfinity query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_drop_infinity(self, expr: DropInfinity) -> Any:
+    def visit_drop_infinity(self, expr) -> Any:
         """Visit a DropInfinity query expression (raises an error)."""
         raise NotImplementedError
 
-    def visit_drop_null_and_nan(self, expr: DropNullAndNan) -> Any:
+    def visit_drop_null_and_nan(self, expr) -> Any:
         """Visit a DropNullAndNan query expression (raises an error)."""
         raise NotImplementedError
+
+    def visit_enforce_constraint(self, expr) -> Any:
+        """Visit an EnforceConstraint query expression (raises an error)."""
+        raise NotImplementedError
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Defines a visitor for determining the output schemas of query expressions."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 from copy import deepcopy
 from typing import KeysView, List, Optional, Union, cast
 
 from pyspark.sql import SparkSession
 
-from tmlt.analytics._catalog import Catalog, PrivateTable, PrivateView, PublicTable
+from tmlt.analytics._catalog import Catalog, PrivateTable, PublicTable
 from tmlt.analytics._schema import (
     ColumnDescriptor,
     ColumnType,
     Schema,
     analytics_to_py_types,
     analytics_to_spark_schema,
     spark_schema_to_analytics_columns,
 )
+from tmlt.analytics.constraints import MaxGroupsPerID, MaxRowsPerGroupPerID
 from tmlt.analytics.query_expr import (
     DropInfinity,
     DropNullAndNan,
+    EnforceConstraint,
     Filter,
     FlatMap,
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
     GroupByBoundedSum,
     GroupByBoundedVariance,
     GroupByCount,
@@ -38,60 +40,69 @@
     ReplaceInfinity,
     ReplaceNullAndNan,
     Select,
 )
 
 
 def _output_schema_for_join(
-    left_schema: Schema, right_schema: Schema, join_columns: Optional[List[str]]
+    left_schema: Schema,
+    right_schema: Schema,
+    join_columns: Optional[List[str]],
+    join_id_space: Optional[str] = None,
 ) -> Schema:
     """Return the resulting schema from joining two tables.
 
+    It is assumed that if either schema has an ID column, the one from
+    left_schema should be used. This is because the appropriate behavior here
+    depends on the type of join being performed, so checks for compatibility of
+    ID columns must happen outside this function.
+
     Args:
         left_schema: Schema for the left table.
         right_schema: Schema for the right table.
         join_columns: The set of columns to join on.
+        join_id_space: The ID space of the resulting join.
     """
     if left_schema.grouping_column is None:
         grouping_column = right_schema.grouping_column
     elif right_schema.grouping_column is None:
         grouping_column = left_schema.grouping_column
     elif left_schema.grouping_column == right_schema.grouping_column:
         grouping_column = left_schema.grouping_column
     else:
         raise ValueError(
-            "Both tables having different grouping columns is not supported"
+            "Joining tables which both have grouping columns is only supported "
+            "if they have the same grouping column"
         )
     common_columns = set(left_schema) & set(right_schema)
-
     if join_columns is None and not common_columns:
-        raise ValueError("Tables have no common columns to join on.")
+        raise ValueError("Tables have no common columns to join on")
     if join_columns is not None and not join_columns:
         # This error case should be caught when constructing the query
         # expression, so it should never get here.
-        raise ValueError(
+        raise AssertionError(
             "Empty list of join columns provided. This is probably a bug; "
             "please let us know about it so we can fix it!"
         )
 
     join_columns = (
         join_columns
         if join_columns
         else sorted(common_columns, key=list(left_schema).index)
     )
 
     if not set(join_columns) <= common_columns:
-        raise ValueError("Join columns must be common to both tables.")
+        raise ValueError("Join columns must be common to both tables")
 
     for column in join_columns:
         if left_schema[column].column_type != right_schema[column].column_type:
             raise ValueError(
-                "Join columns must have identical types on both "
-                f"tables. {left_schema[column]} and "
-                f"{right_schema[column]} are incompatible."
+                "Join columns must have identical types on both tables, "
+                f"but column '{column}' does not: {left_schema[column]} and "
+                f"{right_schema[column]} are incompatible"
             )
 
     output_schema = {
         **{column: left_schema[column] for column in join_columns},
         **{
             column + ("_left" if column in common_columns else ""): left_schema[column]
             for column in left_schema
@@ -100,15 +111,20 @@
         **{
             column
             + ("_right" if column in common_columns else ""): right_schema[column]
             for column in right_schema
             if column not in join_columns
         },
     }
-    return Schema(output_schema, grouping_column=grouping_column)
+    return Schema(
+        output_schema,
+        grouping_column=grouping_column,
+        id_column=left_schema.id_column,
+        id_space=join_id_space,
+    )
 
 
 def _validate_groupby(
     query: Union[
         GroupByBoundedAverage,
         GroupByBoundedSTDEV,
         GroupByBoundedSum,
@@ -149,15 +165,15 @@
                 f" in the input data has type '{input_column_desc.column_type.name}'"
                 " instead."
             )
 
     grouping_column = input_schema.grouping_column
     if grouping_column is not None and grouping_column not in groupby_columns:
         raise ValueError(
-            f"Column produced by grouping transformation '{grouping_column}' "
+            f"Column '{grouping_column}' produced by grouping transformation "
             f"is not in groupby columns {list(groupby_columns)}."
         )
     if (
         not isinstance(query, (GroupByCount, GroupByCountDistinct))
         and query.measure_column in groupby_columns
     ):
         raise ValueError(
@@ -237,158 +253,169 @@
 
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.query_expr import PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = PrivateSource("private")
             >>> query.accept(output_schema_visitor).column_types
             {'A': 'VARCHAR', 'B': 'INTEGER'}
         """
         if expr.source_id not in self._catalog.tables:
-            raise ValueError(f"Query references invalid source '{expr.source_id}'.")
+            raise ValueError(f"Query references nonexistent table '{expr.source_id}'")
         table = self._catalog.tables[expr.source_id]
-        if not isinstance(table, (PrivateTable, PrivateView)):
+        if not isinstance(table, PrivateTable):
             raise ValueError(
-                f"Attempted query on '{expr.source_id}'. "
-                f"'{expr.source_id}' is not a private table."
+                f"Attempted query on table '{expr.source_id}', which is "
+                "not a private table"
             )
         return table.schema
 
     def visit_rename(self, expr: Rename) -> Schema:
         """Returns the resulting schema from evaluating a Rename.
 
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.query_expr import PrivateSource, Rename
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = Rename(PrivateSource("private"), {"B": "C"})
             >>> query.accept(output_schema_visitor).column_types
             {'A': 'VARCHAR', 'C': 'INTEGER'}
         """
         input_schema = expr.child.accept(self)
         grouping_column = input_schema.grouping_column
+        id_column = input_schema.id_column
+        id_space = input_schema.id_space
         nonexistent_columns = set(expr.column_mapper) - set(input_schema)
         if nonexistent_columns:
             raise ValueError(
-                f"Non existent columns {nonexistent_columns} in Rename query."
+                f"Nonexistent columns {nonexistent_columns} in rename query"
             )
         for old, new in expr.column_mapper.items():
             if new in input_schema and new != old:
                 raise ValueError(
-                    f"Cannot rename '{old}' to '{new}'. Column '{new}' already exists."
+                    f"Cannot rename '{old}' to '{new}': column '{new}' already exists"
                 )
             if old == grouping_column:
                 grouping_column = new
+            if old == id_column:
+                id_column = new
+
         return Schema(
             {
                 expr.column_mapper.get(column, column): input_schema[column]
                 for column in input_schema
             },
             grouping_column=grouping_column,
+            id_column=id_column,
+            id_space=id_space,
         )
 
     def visit_filter(self, expr: Filter) -> Schema:
         """Returns the resulting schema from evaluating a Filter.
 
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.query_expr import Filter, PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = Filter(PrivateSource("private"), 'B > 10')
             >>> query.accept(output_schema_visitor).column_types
             {'A': 'VARCHAR', 'B': 'INTEGER'}
         """
         input_schema = expr.child.accept(self)
         spark = SparkSession.builder.getOrCreate()
         test_df = spark.createDataFrame(
             [], schema=analytics_to_spark_schema(input_schema)
         )
         try:
-            test_df.filter(expr.predicate)
+            test_df.filter(expr.condition)
         except Exception as e:
-            raise ValueError(
-                f"Invalid filter expression: '{expr.predicate}' in Filter query: {e}"
-            )
+            raise ValueError(f"Invalid filter condition '{expr.condition}': {e}")
         return input_schema
 
     def visit_select(self, expr: Select) -> Schema:
         """Returns the resulting schema from evaluating a Select.
 
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.query_expr import PrivateSource, Select
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = Select(PrivateSource("private"), ["A"])
             >>> query.accept(output_schema_visitor).column_types
             {'A': 'VARCHAR'}
         """
         input_schema = expr.child.accept(self)
+
         grouping_column = input_schema.grouping_column
-        nonexistent_columns = set(expr.columns) - set(input_schema)
-        if nonexistent_columns:
+        id_column = input_schema.id_column
+        if grouping_column is not None and grouping_column not in expr.columns:
             raise ValueError(
-                f"Non existent columns {nonexistent_columns} in Select query."
+                f"Grouping column '{grouping_column}' may not "
+                "be dropped by select query"
             )
-        if grouping_column is not None and grouping_column not in expr.columns:
+        if id_column is not None and id_column not in expr.columns:
             raise ValueError(
-                f"grouping column {grouping_column} must be included in Select query"
+                f"ID column '{id_column}' may not be dropped by select query"
             )
+
+        nonexistent_columns = set(expr.columns) - set(input_schema)
+        if nonexistent_columns:
+            raise ValueError(
+                f"Nonexistent columns {nonexistent_columns} in select query."
+            )
+
         return Schema(
             {column: input_schema[column] for column in expr.columns},
             grouping_column=grouping_column,
+            id_column=id_column,
+            id_space=input_schema.id_space,
         )
 
     def visit_map(self, expr: Map) -> Schema:
         """Returns the resulting schema from evaluating a Map.
 
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.query_expr import Map, PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={
             ...         "A": ColumnType.VARCHAR,
             ...         "B": ColumnType.INTEGER,
             ...     },
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query1 = Map( # Augment = False example
             ...     child=PrivateSource("private"),
             ...     f=lambda row: {"C": row["B"] + 1, "D": "A"},
             ...     schema_new_columns=Schema(
             ...         {"C": ColumnType.INTEGER, "D": ColumnType.VARCHAR}
@@ -415,94 +442,114 @@
         # Any column created by Map could contain a null value
         for name in list(new_columns.keys()):
             new_columns[name].allow_null = True
         if expr.augment:
             return Schema(
                 {**input_schema, **new_columns},
                 grouping_column=input_schema.grouping_column,
+                id_column=input_schema.id_column,
+                id_space=input_schema.id_space,
             )
         elif input_schema.grouping_column:
             raise ValueError(
-                "Need to set augment=True to ensure that the grouping column "
-                "is available for groupby."
+                "Map must set augment=True to ensure that "
+                f"grouping column '{input_schema.grouping_column}' is not lost."
+            )
+        elif input_schema.id_column:
+            raise ValueError(
+                "Map must set augment=True to ensure that "
+                f"ID column '{input_schema.id_column}' is not lost."
             )
         return new_columns
 
     def visit_flat_map(self, expr: FlatMap) -> Schema:
         # pylint: disable=line-too-long
         """Returns the resulting schema from evaluating a FlatMap.
 
         ..
             >>> from tmlt.analytics._schema import ColumnType, Schema
             >>> from tmlt.analytics.query_expr import FlatMap, PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query1 = FlatMap( # Augment = False example
             ...     child=PrivateSource("private"),
             ...     f=lambda row: [{"C": row["B"]}, {"C": row["B"] + 1}],
-            ...     max_num_rows=2,
             ...     schema_new_columns=Schema({"C": ColumnType.INTEGER}),
             ...     augment=False,
+            ...     max_num_rows=2,
             ... )
             >>> query1.accept(output_schema_visitor).column_types
             {'C': 'INTEGER'}
             >>> query2 = FlatMap( # Augment = True example
             ...     child=PrivateSource("private"),
             ...     f=lambda row: [{"C": row["B"]}, {"C": row["B"] + 1}],
-            ...     max_num_rows=2,
             ...     schema_new_columns=Schema({"C": ColumnType.INTEGER}),
             ...     augment=True,
+            ...     max_num_rows=2,
             ... )
             >>> query2.accept(output_schema_visitor).column_types
             {'A': 'VARCHAR', 'B': 'INTEGER', 'C': 'INTEGER'}
             >>> query3 = FlatMap( # Grouping example
             ...     child=PrivateSource("private"),
             ...     f=lambda row: [{"C": row["B"]}, {"C": row["B"] + 1}],
-            ...     max_num_rows=2,
             ...     schema_new_columns=Schema(
             ...         {"C": ColumnType.INTEGER}, grouping_column="C",
             ...     ),
             ...     augment=True,
+            ...     max_num_rows=2,
             ... )
             >>> query3.accept(output_schema_visitor).column_types
             {'A': 'VARCHAR', 'B': 'INTEGER', 'C': 'INTEGER'}
         """
         input_schema = expr.child.accept(self)
-        if expr.schema_new_columns.grouping_column is None:
-            grouping_column = input_schema.grouping_column
-        else:
+        if expr.schema_new_columns.grouping_column is not None:
             if input_schema.grouping_column:
                 raise ValueError(
                     "Multiple grouping transformations are used in this query. "
                     "Only one grouping transformation is allowed."
                 )
-            (grouping_column,) = expr.schema_new_columns
+            if input_schema.id_column:
+                raise ValueError(
+                    "Grouping flat map cannot be used on tables with "
+                    "the AddRowsWithID protected change"
+                )
+            grouping_column = expr.schema_new_columns.grouping_column
+        else:
+            grouping_column = input_schema.grouping_column
 
         # Make a deep copy - that way we don't modify the schema
         # that the user provided
         new_columns = deepcopy(expr.schema_new_columns)
         # Any column created by the FlatMap could contain a null value
         for name in list(new_columns.keys()):
             new_columns[name].allow_null = True
         if expr.augment:
             return Schema(
-                {**input_schema, **new_columns}, grouping_column=grouping_column
+                {**input_schema, **new_columns},
+                grouping_column=grouping_column,
+                id_column=input_schema.id_column,
+                id_space=input_schema.id_space,
+            )
+        elif input_schema.grouping_column:
+            raise ValueError(
+                "Flat map must set augment=True to ensure that "
+                f"grouping column '{input_schema.grouping_column}' is not lost"
             )
-        elif input_schema.grouping_column is not None:
+        elif input_schema.id_column:
             raise ValueError(
-                "Need to set augment=True to ensure that the grouping column "
-                "is available for groupby."
+                "Flat map must set augment=True to ensure that "
+                f"ID column '{input_schema.id_column}' is not lost"
             )
+
         return new_columns
 
     def visit_join_private(self, expr: JoinPrivate) -> Schema:
         # pylint: disable=line-too-long
         """Returns the resulting schema from evaluating a JoinPrivate.
 
         The ordering of output columns are:
@@ -518,33 +565,31 @@
             >>> from tmlt.analytics.query_expr import (
             ...     JoinPrivate, PrivateSource
             ... )
             >>> from tmlt.analytics.truncation_strategy import TruncationStrategy
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="left_source",
             ...     col_types={
             ...         "left_only": ColumnType.DECIMAL,
             ...         "common1": ColumnType.INTEGER,
             ...         "common2": ColumnType.VARCHAR,
             ...         "common3": ColumnType.INTEGER
             ...     },
-            ...     stability=1,
             ... )
-            >>> catalog.add_private_view(
+            >>> catalog.add_private_table(
             ...     source_id="right_source",
             ...     col_types={
             ...         "common1": ColumnType.INTEGER,
             ...         "common2": ColumnType.VARCHAR,
             ...         "common3": ColumnType.INTEGER,
             ...         "right_only": ColumnType.VARCHAR,
             ...    },
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> # join_columns default behavior is ["common1", "common2", "common3"]
             >>> query1 = JoinPrivate(
             ...     child=PrivateSource("left_source"),
             ...     right_operand_expr=PrivateSource("right_source"),
             ...     truncation_strategy_left=TruncationStrategy.DropExcess(1),
@@ -558,249 +603,355 @@
             ...     truncation_strategy_left=TruncationStrategy.DropExcess(1),
             ...     truncation_strategy_right=TruncationStrategy.DropExcess(1),
             ...     join_columns=["common3"],
             ... )
             >>> query2.accept(output_schema_visitor).column_types
             {'common3': 'INTEGER', 'left_only': 'DECIMAL', 'common1_left': 'INTEGER', 'common2_left': 'VARCHAR', 'common1_right': 'INTEGER', 'common2_right': 'VARCHAR', 'right_only': 'VARCHAR'}
         """
+        left_schema = expr.child.accept(self)
+        right_schema = expr.right_operand_expr.accept(self)
+        if left_schema.id_column != right_schema.id_column:
+            if left_schema.id_column is None or right_schema.id_column is None:
+                raise ValueError(
+                    "Private joins can only be performed between two tables "
+                    "with the same type of protected change"
+                )
+            raise ValueError(
+                "Private joins between tables with the AddRowsWithID "
+                "protected change are only possible when the ID columns of "
+                "the two tables have the same name"
+            )
+        if (
+            left_schema.id_space
+            and right_schema.id_space
+            and left_schema.id_space != right_schema.id_space
+        ):
+            raise ValueError(
+                "Private joins between tables with the AddRowsWithID protected change"
+                " are only possible when both tables are in the same ID space"
+            )
+        join_id_space: Optional[str] = None
+        if left_schema.id_space and right_schema.id_space:
+            join_id_space = left_schema.id_space
         return _output_schema_for_join(
-            left_schema=expr.child.accept(self),
-            right_schema=expr.right_operand_expr.accept(self),
+            left_schema=left_schema,
+            right_schema=right_schema,
             join_columns=expr.join_columns,
+            join_id_space=join_id_space,
         )
 
     def visit_join_public(self, expr: JoinPublic) -> Schema:
         """Returns the resulting schema from evaluating a JoinPublic.
 
         Has analogous behavior to :meth:`OutputSchemaVisitor.visit_join_private`,
         where the private table is the left table.
 
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.query_expr import JoinPublic, PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
-            >>> catalog.add_public_source(
+            >>> catalog.add_public_table(
             ...     "public", {"B": ColumnType.INTEGER, "C": ColumnType.DECIMAL}
             ... )
             >>> query = JoinPublic(
             ...    child=PrivateSource("private"), public_table="public"
             ... )
             >>> query.accept(output_schema_visitor).column_types
             {'B': 'INTEGER', 'A': 'VARCHAR', 'C': 'DECIMAL'}
         """
         input_schema = expr.child.accept(self)
         if isinstance(expr.public_table, str):
             public_table = self._catalog.tables[expr.public_table]
             if not isinstance(public_table, PublicTable):
                 raise ValueError(
-                    f"Attempted JoinPublic on '{expr.public_table}' table. "
-                    f"'{expr.public_table}' is not a public table."
+                    f"Attempted public join on table '{expr.public_table}', "
+                    "which is not a public table"
                 )
             right_schema = public_table.schema
         else:
             right_schema = Schema(
                 spark_schema_to_analytics_columns(expr.public_table.schema)
             )
         return _output_schema_for_join(
             left_schema=input_schema,
             right_schema=right_schema,
             join_columns=expr.join_columns,
+            join_id_space=input_schema.id_space,
         )
 
     def visit_replace_null_and_nan(self, expr: ReplaceNullAndNan) -> Schema:
         """Returns the resulting schema from evaluating a ReplaceNullAndNan."""
         input_schema = expr.child.accept(self)
+
         if (
             input_schema.grouping_column
             and input_schema.grouping_column in expr.replace_with
         ):
             raise ValueError(
-                f"Cannot replace null values in column {input_schema.grouping_column},"
-                " because it is being used as a grouping column"
+                "Cannot replace null values in column "
+                f"'{input_schema.grouping_column}', as it is a grouping column"
             )
+        if input_schema.id_column and input_schema.id_column in expr.replace_with:
+            raise ValueError(
+                f"Cannot replace null values in column '{input_schema.id_column}', "
+                "as it is an ID column"
+            )
+
         if len(expr.replace_with) != 0:
             pytypes = analytics_to_py_types(input_schema)
             for col, val in expr.replace_with.items():
                 if col not in input_schema.keys():
                     raise ValueError(
-                        "ReplaceNullAndNan.replace_with contains a replacement value"
-                        f" for the column {col}, but data has no column named {col}"
+                        f"Column '{col}' does not exist in this table, "
+                        f"available columns are {list(input_schema.keys())}"
                     )
                 if not isinstance(val, pytypes[col]):
                     # it's ok to use an int as a float
                     # so don't raise an error in that case
                     if not (isinstance(val, int) and pytypes[col] == float):
                         raise ValueError(
-                            f"ReplaceNullAndNan.replace_with has column {col}'s default"
-                            f" value set to {val}, which does not match the column type"
-                            f" {input_schema[col].column_type.name}"
+                            f"Column '{col}' cannot have nulls replaced with "
+                            f"{repr(val)}, as that value's type does not match the "
+                            f"column type {input_schema[col].column_type.name}"
                         )
+
         columns_to_change = list(dict(expr.replace_with).keys())
         if len(columns_to_change) == 0:
             columns_to_change = [
                 col
                 for col in input_schema.column_descs.keys()
                 if (input_schema[col].allow_null or input_schema[col].allow_nan)
                 and not (col == input_schema.grouping_column)
             ]
+
         return Schema(
             {
                 name: ColumnDescriptor(
                     column_type=cd.column_type,
                     allow_null=(cd.allow_null and not name in columns_to_change),
                     allow_nan=(cd.allow_nan and not name in columns_to_change),
                     allow_inf=cd.allow_inf,
                 )
                 for name, cd in input_schema.column_descs.items()
             },
             grouping_column=input_schema.grouping_column,
+            id_column=input_schema.id_column,
+            id_space=input_schema.id_space,
         )
 
     def visit_replace_infinity(self, expr: ReplaceInfinity) -> Schema:
         """Returns the resulting schema from evaluating a ReplaceInfinity."""
         input_schema = expr.child.accept(self)
+
+        if (
+            input_schema.grouping_column
+            and input_schema.grouping_column in expr.replace_with
+        ):
+            raise ValueError(
+                "Cannot replace infinite values in column "
+                f"'{input_schema.grouping_column}', as it is a grouping column"
+            )
+        # Float-valued columns cannot be ID columns, but include this to be safe.
+        if input_schema.id_column and input_schema.id_column in expr.replace_with:
+            raise ValueError(
+                f"Cannot replace infinite values in column '{input_schema.id_column}', "
+                "as it is an ID column"
+            )
+
         columns_to_change = list(expr.replace_with.keys())
         if len(columns_to_change) == 0:
             columns_to_change = [
                 col
                 for col in input_schema.column_descs.keys()
                 if input_schema[col].column_type == ColumnType.DECIMAL
             ]
         else:
             for name in expr.replace_with:
                 if name not in input_schema.keys():
                     raise ValueError(
-                        "ReplaceInfinity.replace_with contains replacement values for"
-                        f" the column {name}, but data has no column named {name}"
+                        f"Column '{name}' does not exist in this table, "
+                        f"available columns are {list(input_schema.keys())}"
                     )
                 if input_schema[name].column_type != ColumnType.DECIMAL:
                     raise ValueError(
-                        "ReplaceInfinity.replace_with contains replacement values for"
-                        f" the column {name}, but the column {name} has type"
-                        f" {input_schema[name].column_type.name} (not"
-                        f" {ColumnType.DECIMAL.name})"
+                        f"Column '{name}' has a replacement value provided, but it is "
+                        f"of type {input_schema[name].column_type.name} (not "
+                        f"{ColumnType.DECIMAL.name}) and so cannot "
+                        "contain infinite values"
                     )
         return Schema(
             {
                 name: ColumnDescriptor(
                     column_type=cd.column_type,
                     allow_null=cd.allow_null,
                     allow_nan=cd.allow_nan,
                     allow_inf=(cd.allow_inf and not name in columns_to_change),
                 )
                 for name, cd in input_schema.column_descs.items()
             },
             grouping_column=input_schema.grouping_column,
+            id_column=input_schema.id_column,
+            id_space=input_schema.id_space,
         )
 
-    def visit_drop_infinity(self, expr: DropInfinity) -> Schema:
-        """Returns the resulting schema from evaluating a DropInfinity."""
+    def visit_drop_null_and_nan(self, expr: DropNullAndNan) -> Schema:
+        """Returns the resulting schema from evaluating a DropNullAndNan."""
         input_schema = expr.child.accept(self)
+
         if (
             input_schema.grouping_column
             and input_schema.grouping_column in expr.columns
         ):
             raise ValueError(
-                f"Cannot drop null values in column {input_schema.grouping_column},"
-                " because it is being used as a grouping column"
+                f"Cannot drop null values in column '{input_schema.grouping_column}', "
+                "as it is a grouping column"
+            )
+        if input_schema.id_column and input_schema.id_column in expr.columns:
+            raise ValueError(
+                f"Cannot drop null values in column '{input_schema.id_column}', "
+                "as it is an ID column"
             )
+
         columns = expr.columns.copy()
         if len(columns) == 0:
             columns = [
                 name
                 for name, cd in input_schema.column_descs.items()
-                if (cd.allow_inf) and not name == input_schema.grouping_column
+                if (cd.allow_null or cd.allow_nan)
+                and not name == input_schema.grouping_column
             ]
         else:
             for name in columns:
                 if name not in input_schema.keys():
                     raise ValueError(
-                        "DropInfinity.columns contains the column"
-                        f" {name}, but data has no column named {name}"
-                    )
-                if input_schema[name].column_type != ColumnType.DECIMAL:
-                    raise ValueError(
-                        f"DropInfinity.columns contains the column {name}, but the"
-                        f" column {name} is not a DECIMAL column and cannot contain"
-                        " infinite values"
+                        f"Column '{name}' does not exist in this table, "
+                        f"available columns are {list(input_schema.keys())}"
                     )
+
         return Schema(
             {
                 name: ColumnDescriptor(
                     column_type=cd.column_type,
-                    allow_null=cd.allow_null,
-                    allow_nan=cd.allow_nan,
-                    allow_inf=(cd.allow_inf and not name in columns),
+                    allow_null=(cd.allow_null and not name in columns),
+                    allow_nan=(cd.allow_nan and not name in columns),
+                    allow_inf=(cd.allow_inf),
                 )
                 for name, cd in input_schema.column_descs.items()
             },
             grouping_column=input_schema.grouping_column,
+            id_column=input_schema.id_column,
+            id_space=input_schema.id_space,
         )
 
-    def visit_drop_null_and_nan(self, expr: DropNullAndNan) -> Schema:
-        """Returns the resulting schema from evaluating a DropNullAndNan."""
+    def visit_drop_infinity(self, expr: DropInfinity) -> Schema:
+        """Returns the resulting schema from evaluating a DropInfinity."""
         input_schema = expr.child.accept(self)
+
         if (
             input_schema.grouping_column
             and input_schema.grouping_column in expr.columns
         ):
             raise ValueError(
-                f"Cannot drop null values in column {input_schema.grouping_column},"
-                " because it is being used as a grouping column"
+                "Cannot drop infinite values in column "
+                f"'{input_schema.grouping_column}', as it is a grouping column"
+            )
+        # Float-valued columns cannot be ID columns, but include this to be safe.
+        if input_schema.id_column and input_schema.id_column in expr.columns:
+            raise ValueError(
+                f"Cannot drop infinite values in column '{input_schema.id_column}', "
+                "as it is an ID column"
             )
+
         columns = expr.columns.copy()
         if len(columns) == 0:
             columns = [
                 name
                 for name, cd in input_schema.column_descs.items()
-                if (cd.allow_null or cd.allow_nan)
-                and not name == input_schema.grouping_column
+                if (cd.allow_inf) and not name == input_schema.grouping_column
             ]
         else:
             for name in columns:
                 if name not in input_schema.keys():
                     raise ValueError(
-                        "DropNullAndNan.columns contains the column"
-                        f" {name}, but data has no column named {name}"
+                        f"Column '{name}' does not exist in this table, "
+                        f"available columns are {list(input_schema.keys())}"
                     )
+                if input_schema[name].column_type != ColumnType.DECIMAL:
+                    raise ValueError(
+                        f"Column '{name}' was given as a column to drop "
+                        "infinite values from, but it is of type"
+                        f"{input_schema[name].column_type.name} (not "
+                        f"{ColumnType.DECIMAL.name}) and so cannot "
+                        "contain infinite values"
+                    )
+
         return Schema(
             {
                 name: ColumnDescriptor(
                     column_type=cd.column_type,
-                    allow_null=(cd.allow_null and not name in columns),
-                    allow_nan=(cd.allow_nan and not name in columns),
-                    allow_inf=(cd.allow_inf),
+                    allow_null=cd.allow_null,
+                    allow_nan=cd.allow_nan,
+                    allow_inf=(cd.allow_inf and not name in columns),
                 )
                 for name, cd in input_schema.column_descs.items()
             },
             grouping_column=input_schema.grouping_column,
+            id_column=input_schema.id_column,
+            id_space=input_schema.id_space,
         )
 
+    def visit_enforce_constraint(self, expr: EnforceConstraint) -> Schema:
+        """Returns the resulting schema from evaluating an EnforceConstraint."""
+        input_schema = expr.child.accept(self)
+        constraint = expr.constraint
+
+        if not input_schema.id_column:
+            raise ValueError(
+                f"Constraint {expr.constraint} can only be applied to tables"
+                " with the AddRowsWithID protected change"
+            )
+        if isinstance(constraint, (MaxGroupsPerID, MaxRowsPerGroupPerID)):
+            grouping_column = constraint.grouping_column
+            if grouping_column not in input_schema:
+                raise ValueError(
+                    f"The grouping column of constraint {constraint}"
+                    " does not exist in this table; available columns"
+                    f" are: {', '.join(input_schema.keys())}"
+                )
+            if grouping_column == input_schema.id_column:
+                raise ValueError(
+                    f"The grouping column of constraint {constraint} cannot be"
+                    " the ID column of the table it is applied to"
+                )
+
+        # No current constraints modify the schema. If that changes in the
+        # future, the logic for it may have to be pushed into the Constraint
+        # type (like how constraint._enforce() works), but for now this works.
+        return input_schema
+
     def visit_groupby_count(self, expr: GroupByCount) -> Schema:
         """Returns the resulting schema from evaluating a GroupByCount.
 
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.keyset import KeySet
             >>> from tmlt.analytics.query_expr import PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = GroupByCount(
             ...     child=PrivateSource("private"),
             ...     groupby_keys=KeySet.from_dict({"A": ["a1", "a2", "a3"]}),
             ...     output_column="count",
             ... )
@@ -815,18 +966,17 @@
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.keyset import KeySet
             >>> from tmlt.analytics.query_expr import PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = GroupByCountDistinct(
             ...     child=PrivateSource("private"),
             ...     groupby_keys=KeySet.from_dict({"A": ["a1", "a2", "a3"]}),
             ...     output_column="count_distinct",
             ... )
@@ -841,18 +991,17 @@
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.keyset import KeySet
             >>> from tmlt.analytics.query_expr import PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = GroupByQuantile(
             ...     child=PrivateSource("private"),
             ...     groupby_keys=KeySet.from_dict({"A": ["a1", "a2", "a3"]}),
             ...     measure_column="B",
             ...     quantile=0.5,
@@ -871,18 +1020,17 @@
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.keyset import KeySet
             >>> from tmlt.analytics.query_expr import PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = GroupByBoundedSum(
             ...     child=PrivateSource("private"),
             ...     groupby_keys=KeySet.from_dict({"A": ["a1", "a2", "a3"]}),
             ...     measure_column="B",
             ...     low=0,
@@ -900,18 +1048,17 @@
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.keyset import KeySet
             >>> from tmlt.analytics.query_expr import PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = GroupByBoundedAverage(
             ...     child=PrivateSource("private"),
             ...     groupby_keys=KeySet.from_dict({"A": ["a1", "a2", "a3"]}),
             ...     measure_column="B",
             ...     low=0,
@@ -929,18 +1076,17 @@
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.keyset import KeySet
             >>> from tmlt.analytics.query_expr import PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = GroupByBoundedAverage(
             ...     child=PrivateSource("private"),
             ...     groupby_keys=KeySet.from_dict({"A": ["a1", "a2", "a3"]}),
             ...     measure_column="B",
             ...     low=0,
@@ -958,18 +1104,17 @@
         ..
             >>> from tmlt.analytics._schema import ColumnType
             >>> from tmlt.analytics.keyset import KeySet
             >>> from tmlt.analytics.query_expr import PrivateSource
 
         Example:
             >>> catalog = Catalog()
-            >>> catalog.add_private_source(
+            >>> catalog.add_private_table(
             ...     source_id="private",
             ...     col_types={"A": ColumnType.VARCHAR, "B": ColumnType.INTEGER},
-            ...     stability=1,
             ... )
             >>> output_schema_visitor = OutputSchemaVisitor(catalog)
             >>> query = GroupByBoundedSTDEV(
             ...     child=PrivateSource("private"),
             ...     groupby_keys=KeySet.from_dict({"A": ["a1", "a2", "a3"]}),
             ...     measure_column="B",
             ...     low=0,
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,141 @@
 """Defines a visitor for creating a transformation from a query expression."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 import dataclasses
 import datetime
-from typing import Any, Dict, Optional, Union
+import warnings
+from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Type, Union
 
 from pyspark.sql import DataFrame
 
 from tmlt.analytics._catalog import Catalog
+from tmlt.analytics._query_expr_compiler._constraint_propagation import (
+    propagate_flat_map,
+    propagate_join_private,
+    propagate_join_public,
+    propagate_map,
+    propagate_rename,
+    propagate_replace,
+    propagate_select,
+    propagate_unmodified,
+)
 from tmlt.analytics._query_expr_compiler._output_schema_visitor import (
     OutputSchemaVisitor,
 )
 from tmlt.analytics._schema import (
+    ColumnDescriptor,
     ColumnType,
     Schema,
     analytics_to_spark_columns_descriptor,
     spark_dataframe_domain_to_analytics_columns,
     spark_schema_to_analytics_columns,
 )
+from tmlt.analytics._table_identifier import Identifier, TemporaryTable
+from tmlt.analytics._table_reference import (
+    TableReference,
+    find_named_tables,
+    find_reference,
+    lookup_domain,
+    lookup_metric,
+)
+from tmlt.analytics._transformation_utils import generate_nested_transformation
+from tmlt.analytics.constraints import Constraint, simplify_constraints
 from tmlt.analytics.query_expr import AnalyticsDefault
 from tmlt.analytics.query_expr import DropInfinity as DropInfExpr
-from tmlt.analytics.query_expr import DropNullAndNan
+from tmlt.analytics.query_expr import DropNullAndNan, EnforceConstraint
 from tmlt.analytics.query_expr import Filter as FilterExpr
 from tmlt.analytics.query_expr import FlatMap as FlatMapExpr
 from tmlt.analytics.query_expr import (
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
     GroupByBoundedSum,
     GroupByBoundedVariance,
     GroupByCount,
     GroupByCountDistinct,
     GroupByQuantile,
 )
 from tmlt.analytics.query_expr import JoinPrivate as JoinPrivateExpr
 from tmlt.analytics.query_expr import JoinPublic as JoinPublicExpr
 from tmlt.analytics.query_expr import Map as MapExpr
-from tmlt.analytics.query_expr import PrivateSource, QueryExpr, QueryExprVisitor
+from tmlt.analytics.query_expr import QueryExpr, QueryExprVisitor
 from tmlt.analytics.query_expr import Rename as RenameExpr
 from tmlt.analytics.query_expr import ReplaceInfinity, ReplaceNullAndNan
 from tmlt.analytics.query_expr import Select as SelectExpr
 from tmlt.analytics.truncation_strategy import TruncationStrategy
 from tmlt.core.domains.collections import DictDomain, ListDomain
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain, SparkRowDomain
 from tmlt.core.measurements.aggregations import NoiseMechanism
 from tmlt.core.metrics import (
+    AddRemoveKeys,
     DictMetric,
     HammingDistance,
     IfGroupedBy,
+    Metric,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.transformations.converters import HammingDistanceToSymmetricDifference
 from tmlt.core.transformations.dictionary import (
     AugmentDictTransformation,
     CreateDictFromValue,
-    GetValue,
     Subset,
+    create_copy_and_transform_value,
+)
+from tmlt.core.transformations.identity import Identity as IdentityTransformation
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    DropInfsValue as DropInfsValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    DropNaNsValue as DropNaNsValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    DropNullsValue as DropNullsValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    FilterValue as FilterValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    FlatMapValue as FlatMapValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    MapValue as MapValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    PublicJoinValue as PublicJoinValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    RenameValue as RenameValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    ReplaceInfsValue as ReplaceInfsValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    ReplaceNaNsValue as ReplaceNaNsValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    ReplaceNullsValue as ReplaceNullsValueTransformation,
+)
+from tmlt.core.transformations.spark_transformations.add_remove_keys import (
+    SelectValue as SelectValueTransformation,
 )
 from tmlt.core.transformations.spark_transformations.filter import (
     Filter as FilterTransformation,
 )
 from tmlt.core.transformations.spark_transformations.join import (
     PrivateJoin as PrivateJoinTransformation,
 )
 from tmlt.core.transformations.spark_transformations.join import (
+    PrivateJoinOnKey as PrivateJoinOnKeyTransformation,
+)
+from tmlt.core.transformations.spark_transformations.join import (
     PublicJoin as PublicJoinTransformation,
 )
 from tmlt.core.transformations.spark_transformations.join import (
     TruncationStrategy as CoreTruncationStrategy,
 )
 from tmlt.core.transformations.spark_transformations.map import (
     FlatMap as FlatMapTransformation,
@@ -82,545 +146,788 @@
     RowToRowsTransformation,
     RowToRowTransformation,
 )
 from tmlt.core.transformations.spark_transformations.nan import (
     DropInfs as DropInfTransformation,
 )
 from tmlt.core.transformations.spark_transformations.nan import (
-    DropNaNs,
-    DropNulls,
-    ReplaceInfs,
-    ReplaceNaNs,
-    ReplaceNulls,
+    DropNaNs as DropNaNsTransformation,
+)
+from tmlt.core.transformations.spark_transformations.nan import (
+    DropNulls as DropNullsTransformation,
+)
+from tmlt.core.transformations.spark_transformations.nan import (
+    ReplaceInfs as ReplaceInfsTransformation,
+)
+from tmlt.core.transformations.spark_transformations.nan import (
+    ReplaceNaNs as ReplaceNaNsTransformation,
+)
+from tmlt.core.transformations.spark_transformations.nan import (
+    ReplaceNulls as ReplaceNullsTransformation,
 )
 from tmlt.core.transformations.spark_transformations.rename import (
     Rename as RenameTransformation,
 )
 from tmlt.core.transformations.spark_transformations.select import (
     Select as SelectTransformation,
 )
-from tmlt.core.utils.misc import get_nonconflicting_string
 
 
 class TransformationVisitor(QueryExprVisitor):
     """A visitor to create a transformation from a query expression."""
 
+    class Output(NamedTuple):
+        """A container for the outputs of the visitor."""
+
+        transformation: Transformation
+        reference: TableReference
+        constraints: List[Constraint]
+
     def __init__(
         self,
         input_domain: DictDomain,
         input_metric: DictMetric,
         mechanism: NoiseMechanism,
         public_sources: Dict[str, DataFrame],
+        table_constraints: Dict[Identifier, List[Constraint]],
     ):
         """Constructor for a TransformationVisitor.
 
         Args:
             input_domain: The input domain that the transformation should have.
             input_metric: The input metric that the transformation should have.
             mechanism: The noise mechanism (only used for FlatMaps).
             public_sources: Public sources to use for JoinPublic queries.
+            table_constraints: A mapping of tables to the existing constraints on them.
         """
         self.input_domain = input_domain
         self.input_metric = input_metric
         self.mechanism = mechanism
         self.public_sources = public_sources
+        self.table_constraints = table_constraints
 
     def validate_transformation(
-        self, query: QueryExpr, transformation: Transformation, catalog: Catalog
+        self,
+        query: QueryExpr,
+        transformation: Transformation,
+        reference: TableReference,
+        catalog: Catalog,
     ):
         """Ensure that a query's transformation is valid on a given catalog."""
         expected_schema = query.accept(OutputSchemaVisitor(catalog))
         expected_output_domain = SparkDataFrameDomain(
             analytics_to_spark_columns_descriptor(expected_schema)
         )
-        expected_output_metric = (
-            SymmetricDifference()
-            if expected_schema.grouping_column is None
-            else IfGroupedBy(expected_schema.grouping_column, self.inner_metric())
-        )
-        if transformation.output_domain != expected_output_domain:
+
+        expected_output_metric: Metric
+        if (
+            expected_schema.grouping_column is not None
+            and expected_schema.id_column is not None
+        ):
+            raise AssertionError(
+                "Output schema from a transformation had both an ID column "
+                "and a grouping column, which is not allowed. This is probably a bug; "
+                "please let us know about it so we can fix it!"
+            )
+
+        if expected_schema.grouping_column is not None:
+            expected_output_metric = IfGroupedBy(
+                expected_schema.grouping_column, self.inner_metric()
+            )
+        elif expected_schema.id_column is not None:
+            expected_output_metric = IfGroupedBy(
+                expected_schema.id_column, SymmetricDifference()
+            )
+        else:
+            expected_output_metric = SymmetricDifference()
+
+        if (
+            lookup_domain(transformation.output_domain, reference)
+            != expected_output_domain
+        ):
             raise AssertionError(
                 "Unexpected output domain. This is probably a bug; "
                 "please let us know about it so we can fix it!"
             )
-        if transformation.output_metric != expected_output_metric:
+        if (
+            lookup_metric(transformation.output_metric, reference)
+            != expected_output_metric
+        ):
             raise AssertionError(
                 "Unexpected output metric. This is probably a bug; "
                 "please let us know about it so we can fix it!"
             )
 
-    # TODO(#2172): update so it no longer assumes source ID is in domain
-    def visit_private_source(self, expr: PrivateSource) -> Transformation:
-        """Create a transformation from a PrivateSource query expression."""
-        # check if the source ID is in the input domain's keys. If not,
-        # it likely exists in a dict one level into the input domain
-        # if expr.source_id in self.input_domain.key_to_domain:
-        return GetValue(self.input_domain, self.input_metric, expr.source_id)
+    def inner_metric(self) -> Union[SumOf, RootSumOfSquared]:
+        """Get the inner metric used by this TransformationVisitor."""
+        if self.mechanism in (NoiseMechanism.LAPLACE, NoiseMechanism.GEOMETRIC):
+            return SumOf(SymmetricDifference())
+        else:
+            if self.mechanism != NoiseMechanism.DISCRETE_GAUSSIAN:
+                raise RuntimeError(
+                    f"Unsupported mechanism {self.mechanism}. "
+                    "Supported mechanisms are "
+                    f"{NoiseMechanism.DISCRETE_GAUSSIAN}, "
+                    f"{NoiseMechanism.LAPLACE}, and"
+                    f"{NoiseMechanism.GEOMETRIC}."
+                )
+            return RootSumOfSquared(SymmetricDifference())
 
-    def _visit_child(self, child: QueryExpr) -> Transformation:
+    def _visit_child(self, child: QueryExpr) -> Output:
         """Visit a child query and raise assertion errors if needed."""
-        transformation = child.accept(self)
+        transformation, reference, constraints = child.accept(self)
         if not isinstance(transformation, Transformation):
             raise AssertionError(
                 "Child query did not create a transformation. "
                 "This is probably a bug; please let us know about it so "
                 "we can fix it!"
             )
-        if not isinstance(transformation.output_domain, SparkDataFrameDomain):
+        input_domain = lookup_domain(transformation.output_domain, reference)
+        input_metric = lookup_metric(transformation.output_metric, reference)
+        if not isinstance(input_domain, SparkDataFrameDomain):
             raise AssertionError(
                 "Child query has an invalid output domain. "
                 "This is probably a bug; please let us know about it so "
                 "we can fix it!"
             )
         if not isinstance(
-            transformation.output_metric,
-            (IfGroupedBy, SymmetricDifference, HammingDistance),
+            input_metric, (IfGroupedBy, SymmetricDifference, HammingDistance)
         ):
             raise AssertionError(
                 "Child query does not have a recognized output metric. "
                 "This is probably a bug; please let us know about "
                 "it so we can fix it!"
             )
-        return transformation
+        return self.Output(transformation, reference, constraints)
 
-    def visit_rename(self, query: RenameExpr) -> Transformation:
-        """Create a transformation from a Rename query expression."""
-        if not isinstance(query.column_mapper, dict):
-            raise ValueError(
-                "Rename query's column_mapper must be "
-                "a dictionary mapping old column names "
-                "to new column names."
-            )
-        child = self._visit_child(query.child)
-        assert isinstance(child.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            child.output_metric, (IfGroupedBy, SymmetricDifference, HammingDistance)
-        )
-        rename_transformation = RenameTransformation(
-            input_domain=child.output_domain,
-            metric=child.output_metric,
-            rename_mapping=query.column_mapper,
+    @classmethod
+    def _ensure_not_hamming(
+        cls,
+        transformation: Transformation,
+        reference: TableReference,
+        constraints: List[Constraint],
+    ) -> Output:
+        """Convert transformation to one with a SymmetricDifference() output metric."""
+        input_domain = lookup_domain(transformation.output_domain, reference)
+        input_metric = lookup_metric(transformation.output_metric, reference)
+        if not isinstance(input_metric, HammingDistance):
+            return cls.Output(transformation, reference, constraints)
+
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            if not isinstance(input_domain, SparkDataFrameDomain):
+                raise AssertionError(
+                    "Cannot convert this transformation to one with a "
+                    "SymmetricDifference output metric. This is probably "
+                    "a bug; please let us know about it so we can fix it!"
+                )
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                reference.identifier,
+                target,
+                HammingDistanceToSymmetricDifference(input_domain),
+                lambda *args: None,
+            )
+
+        transformation_generator: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric
+        }
+
+        return cls.Output(
+            *generate_nested_transformation(
+                transformation, reference.parent, transformation_generator
+            ),
+            constraints,
         )
-        return child | rename_transformation
 
-    @staticmethod
-    def _ensure_not_hamming(transformation: Transformation) -> Transformation:
-        """Convert transformation to one with a SymmetricDifference() output metric."""
-        if not isinstance(transformation.output_metric, HammingDistance):
-            return transformation
-        if not isinstance(transformation.output_domain, SparkDataFrameDomain):
+    def visit_private_source(self, expr) -> Output:
+        """Create a transformation from a PrivateSource query expression."""
+        ref = find_reference(expr.source_id, self.input_domain)
+        if ref is None:
+            named_tables = find_named_tables(self.input_domain)
+            raise ValueError(
+                f"Table '{expr.source_id}' does not exist. "
+                f"Available tables are: {named_tables}"
+            )
+        transformation = IdentityTransformation(self.input_metric, self.input_domain)
+        try:
+            constraints = self.table_constraints[ref.identifier]
+        except KeyError:
             raise AssertionError(
-                "Cannot convert this transformation to one with a "
-                "SymmetricDifference output metric. This is probably "
-                "a bug; please let us know about it so we can fix it!"
+                f"Table {ref.identifier} not present in constraints dictionary. "
+                "This is probably a bug; please let us know about it so we can fix it!"
             )
-        return transformation | HammingDistanceToSymmetricDifference(
-            transformation.output_domain
+        return self.Output(transformation, ref, constraints)
+
+    def visit_rename(self, expr: RenameExpr) -> Output:
+        """Create a transformation from a Rename query expression."""
+        child_transformation, child_ref, child_constraints = expr.child.accept(self)
+
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            input_domain = lookup_domain(child_transformation.output_domain, child_ref)
+            input_metric = lookup_metric(child_transformation.output_metric, child_ref)
+            if not isinstance(input_domain, SparkDataFrameDomain):
+                raise AssertionError(
+                    "Unrecognized input domain. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            if not isinstance(input_metric, (SymmetricDifference, IfGroupedBy)):
+                raise AssertionError(
+                    "Unrecognized input metric. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                RenameTransformation(input_domain, input_metric, expr.column_mapper),
+                lambda *args: None,
+            )
+
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            return RenameValueTransformation(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                expr.column_mapper,
+            )
+
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation, child_ref.parent, transformation_generators
+            ),
+            simplify_constraints(propagate_rename(expr, child_constraints)),
         )
 
-    def visit_filter(self, query: FilterExpr) -> Transformation:
+    def visit_filter(self, expr: FilterExpr) -> Output:
         """Create a transformation from a FilterExpr query expression."""
-        child = self._ensure_not_hamming(self._visit_child(query.child))
-        assert isinstance(child.output_domain, SparkDataFrameDomain)
-        assert isinstance(child.output_metric, (IfGroupedBy, SymmetricDifference))
-        transformation = FilterTransformation(
-            domain=child.output_domain,
-            metric=child.output_metric,
-            filter_expr=query.predicate,
+        child_transformation, child_ref, child_constraints = expr.child.accept(self)
+
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            input_domain = lookup_domain(child_transformation.output_domain, child_ref)
+            input_metric = lookup_metric(child_transformation.output_metric, child_ref)
+            if not isinstance(input_domain, SparkDataFrameDomain):
+                raise AssertionError(
+                    "Unrecognized input domain. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            if not isinstance(input_metric, (IfGroupedBy, SymmetricDifference)):
+                raise AssertionError(
+                    "Unrecognized input metric. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                FilterTransformation(input_domain, input_metric, expr.condition),
+                lambda *args: None,
+            )
+
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            return FilterValueTransformation(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                expr.condition,
+            )
+
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation, child_ref.parent, transformation_generators
+            ),
+            simplify_constraints(propagate_unmodified(expr, child_constraints)),
         )
-        return child | transformation
 
-    def visit_select(self, query: SelectExpr) -> Transformation:
+    def visit_select(self, expr: SelectExpr) -> Output:
         """Create a transformation from a Select query expression."""
-        child = self._visit_child(query.child)
-        assert isinstance(child.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            child.output_metric, (IfGroupedBy, SymmetricDifference, HammingDistance)
-        )
-        transformation = SelectTransformation(
-            input_domain=child.output_domain,
-            metric=child.output_metric,
-            columns=list(query.columns),
+        child_transformation, child_ref, child_constraints = expr.child.accept(self)
+
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            input_domain = lookup_domain(child_transformation.output_domain, child_ref)
+            input_metric = lookup_metric(child_transformation.output_metric, child_ref)
+
+            if not isinstance(input_domain, SparkDataFrameDomain):
+                raise AssertionError(
+                    "Unrecognized input domain. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            if not isinstance(
+                input_metric, (IfGroupedBy, SymmetricDifference, HammingDistance)
+            ):
+                raise AssertionError(
+                    "Unrecognized input metric. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                SelectTransformation(input_domain, input_metric, expr.columns),
+                lambda *args: None,
+            )
+
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            return SelectValueTransformation(
+                parent_domain, parent_metric, child_ref.identifier, target, expr.columns
+            )
+
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation, child_ref.parent, transformation_generators
+            ),
+            simplify_constraints(propagate_select(expr, child_constraints)),
         )
-        return child | transformation
 
-    def visit_map(self, query: MapExpr) -> Transformation:
+    def visit_map(self, expr: MapExpr) -> Output:
         """Create a transformation from a Map query expression."""
-        child = self._visit_child(query.child)
-        assert isinstance(child.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            child.output_metric, (IfGroupedBy, HammingDistance, SymmetricDifference)
-        )
-        transformer_input_domain = SparkRowDomain(child.output_domain.schema)
+        child_transformation, child_ref, child_constraints = expr.child.accept(self)
+
+        input_domain = lookup_domain(child_transformation.output_domain, child_ref)
+        if not isinstance(input_domain, SparkDataFrameDomain):
+            raise AssertionError(
+                "Unrecognized input domain. This is probably a bug; "
+                "please let us know about it so we can fix it!"
+            )
+        transformer_input_domain = SparkRowDomain(input_domain.schema)
         # Any new column created by Map could contain a null value
         spark_columns_descriptor = {
             k: dataclasses.replace(v, allow_null=True)
             for k, v in analytics_to_spark_columns_descriptor(
-                query.schema_new_columns
+                expr.schema_new_columns
             ).items()
         }
-        if query.augment:
+
+        if expr.augment:
             output_schema = {
                 **transformer_input_domain.schema,
                 **spark_columns_descriptor,
             }
         else:
             output_schema = spark_columns_descriptor
-        output_domain = SparkRowDomain(output_schema)
 
+        output_domain = SparkRowDomain(output_schema)
         # If you change `getattr(query, "f")` below to `query.f`,
-        # mypy will complain at you
-        transformation = MapTransformation(
-            metric=child.output_metric,
-            row_transformer=RowToRowTransformation(
-                input_domain=transformer_input_domain,
-                output_domain=output_domain,
-                trusted_f=getattr(query, "f"),
-                augment=query.augment,
-            ),
+        # mypy will be upset
+        transformer = RowToRowTransformation(
+            input_domain=transformer_input_domain,
+            output_domain=output_domain,
+            trusted_f=getattr(expr, "f"),
+            augment=expr.augment,
         )
-        return child | transformation
 
-    def inner_metric(self) -> Union[SumOf, RootSumOfSquared]:
-        """Get the inner metric used by this TransformationVisitor."""
-        if self.mechanism in (NoiseMechanism.LAPLACE, NoiseMechanism.GEOMETRIC):
-            return SumOf(SymmetricDifference())
-        else:
-            if self.mechanism != NoiseMechanism.DISCRETE_GAUSSIAN:
-                raise RuntimeError(
-                    f"Unsupported mechanism {self.mechanism}. "
-                    "Supported mechanisms are "
-                    f"{NoiseMechanism.DISCRETE_GAUSSIAN}, "
-                    f"{NoiseMechanism.LAPLACE}, and"
-                    f"{NoiseMechanism.GEOMETRIC}."
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            input_metric = lookup_metric(child_transformation.output_metric, child_ref)
+            if not isinstance(
+                input_metric, (IfGroupedBy, SymmetricDifference, HammingDistance)
+            ):
+                raise AssertionError(
+                    "Unrecognized input metric. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
                 )
-            return RootSumOfSquared(SymmetricDifference())
 
-    def visit_flat_map(self, query: FlatMapExpr) -> Transformation:
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                MapTransformation(metric=input_metric, row_transformer=transformer),
+                lambda *args: None,
+            )
+
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            if not expr.augment:
+                raise ValueError(
+                    "Maps on tables with the AddRowsWithID protected change "
+                    "must be augmenting"
+                )
+            return MapValueTransformation(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                row_transformer=transformer,
+            )
+
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation, child_ref.parent, transformation_generators
+            ),
+            simplify_constraints(propagate_map(expr, child_constraints)),
+        )
+
+    def visit_flat_map(self, expr: FlatMapExpr) -> Output:
         """Create a transformation from a FlatMap query expression."""
-        child = self._visit_child(query.child)
-        assert isinstance(child.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            child.output_metric, (IfGroupedBy, HammingDistance, SymmetricDifference)
+        child_transformation, child_ref, child_constraints = self._ensure_not_hamming(
+            *expr.child.accept(self)
         )
 
-        transformer_input_domain = SparkRowDomain(child.output_domain.schema)
+        input_domain = lookup_domain(child_transformation.output_domain, child_ref)
+        if not isinstance(input_domain, SparkDataFrameDomain):
+            raise AssertionError(
+                "Unrecognized input domain. This is probably a bug; "
+                "please let us know about it so we can fix it!"
+            )
+        transformer_input_domain = SparkRowDomain(input_domain.schema)
         # Any new column created by FlatMap could contain a null value
         spark_columns_descriptor = {
             k: dataclasses.replace(v, allow_null=True)
             for k, v in analytics_to_spark_columns_descriptor(
-                query.schema_new_columns
+                expr.schema_new_columns
             ).items()
         }
-        if query.augment:
+
+        if expr.augment:
             output_schema = {
                 **transformer_input_domain.schema,
                 **spark_columns_descriptor,
             }
         else:
             output_schema = spark_columns_descriptor
+
         output_domain = ListDomain(SparkRowDomain(output_schema))
 
-        # If you change `getattr(query, "f")` below to `query.f`,
-        # mypy will complain at you
         row_transformer = RowToRowsTransformation(
             input_domain=transformer_input_domain,
             output_domain=output_domain,
-            trusted_f=getattr(query, "f"),
-            augment=query.augment,
+            trusted_f=getattr(expr, "f"),
+            augment=expr.augment,
         )
 
-        transformation: Transformation
-        if query.schema_new_columns.grouping_column is not None:
-            transformation = GroupingFlatMap(
-                output_metric=self.inner_metric(),  # (sqrt) sum of (squared) symm diff
-                row_transformer=row_transformer,
-                max_num_rows=query.max_num_rows,
-            )
-        else:
-            child = self._ensure_not_hamming(child)
-            assert isinstance(child.output_domain, SparkDataFrameDomain)
-            assert isinstance(child.output_metric, (IfGroupedBy, SymmetricDifference))
-
-            transformation = FlatMapTransformation(
-                metric=child.output_metric,
-                row_transformer=row_transformer,
-                max_num_rows=query.max_num_rows,
-            )
-        return child | transformation
-
-    def visit_join_private(self, query: JoinPrivateExpr) -> Transformation:
-        """Create a transformation from a JoinPrivate query expression."""
-        child = self._visit_child(query.child)
-        left_metric, left_transformation = (child.output_metric, child)
-
-        # Check that left metrics are correct
-        if isinstance(left_metric, IfGroupedBy):
-            raise ValueError(
-                "Left operand used a grouping transformation. "
-                "This is not yet supported for private joins."
-            )
-        if isinstance(left_metric, HammingDistance):
-            if not isinstance(left_transformation.output_domain, SparkDataFrameDomain):
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            if expr.max_num_rows is None:
+                raise ValueError(
+                    "Flat maps on tables without IDs must have a defined max_num_rows"
+                    " parameter."
+                )
+            input_metric = lookup_metric(child_transformation.output_metric, child_ref)
+            if not isinstance(input_metric, (IfGroupedBy, SymmetricDifference)):
                 raise AssertionError(
-                    "Left operand has an unsupported "
-                    "output domain. This is probably a bug; please let us "
-                    "know about it so we can fix it!"
+                    "Unrecognized input metric. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
                 )
-            left_transformation = (
-                left_transformation
-                | HammingDistanceToSymmetricDifference(
-                    left_transformation.output_domain
+            transformation: Transformation
+            if expr.schema_new_columns.grouping_column is not None:
+                transformation = GroupingFlatMap(
+                    output_metric=self.inner_metric(),
+                    row_transformer=row_transformer,
+                    max_num_rows=expr.max_num_rows,
+                )
+            else:
+                transformation = FlatMapTransformation(
+                    metric=input_metric,
+                    row_transformer=row_transformer,
+                    max_num_rows=expr.max_num_rows,
                 )
-            )
-        if left_transformation.output_metric != SymmetricDifference():
-            raise ValueError(
-                "Left operand has an unsupported output metric. "
-                "The only supported output metrics are "
-                f"{SymmetricDifference()} and {HammingDistance()}"
-            )
-
-        current_keys = [str(k) for k in self.input_domain.key_to_domain.keys()]
-        left_output_key = get_nonconflicting_string(current_keys)
-        right_output_key = get_nonconflicting_string(current_keys + [left_output_key])
 
-        add_left_transformation = AugmentDictTransformation(
-            left_transformation
-            | CreateDictFromValue(
-                input_domain=left_transformation.output_domain,
-                input_metric=left_transformation.output_metric,
-                key=left_output_key,
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                transformation,
+                lambda *args: None,
             )
-        )
-        # input = {left_input, right_input},
-        # output = {left_input, right_input, left_output}
 
-        if not isinstance(add_left_transformation.output_domain, DictDomain):
-            raise AssertionError(
-                "Left transformation output domain has the wrong type. "
-                "This is probably a bug; please let us know so we can "
-                "fix it!"
-            )
-        if not isinstance(add_left_transformation.output_metric, DictMetric):
-            raise AssertionError(
-                "Left transformation output metric has the wrong type. "
-                "This is probably a bug; please let us know so we can "
-                "fix it!"
-            )
-        # Get right operand transformation
-        right_visitor = TransformationVisitor(
-            input_domain=add_left_transformation.output_domain,
-            input_metric=add_left_transformation.output_metric,
-            mechanism=self.mechanism,
-            public_sources=self.public_sources,
-        )
-        right_transformation = query.right_operand_expr.accept(right_visitor)
-        if not isinstance(right_transformation, Transformation):
-            raise AssertionError(
-                "Right operand does not produce a transformation. "
-                "This is probably a bug; please let us know so we can "
-                "fix it!"
-            )
-        # Check that right metrics are correct
-        if isinstance(right_transformation.output_metric, IfGroupedBy):
-            raise ValueError(
-                "Right operand used a grouping transformation. "
-                "This is not yet supported for private joins."
-            )
-        if not isinstance(right_transformation.output_domain, SparkDataFrameDomain):
-            raise AssertionError(
-                "Right operand has an output domain other than "
-                "SparkDataFrameDomain. This is probably a bug; "
-                "please let us know so we can fix it!"
-            )
-        if isinstance(right_transformation.output_metric, HammingDistance):
-            right_transformation = (
-                right_transformation
-                | HammingDistanceToSymmetricDifference(
-                    right_transformation.output_domain
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            if not expr.augment:
+                raise ValueError(
+                    "Flat maps on tables with the AddRowsWithID protected change "
+                    "must be augmenting"
                 )
-            )
-        if right_transformation.output_metric != SymmetricDifference():
-            raise AssertionError(
-                "Right operand has an output metric other than "
-                "SymmetricDifference. This is probably a bug; "
-                "please let us know so we can fix it!"
+            if expr.schema_new_columns.grouping_column is not None:
+                raise ValueError(
+                    "Flat maps on tables with the AddRowsWithID protected "
+                    "change cannot be grouping"
+                )
+            if expr.max_num_rows is not None:
+                warnings.warn(
+                    "When performing a flat map on a table with the AddRowsWithID "
+                    "ProtectedChange(), the max_num_rows parameter "
+                    "is not required and will be ignored."
+                )
+            return FlatMapValueTransformation(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                row_transformer=row_transformer,
+                max_num_rows=expr.max_num_rows,
             )
 
-        add_right_transformation = AugmentDictTransformation(
-            right_transformation
-            | CreateDictFromValue(
-                input_domain=right_transformation.output_domain,
-                input_metric=right_transformation.output_metric,
-                key=right_output_key,
-            )
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation, child_ref.parent, transformation_generators
+            ),
+            simplify_constraints(propagate_flat_map(expr, child_constraints)),
         )
-        # input = {left_input, right_input, left_output},
-        # output = {left_input, right_input, left_output, right_output}
 
-        combined_transformations = add_left_transformation | add_right_transformation
-        # input = {left_input, right_input},
-        # output = {left_input, right_input, left_output, right_output}
+    def visit_join_private(self, expr: JoinPrivateExpr) -> Output:
+        """Create a transformation from a JoinPrivate query expression."""
+        left_transformation, left_ref, left_constraints = expr.child.accept(self)
+        right_visitor = TransformationVisitor(
+            left_transformation.output_domain,
+            left_transformation.output_metric,
+            self.mechanism,
+            self.public_sources,
+            self.table_constraints,
+        )
+        (
+            right_transformation,
+            right_ref,
+            right_constraints,
+        ) = expr.right_operand_expr.accept(right_visitor)
 
-        if not isinstance(combined_transformations.output_domain, DictDomain):
-            raise AssertionError(
-                "Combined transformation has an unrecognized "
-                "output domain. This is probably a bug; "
-                "please let us know so we can fix it! "
-            )
-        if not isinstance(combined_transformations.output_metric, DictMetric):
-            raise AssertionError(
-                "Combined transformation has an unrecognized "
-                "output metric. This is probably a bug; "
-                "please let us know so we can fix it!"
+        if left_ref.parent != right_ref.parent:
+            raise ValueError(
+                "Left and right tables must be initialized with compatible "
+                f"ProtectedChange() descriptions, but {left_ref} and {right_ref} "
+                "were not."
             )
-        previous_transformation = combined_transformations | Subset(
-            input_domain=combined_transformations.output_domain,
-            input_metric=combined_transformations.output_metric,
-            keys=[left_output_key, right_output_key],
-        )
-        # input = {left_input, right_input}, output = {left_output, right_output}
 
-        # Create the PrivateJoin transformation
-        previous_domain = previous_transformation.output_domain
-        if not isinstance(previous_domain, DictDomain):
-            raise AssertionError("This is a bug. Please let us know so we can fix it!")
-        left_domain = previous_domain.key_to_domain[left_output_key]
-        right_domain = previous_domain.key_to_domain[right_output_key]
+        child_transformation = left_transformation | right_transformation
+        left_domain = lookup_domain(child_transformation.output_domain, left_ref)
+        right_domain = lookup_domain(child_transformation.output_domain, right_ref)
         if not isinstance(left_domain, SparkDataFrameDomain):
-            raise ValueError(
-                "Left operand has an output domain that is not a SparkDataFrameDomain."
+            raise AssertionError(
+                "Unrecognized input domain. This is probably a bug; "
+                "please let us know about it so we can fix it!"
             )
         if not isinstance(right_domain, SparkDataFrameDomain):
-            raise ValueError(
-                "Right operand has an output domain that is not a SparkDataFrameDomain."
+            raise AssertionError(
+                "Unrecognized input domain. This is probably a bug; "
+                "please let us know about it so we can fix it!"
             )
 
-        def get_core_truncation_strategy(
+        def get_truncation_params(
             strategy: TruncationStrategy.Type,
-        ) -> CoreTruncationStrategy:
+        ) -> Tuple[CoreTruncationStrategy, int]:
             if isinstance(strategy, TruncationStrategy.DropExcess):
-                return CoreTruncationStrategy.TRUNCATE
+                return CoreTruncationStrategy.TRUNCATE, strategy.max_records
             elif isinstance(strategy, TruncationStrategy.DropNonUnique):
-                return CoreTruncationStrategy.DROP
+                return CoreTruncationStrategy.DROP, 1
             else:
-                # This will be triggered if an end user tries to implement their own
-                # subclass of TruncationStrategy, or if this function is not updated
-                # when a new TruncationStrategy variant is added to the
-                # library. Unfortunately, because TruncationStrategy is not an enum
-                # it isn't possible to use the mypy assert_never trick to check that
-                # this is exhaustive.
                 raise ValueError(
                     f"Truncation strategy type {strategy.__class__.__qualname__} "
                     "is not supported."
                 )
 
-        def get_truncation_threshold(strategy: TruncationStrategy.Type) -> int:
-            if isinstance(strategy, TruncationStrategy.DropExcess):
-                return strategy.max_records
-            elif isinstance(strategy, TruncationStrategy.DropNonUnique):
-                return 1
-            else:
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            if (
+                expr.truncation_strategy_left is None
+                or expr.truncation_strategy_right is None
+            ):
                 raise ValueError(
-                    f"Truncation strategy type {strategy.__class__.__qualname__} "
-                    "is not supported."
+                    "When joining without IDs, truncation strategies are required."
                 )
-
-        join_on_nulls: bool = any(
-            [v.allow_null for v in dict(left_domain.schema).values()]
-            + [v.allow_null for v in dict(right_domain.schema).values()]
-        )
-        if query.join_columns is not None:
-            join_on_nulls = any(
-                [
-                    (left_domain[col].allow_null and right_domain[col].allow_null)
-                    for col in query.join_columns
-                ]
+            l_trunc_strat, l_trunc_threshold = get_truncation_params(
+                expr.truncation_strategy_left
             )
-
-        transformation = PrivateJoinTransformation(
-            input_domain=previous_domain,
-            left_key=left_output_key,
-            right_key=right_output_key,
-            left_truncation_strategy=get_core_truncation_strategy(
-                query.truncation_strategy_left
-            ),
-            right_truncation_strategy=get_core_truncation_strategy(
-                query.truncation_strategy_right
-            ),
-            left_truncation_threshold=get_truncation_threshold(
-                query.truncation_strategy_left
-            ),
-            right_truncation_threshold=get_truncation_threshold(
-                query.truncation_strategy_right
+            r_trunc_strat, r_trunc_threshold = get_truncation_params(
+                expr.truncation_strategy_right
+            )
+            subset = Subset(
+                parent_domain,
+                parent_metric,
+                [left_ref.identifier, right_ref.identifier],
+            )
+            if not isinstance(subset.output_domain, DictDomain):
+                raise AssertionError(
+                    "Unrecognized input domain. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            join = PrivateJoinTransformation(
+                input_domain=subset.output_domain,
+                left_key=left_ref.identifier,
+                right_key=right_ref.identifier,
+                left_truncation_strategy=l_trunc_strat,
+                right_truncation_strategy=r_trunc_strat,
+                left_truncation_threshold=l_trunc_threshold,
+                right_truncation_threshold=r_trunc_threshold,
+                join_cols=expr.join_columns,
+                join_on_nulls=True,
+            )
+            create_dict = CreateDictFromValue(
+                join.output_domain, join.output_metric, key=target
+            )
+            return AugmentDictTransformation(subset | join | create_dict)
+
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            if (expr.truncation_strategy_left is not None) or (
+                expr.truncation_strategy_right is not None
+            ):
+                warnings.warn(
+                    "When joining with IDs, truncation strategies are not required."
+                    " Provided truncation parameters will be ignored."
+                )
+            return PrivateJoinOnKeyTransformation(
+                parent_domain,
+                parent_metric,
+                left_ref.identifier,
+                right_ref.identifier,
+                target,
+                expr.join_columns,
+                join_on_nulls=True,
+            )
+
+        common_cols = set(left_domain.schema) & set(right_domain.schema)
+        join_cols = set(expr.join_columns or common_cols)
+        overlapping_cols = common_cols - join_cols
+        constraints = propagate_join_private(
+            join_cols, overlapping_cols, left_constraints, right_constraints
+        )
+
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation,
+                # right_ref.parent and left_ref.parent must be the same,
+                # so either works here.
+                right_ref.parent,
+                transformation_generators,
             ),
-            join_cols=query.join_columns,
-            join_on_nulls=join_on_nulls,
+            simplify_constraints(constraints),
         )
-        return previous_transformation | transformation
 
-    def visit_join_public(self, query: JoinPublicExpr) -> Transformation:
+    def visit_join_public(self, expr: JoinPublicExpr) -> Output:
         """Create a transformation from a JoinPublic query expression."""
+        child_transformation, child_ref, child_constraints = self._ensure_not_hamming(
+            *self._visit_child(expr.child)
+        )
+
         public_df: DataFrame
-        if isinstance(query.public_table, str):
+        if isinstance(expr.public_table, str):
             try:
-                public_df = self.public_sources[query.public_table]
+                public_df = self.public_sources[expr.public_table]
             except KeyError:
                 raise ValueError(
-                    "There is no public source with the identifier "
-                    f"{query.public_table}"
+                    f"There is no public source with the identifier {expr.public_table}"
                 )
         else:
-            public_df = query.public_table
-
-        child = self._ensure_not_hamming(self._visit_child(query.child))
-        assert isinstance(child.output_domain, SparkDataFrameDomain)
-        assert isinstance(child.output_metric, (IfGroupedBy, SymmetricDifference))
+            public_df = expr.public_table
 
         public_df_schema = Schema(spark_schema_to_analytics_columns(public_df.schema))
-        transformation = PublicJoinTransformation(
-            input_domain=SparkDataFrameDomain(child.output_domain.schema),
-            public_df=public_df,
-            public_df_domain=SparkDataFrameDomain(
-                analytics_to_spark_columns_descriptor(public_df_schema)
-            ),
-            join_cols=list(query.join_columns) if query.join_columns else None,
-            metric=child.output_metric,
-            join_on_nulls=any(
-                [
-                    public_df_schema[col].allow_null
-                    for col in list(public_df_schema.keys())
-                ]
-            ),
-        )
-        return child | transformation
 
-    def visit_replace_null_and_nan(self, query: ReplaceNullAndNan) -> Transformation:
-        """Create a transformation from a ReplaceNullAndNan query expression."""
-        child = self._visit_child(query.child)
-        assert isinstance(child.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            child.output_metric, (IfGroupedBy, HammingDistance, SymmetricDifference)
+        join_null_cols = any(
+            public_df_schema[col].allow_null for col in public_df_schema.keys()
         )
-        grouping_column: Optional[str] = None
-        if isinstance(child.output_metric, IfGroupedBy):
-            grouping_column = child.output_metric.column
-            if grouping_column in query.replace_with:
-                raise ValueError(
-                    "Cannot replace null values in column"
-                    f" {child.output_metric.column}, because it is being used as a"
-                    " grouping column"
+
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            input_domain = lookup_domain(child_transformation.output_domain, child_ref)
+            input_metric = lookup_metric(child_transformation.output_metric, child_ref)
+            if not isinstance(input_domain, SparkDataFrameDomain):
+                raise AssertionError(
+                    "Unrecognized input domain. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
                 )
-        analytics_schema = spark_dataframe_domain_to_analytics_columns(
-            child.output_domain
+            if not isinstance(input_metric, (IfGroupedBy, SymmetricDifference)):
+                raise AssertionError(
+                    "Unrecognized input metric. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                PublicJoinTransformation(
+                    input_domain=SparkDataFrameDomain(input_domain.schema),
+                    public_df=public_df,
+                    public_df_domain=SparkDataFrameDomain(
+                        analytics_to_spark_columns_descriptor(public_df_schema)
+                    ),
+                    join_cols=expr.join_columns if expr.join_columns else None,
+                    metric=input_metric,
+                    join_on_nulls=join_null_cols,
+                ),
+                lambda *args: None,
+            )
+
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            return PublicJoinValueTransformation(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                public_df,
+                SparkDataFrameDomain(
+                    analytics_to_spark_columns_descriptor(public_df_schema)
+                ),
+                expr.join_columns,
+                join_on_nulls=join_null_cols,
+            )
+
+        child_domain = lookup_domain(child_transformation.output_domain, child_ref)
+        if not isinstance(child_domain, SparkDataFrameDomain):
+            raise AssertionError(
+                "Unrecognized input domain. This is probably a bug; "
+                "please let us know about it so we can fix it!"
+            )
+
+        common_cols = set(child_domain.schema) & set(public_df_schema)
+        join_cols = set(expr.join_columns or common_cols)
+        overlapping_cols = common_cols - join_cols
+        constraints = propagate_join_public(
+            join_cols, overlapping_cols, public_df, child_constraints
+        )
+
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation, child_ref.parent, transformation_generators
+            ),
+            simplify_constraints(constraints),
         )
 
-        replace_with: Dict[str, Any] = dict(query.replace_with).copy()
+    @staticmethod
+    def _get_replace_with(
+        expr: ReplaceNullAndNan,
+        analytics_schema: Dict[str, ColumnDescriptor],
+        grouping_column: Optional[str] = None,
+    ) -> Dict[str, Any]:
+        replace_with: Dict[str, Any] = dict(expr.replace_with).copy()
         if len(replace_with) == 0:
-            for col in list(Schema(analytics_schema).column_descs.keys()):
+            for col in Schema(analytics_schema).column_descs:
                 if col == grouping_column:
                     continue
                 if not analytics_schema[col].allow_null and not (
                     analytics_schema[col].allow_nan
                 ):
                     continue
                 if analytics_schema[col].column_type == ColumnType.INTEGER:
@@ -647,185 +954,452 @@
             for col in replace_with:
                 if not col in analytics_schema:
                     raise ValueError(
                         f"Cannot replace values in column {col}, because it is not in"
                         " the schema"
                     )
             # Make sure all DECIMAL replacement values are floats
-            for col in list(replace_with.keys()):
+            for col in replace_with.keys():
                 if analytics_schema[col].column_type == ColumnType.DECIMAL:
                     replace_with[col] = float(replace_with[col])
 
-        also_replace_nan = any(
-            [
-                (
-                    analytics_schema[col].column_type == ColumnType.DECIMAL
-                    and analytics_schema[col].allow_nan
+        return replace_with
+
+    def visit_replace_null_and_nan(self, expr: ReplaceNullAndNan) -> Output:
+        """Create a transformation from a ReplaceNullAndNan query expression."""
+        child_transformation, child_ref, child_constraints = self._visit_child(
+            expr.child
+        )
+        input_domain = lookup_domain(child_transformation.output_domain, child_ref)
+        input_metric = lookup_metric(child_transformation.output_metric, child_ref)
+        if not isinstance(input_domain, SparkDataFrameDomain):
+            raise AssertionError(
+                "Unrecognized input domain. This is probably a bug; "
+                "please let us know about it so we can fix it!"
+            )
+        if not isinstance(
+            input_metric, (IfGroupedBy, HammingDistance, SymmetricDifference)
+        ):
+            raise AssertionError(
+                "Unrecognized input metric. This is probably a bug; "
+                "please let us know about it so we can fix it!"
+            )
+        grouping_column: Optional[str] = None
+        if isinstance(input_metric, IfGroupedBy):
+            grouping_column = input_metric.column
+            if grouping_column in expr.replace_with:
+                raise ValueError(
+                    "Cannot replace null values in column"
+                    f" {input_metric.column}, because it is being used as a"
+                    " grouping column"
                 )
-                for col in list(replace_with.keys())
-            ]
+        analytics_schema = spark_dataframe_domain_to_analytics_columns(input_domain)
+
+        replace_with = self._get_replace_with(expr, analytics_schema, grouping_column)
+
+        replace_null = any(analytics_schema[col].allow_null for col in replace_with)
+
+        replace_nan = any(
+            analytics_schema[col].column_type == ColumnType.DECIMAL
+            and analytics_schema[col].allow_nan
+            for col in replace_with.keys()
         )
 
-        transformation: Transformation = child
+        null_replace_map = {
+            col: val
+            for col, val in replace_with.items()
+            if analytics_schema[col].allow_null
+        }
 
-        if any([analytics_schema[col].allow_null for col in replace_with]):
-            transformation = transformation | ReplaceNulls(
-                input_domain=child.output_domain,
-                metric=child.output_metric,
-                replace_map={
-                    col: val
-                    for col, val in replace_with.items()
-                    if analytics_schema[col].allow_null
-                },
-            )
-        if also_replace_nan:
-            # These assertions are here to make MyPy happy
-            # If they fail, something is very wrong in Core
-            assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-            assert isinstance(
-                transformation.output_metric,
-                (IfGroupedBy, HammingDistance, SymmetricDifference),
-            )
-            replace_nan = ReplaceNaNs(
-                input_domain=transformation.output_domain,
-                metric=transformation.output_metric,
-                replace_map={
-                    col: replace_with[col]
-                    for col in list(replace_with.keys())
-                    if (
-                        analytics_schema[col].column_type == ColumnType.DECIMAL
-                        and analytics_schema[col].allow_nan
-                    )
-                },
+        nan_replace_map = {
+            col: replace_with[col]
+            for col in replace_with.keys()
+            if (
+                analytics_schema[col].column_type == ColumnType.DECIMAL
+                and analytics_schema[col].allow_nan
             )
-            transformation = transformation | replace_nan
-        return transformation
+        }
+
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            transformation: Transformation = IdentityTransformation(
+                input_metric, input_domain
+            )
+            if replace_null:
+                assert isinstance(input_domain, SparkDataFrameDomain)
+                assert isinstance(
+                    input_metric, (IfGroupedBy, HammingDistance, SymmetricDifference)
+                )
+                transformation |= ReplaceNullsTransformation(
+                    input_domain=input_domain,
+                    metric=input_metric,
+                    replace_map=null_replace_map,
+                )
+            if replace_nan:
+                assert isinstance(transformation.output_domain, SparkDataFrameDomain)
+                assert isinstance(
+                    transformation.output_metric,
+                    (IfGroupedBy, HammingDistance, SymmetricDifference),
+                )
+                transformation |= ReplaceNaNsTransformation(
+                    input_domain=transformation.output_domain,
+                    metric=transformation.output_metric,
+                    replace_map=nan_replace_map,
+                )
 
-    def visit_replace_infinity(self, query: ReplaceInfinity) -> Transformation:
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                transformation,
+                lambda *args: None,
+            )
+
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            transformation: Transformation = IdentityTransformation(
+                parent_metric, parent_domain
+            )
+            temp_table_id = TemporaryTable()
+
+            if replace_null:
+                transformation |= ReplaceNullsValueTransformation(
+                    parent_domain,
+                    parent_metric,
+                    child_ref.identifier,
+                    temp_table_id if replace_nan else target,
+                    replace_map=null_replace_map,
+                )
+
+            if replace_nan:
+                assert isinstance(transformation.output_domain, DictDomain)
+                assert isinstance(transformation.output_metric, AddRemoveKeys)
+                transformation |= ReplaceNaNsValueTransformation(
+                    transformation.output_domain,
+                    transformation.output_metric,
+                    temp_table_id if replace_null else child_ref.identifier,
+                    target,
+                    nan_replace_map,
+                )
+
+            if (not replace_null) and (not replace_nan):
+                # Rename that essentially does nothing
+                assert isinstance(transformation.output_domain, DictDomain)
+                assert isinstance(transformation.output_metric, AddRemoveKeys)
+                transformation |= RenameValueTransformation(
+                    transformation.output_domain,
+                    transformation.output_metric,
+                    child_ref.identifier,
+                    target,
+                    {},
+                )
+            return transformation
+
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation, child_ref.parent, transformation_generators
+            ),
+            simplify_constraints(propagate_replace(expr, child_constraints)),
+        )
+
+    def visit_replace_infinity(self, expr: ReplaceInfinity) -> Output:
         """Create a transformation from a ReplaceInfinity query expression."""
-        child = self._visit_child(query.child)
-        assert isinstance(child.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            child.output_metric, (IfGroupedBy, HammingDistance, SymmetricDifference)
+        child_transformation, child_ref, child_constraints = self._visit_child(
+            expr.child
         )
+        input_domain = lookup_domain(child_transformation.output_domain, child_ref)
+        input_metric = lookup_metric(child_transformation.output_metric, child_ref)
+
         analytics_schema = Schema(
-            spark_dataframe_domain_to_analytics_columns(child.output_domain)
+            spark_dataframe_domain_to_analytics_columns(input_domain)
         )
-        replace_with = query.replace_with.copy()
+        replace_with = expr.replace_with.copy()
         if len(replace_with) == 0:
             replace_with = {
                 col: (AnalyticsDefault.DECIMAL, AnalyticsDefault.DECIMAL)
                 for col in analytics_schema.column_descs
                 if analytics_schema[col].column_type == ColumnType.DECIMAL
             }
-        transformation = ReplaceInfs(
-            input_domain=child.output_domain,
-            metric=child.output_metric,
-            replace_map=replace_with,
-        )
-        return child | transformation
-
-    def visit_drop_infinity(self, query: DropInfExpr) -> Transformation:
-        """Create a transformation from a DropInfinity expression."""
-        child = self._visit_child(query.child)
+
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            if not isinstance(input_domain, SparkDataFrameDomain):
+                raise AssertionError(
+                    "Unrecognized input domain. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            if not isinstance(
+                input_metric, (IfGroupedBy, HammingDistance, SymmetricDifference)
+            ):
+                raise AssertionError(
+                    "Unrecognized input metric. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                ReplaceInfsTransformation(
+                    input_domain=input_domain,
+                    metric=input_metric,
+                    replace_map=replace_with,
+                ),
+                lambda *args: None,
+            )
+
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            return ReplaceInfsValueTransformation(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                replace_map=replace_with,
+            )
+
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation, child_ref.parent, transformation_generators
+            ),
+            simplify_constraints(propagate_replace(expr, child_constraints)),
+        )
+
+    def visit_drop_infinity(self, expr: DropInfExpr) -> Output:
+        """Create a transformation from a DropInfinity query expression."""
+        child_transformation, child_ref, child_constraints = self._ensure_not_hamming(
+            *self._visit_child(expr.child)
+        )
+        input_domain = lookup_domain(child_transformation.output_domain, child_ref)
+        input_metric = lookup_metric(child_transformation.output_metric, child_ref)
         analytics_schema = Schema(
-            spark_dataframe_domain_to_analytics_columns(child.output_domain)
+            spark_dataframe_domain_to_analytics_columns(input_domain)
         )
 
         grouping_column: Optional[str] = None
-        if isinstance(child.output_metric, IfGroupedBy):
-            grouping_column = child.output_metric.column
-            if grouping_column in query.columns:
+        if isinstance(input_metric, IfGroupedBy):
+            grouping_column = input_metric.column
+            if grouping_column in expr.columns:
                 raise ValueError(
                     "Cannot drop infinite values in column"
-                    f" {child.output_metric.column}, because it is being used as a"
+                    f" {input_metric.column}, because it is being used as a"
                     " grouping column"
                 )
 
-        columns = query.columns.copy()
+        columns = expr.columns.copy()
         if len(columns) == 0:
             columns = [
                 col
                 for col, cd in analytics_schema.column_descs.items()
                 if (cd.column_type == ColumnType.DECIMAL and cd.allow_inf)
                 and not (col == grouping_column)
             ]
         else:
             for col in columns:
                 if analytics_schema.column_descs[col].column_type != ColumnType.DECIMAL:
                     raise ValueError(
-                        "Cannot drop infinite values from column {col}, because that"
+                        f"Cannot drop infinite values from column {col}, because that"
                         " column's type is not DECIMAL"
                     )
 
-        transformation: Transformation = self._ensure_not_hamming(child)
-        # visit_child will raise an exception if these aren't true;
-        # these asserts are for mypy
-        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            transformation.output_metric, (IfGroupedBy, SymmetricDifference)
-        )
-        transformation = transformation | DropInfTransformation(
-            transformation.output_domain, transformation.output_metric, columns
-        )
-
-        return transformation
-
-    def visit_drop_null_and_nan(self, query: DropNullAndNan) -> Transformation:
-        """Create a transformation from a DropNullAndNan expression."""
-        child = self._visit_child(query.child)
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            if not isinstance(input_domain, SparkDataFrameDomain):
+                raise AssertionError(
+                    "Unrecognized input domain. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            if not isinstance(input_metric, (IfGroupedBy, SymmetricDifference)):
+                raise AssertionError(
+                    "Unrecognized input metric. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                DropInfTransformation(
+                    input_domain=input_domain, metric=input_metric, columns=columns
+                ),
+                lambda *args: None,
+            )
+
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            return DropInfsValueTransformation(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                columns=columns,
+            )
+
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation, child_ref.parent, transformation_generators
+            ),
+            simplify_constraints(propagate_unmodified(expr, child_constraints)),
+        )
+
+    def visit_drop_null_and_nan(self, expr: DropNullAndNan) -> Output:
+        """Create a transformation from a DropNullAndNan query expression."""
+        child_transformation, child_ref, child_constraints = self._ensure_not_hamming(
+            *self._visit_child(expr.child)
+        )
+        input_domain = lookup_domain(child_transformation.output_domain, child_ref)
+        input_metric = lookup_metric(child_transformation.output_metric, child_ref)
+
         analytics_schema = Schema(
-            spark_dataframe_domain_to_analytics_columns(child.output_domain)
+            spark_dataframe_domain_to_analytics_columns(input_domain)
         )
 
         grouping_column: Optional[str] = None
-        if isinstance(child.output_metric, IfGroupedBy):
-            grouping_column = child.output_metric.column
-            if grouping_column in query.columns:
+        if isinstance(input_metric, IfGroupedBy):
+            grouping_column = input_metric.column
+            if grouping_column in expr.columns:
                 raise ValueError(
                     "Cannot drop null values in column"
-                    f" {child.output_metric.column}, because it is being used as a"
+                    f" {input_metric.column}, because it is being used as a"
                     " grouping column"
                 )
 
-        columns = query.columns.copy()
+        columns = expr.columns.copy()
         if len(columns) == 0:
             columns = [
                 col
                 for col, cd in analytics_schema.column_descs.items()
                 if (cd.allow_null or cd.allow_nan) and not (col == grouping_column)
             ]
 
-        transformation: Transformation = self._ensure_not_hamming(child)
-        # visit_child will raise an exception if these aren't true;
-        # these asserts are for mypy
-        assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-        assert isinstance(
-            transformation.output_metric, (IfGroupedBy, SymmetricDifference)
-        )
         null_columns = [col for col in columns if analytics_schema[col].allow_null]
-        if len(null_columns) != 0:
-            transformation = transformation | DropNulls(
-                transformation.output_domain, transformation.output_metric, null_columns
-            )
+
         nan_columns = [col for col in columns if analytics_schema[col].allow_nan]
-        if len(nan_columns) != 0:
-            # Either a DropNulls transformation was created - for which these
-            # should always be true - or it wasn't, in which case we already
-            # checked these.
-            # These asserts are just here so mypy knows what types to expect.
-            assert isinstance(transformation.output_domain, SparkDataFrameDomain)
-            assert isinstance(
-                transformation.output_metric, (IfGroupedBy, SymmetricDifference)
-            )
-            transformation = transformation | DropNaNs(
-                transformation.output_domain, transformation.output_metric, nan_columns
+
+        def gen_transformation_dictmetric(parent_domain, parent_metric, target):
+            if not isinstance(input_domain, SparkDataFrameDomain):
+                raise AssertionError(
+                    "Unrecognized input domain. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            if not isinstance(input_metric, (IfGroupedBy, SymmetricDifference)):
+                raise AssertionError(
+                    "Unrecognized input metric. This is probably a bug; "
+                    "please let us know about it so we can fix it!"
+                )
+            transformation: Transformation = IdentityTransformation(
+                input_metric, input_domain
             )
 
-        return transformation
+            if null_columns:
+                transformation |= DropNullsTransformation(
+                    input_domain, input_metric, null_columns
+                )
+
+            if nan_columns:
+                assert isinstance(transformation.output_domain, SparkDataFrameDomain)
+                assert isinstance(
+                    transformation.output_metric, (IfGroupedBy, SymmetricDifference)
+                )
+                transformation |= DropNaNsTransformation(
+                    transformation.output_domain,
+                    transformation.output_metric,
+                    nan_columns,
+                )
+
+            return create_copy_and_transform_value(
+                parent_domain,
+                parent_metric,
+                child_ref.identifier,
+                target,
+                transformation,
+                lambda *args: None,
+            )
+
+        def gen_transformation_ark(parent_domain, parent_metric, target):
+            transformation: Transformation = IdentityTransformation(
+                parent_metric, parent_domain
+            )
+            temp_table_id = TemporaryTable()
+
+            if null_columns:
+                transformation |= DropNullsValueTransformation(
+                    parent_domain,
+                    parent_metric,
+                    child_ref.identifier,
+                    temp_table_id if nan_columns else target,
+                    null_columns,
+                )
+
+            if nan_columns:
+                assert isinstance(transformation.output_domain, DictDomain)
+                assert isinstance(transformation.output_metric, AddRemoveKeys)
+                transformation |= DropNaNsValueTransformation(
+                    transformation.output_domain,
+                    transformation.output_metric,
+                    temp_table_id if null_columns else child_ref.identifier,
+                    target,
+                    nan_columns,
+                )
+
+            if (not null_columns) and (not nan_columns):
+                # Rename that essentially does nothing
+                assert isinstance(transformation.output_domain, DictDomain)
+                assert isinstance(transformation.output_metric, AddRemoveKeys)
+                transformation |= RenameValueTransformation(
+                    transformation.output_domain,
+                    transformation.output_metric,
+                    child_ref.identifier,
+                    target,
+                    {},
+                )
+            return transformation
+
+        transformation_generators: Dict[Type[Metric], Callable] = {
+            DictMetric: gen_transformation_dictmetric,
+            AddRemoveKeys: gen_transformation_ark,
+        }
+
+        return self.Output(
+            *generate_nested_transformation(
+                child_transformation, child_ref.parent, transformation_generators
+            ),
+            simplify_constraints(propagate_unmodified(expr, child_constraints)),
+        )
+
+    def visit_enforce_constraint(self, expr: EnforceConstraint) -> Output:
+        """Create a transformation from an EnforceConstraint query expression."""
+        # Note: at present, enforcing one constraint can never invalidate
+        # another constraint, so just adding the new constraint to the list of
+        # constraints is perfectly fine. If a new constraint is added that can
+        # invalidate other constraints, this will have to be broken out into
+        # per-constraint-type logic.
+        child_transformation, child_ref, child_constraints = self._visit_child(
+            expr.child
+        )
+        # pylint: disable=protected-access
+        transformation, ref = expr.constraint._enforce(
+            child_transformation, child_ref, *expr.options
+        )
+        # pylint: enable=protected-access
+        return self.Output(
+            transformation,
+            ref,
+            simplify_constraints(child_constraints + [expr.constraint]),
+        )
 
     # None of the queries that produce measurements are implemented
     def visit_groupby_count(self, expr: GroupByCount) -> Any:
         """Visit a GroupByCount query expression (raises an error)."""
         raise NotImplementedError
 
     def visit_groupby_count_distinct(self, expr: GroupByCountDistinct) -> Any:
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/_schema.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/_schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Schema management for private and public tables.
 
 The schema represents the column types of the underlying table. This allows
 for seamless transitions of the data representation type.
 """
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 import datetime
 from collections.abc import Mapping
 from dataclasses import dataclass
 from enum import Enum
 from typing import Dict, Iterator, List
 from typing import Mapping as MappingType
@@ -26,14 +26,15 @@
     StructField,
     StructType,
     TimestampType,
 )
 
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.spark_domains import (
+    SparkColumnDescriptor,
     SparkColumnsDescriptor,
     SparkDataFrameDomain,
     SparkDateColumnDescriptor,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
     SparkTimestampColumnDescriptor,
@@ -89,37 +90,52 @@
       INTEGER, DECIMAL, VARCHAR, DATE, TIMESTAMP
     """
 
     def __init__(
         self,
         column_descs: MappingType[str, Union[str, ColumnType, ColumnDescriptor]],
         grouping_column: Optional[str] = None,
+        id_column: Optional[str] = None,
+        id_space: Optional[str] = None,
         default_allow_null: bool = False,
         default_allow_nan: bool = False,
         default_allow_inf: bool = False,
     ):
         """Constructor.
 
         Args:
             column_descs: Mapping from column names to supported types.
             grouping_column: Optional column that must be grouped by in this query.
+            id_column: The ID column on this table, if one exists.
+            id_space: The ID space for this table, if one exists.
             default_allow_null: When a ColumnType or string is used as the value
                 in the ColumnDescriptors mapping, the column will allow_null if
                 default_allow_null is True.
             default_allow_nan: When a ColumnType or string is used as the value
                 in the ColumnDescriptors mapping, the column will allow_nan if
                 default_allow_nan is True.
             default_allow_inf: When a ColumnType or string is used as the value
                 in the ColumnDescriptors mapping, the column will allow_inf if
                 default_allow_inf is True.
         """
         # TODO(#1539): update Schema interface to use ColumnDescriptor everywhere.
         if "" in column_descs:
             raise ValueError('"" (the empty string) is not a supported column name')
+        if grouping_column is not None and grouping_column not in column_descs:
+            raise KeyError(
+                f"Grouping column '{grouping_column}' is not one of the provided"
+                " columns"
+            )
         self._grouping_column = grouping_column
+        if id_column is not None and id_column not in column_descs:
+            raise KeyError(
+                f"ID column '{id_column}' is not one of the provided columns"
+            )
+        self._id_column = id_column
+        self._id_space = id_space
 
         supported_types: List[str] = [t.name for t in list(ColumnType)]
         column_types: List[str] = []
         for cd in column_descs.values():
             if isinstance(cd, ColumnDescriptor):
                 column_types.append(cd.column_type.name)
             elif isinstance(cd, ColumnType):
@@ -128,18 +144,15 @@
                 column_types.append(cd)
         invalid_types = set(column_types) - set(supported_types)
         if invalid_types:
             raise ValueError(
                 f"Column types {invalid_types} not supported; "
                 f"use supported types {supported_types}."
             )
-        if grouping_column is not None and grouping_column not in column_descs:
-            raise KeyError(
-                f"grouping_column ({grouping_column}) is not in column_descs"
-            )
+
         self._column_descs: Dict[str, ColumnDescriptor] = {}
         for col, ty in column_descs.items():
             if isinstance(ty, ColumnDescriptor):
                 self._column_descs[col] = ty
             elif isinstance(ty, ColumnType):
                 self._column_descs[col] = ColumnDescriptor(
                     ty,
@@ -167,24 +180,36 @@
         return {col: desc.column_type.name for col, desc in self.column_descs.items()}
 
     @property
     def grouping_column(self) -> Optional[str]:
         """Returns the optional column that must be grouped by."""
         return self._grouping_column
 
+    @property
+    def id_column(self) -> Optional[str]:
+        """Return whether the grouping column is an ID column."""
+        return self._id_column
+
+    @property
+    def id_space(self) -> Optional[str]:
+        """Return the ID space for this schema."""
+        return self._id_space
+
     def __eq__(self, other: object) -> bool:
         """Returns True if schemas are equal.
 
         Args:
             other: Schema to check against.
         """
         if isinstance(other, Schema):
             return (
                 self.column_descs == other.column_descs
                 and self.grouping_column == other.grouping_column
+                and self.id_column == other.id_column
+                and self.id_space == other.id_space
             )
         return False
 
     def __getitem__(self, column: str) -> ColumnDescriptor:
         """Returns the data type for the given column.
 
         Args:
@@ -198,19 +223,23 @@
 
     def __len__(self) -> int:
         """Return the number of columns in the schema."""
         return len(self.column_descs)
 
     def __repr__(self) -> str:
         """Return a string representation of self."""
+        out = f"Schema({self.column_descs}"
         if self.grouping_column:
-            return (
-                f"Schema({self.column_descs}, grouping_column='{self.grouping_column}')"
-            )
-        return f"Schema({self.column_descs})"
+            out += f", grouping_column={self.grouping_column}"
+        if self.id_column:
+            out += f", id_column={self.id_column}"
+        if self.id_space:
+            out += f", id_space={self.id_space}"
+        out += ")"
+        return out
 
 
 _SPARK_TO_ANALYTICS: Dict[DataType, ColumnType] = {
     IntegerType(): ColumnType.INTEGER,
     LongType(): ColumnType.INTEGER,
     DoubleType(): ColumnType.DECIMAL,
     FloatType(): ColumnType.DECIMAL,
@@ -269,15 +298,15 @@
     )
 
 
 def analytics_to_spark_columns_descriptor(
     analytics_schema: Schema,
 ) -> SparkColumnsDescriptor:
     """Convert a schema in Analytics representation to a Spark columns descriptor."""
-    out: SparkColumnsDescriptor = {}
+    out: Dict[str, SparkColumnDescriptor] = {}
     for column_name, column_desc in analytics_schema.column_descs.items():
         if column_desc.column_type == ColumnType.DECIMAL:
             out[column_name] = SparkFloatColumnDescriptor(
                 allow_nan=column_desc.allow_nan,
                 allow_inf=column_desc.allow_inf,
                 allow_null=column_desc.allow_null,
             )
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/binning_spec.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/binning_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A BinningSpec defines a binning operation on a column."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 import bisect
 import datetime
 import math
 from typing import Any, Generic, List, Optional, Sequence, TypeVar, cast
 
 from tmlt.analytics._schema import ColumnDescriptor, ColumnType, column_type_to_py_type
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/keyset.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/keyset.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 and the values ``[0, 1, 2, 3]`` for column B.
 
 Currently, KeySets are used as a simpler way to specify domains for groupby
 transformations.
 """
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 from __future__ import annotations
 
 import datetime
 from typing import Callable, Dict, Iterable, List, Mapping, Optional, Tuple, Type, Union
 
 from pyspark.sql import Column, DataFrame
@@ -41,15 +41,15 @@
                 f"{','.join(str(t) for t in allowed_types)}"
             )
 
 
 def _check_dict_schema(types: Dict[str, type]) -> None:
     """Raise an exception if the dict contains a type not allowed in a KeySet."""
     allowed_types = {int, str, datetime.date}
-    for (col, dtype) in types.items():
+    for col, dtype in types.items():
         if dtype not in allowed_types:
             raise ValueError(
                 f"Column {col} has type {dtype.__qualname__}, which is "
                 "not allowed in KeySets. Allowed column types are: "
                 f"{','.join(t.__qualname__ for t in allowed_types)}"
             )
 
@@ -154,22 +154,22 @@
         caller to ensure that the given dataframe remains valid for the lifetime
         of the KeySet. If the dataframe becomes invalid, for example because its
         Spark session is closed, this method or any uses of the resulting
         dataframe may raise exceptions or have other unanticipated effects.
         """
         return KeySet(coerce_spark_schema_or_fail(dataframe).dropDuplicates())
 
-    def filter(self, expr: Union[Column, str]) -> KeySet:
-        """Filter this KeySet using some expression.
+    def filter(self, condition: Union[Column, str]) -> KeySet:
+        """Filter this KeySet using some condition.
 
         This method accepts the same syntax as
-        :meth:`~pyspark.sql.DataFrame.filter`: valid expressions are those that
+        :meth:`~pyspark.sql.DataFrame.filter`: valid conditions are those that
         can be used in a `WHERE clause
         <https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-where.html>`__
-        in Spark SQL. Examples of valid predicates include:
+        in Spark SQL. Examples of valid conditions include:
 
         * ``age < 42``
         * ``age BETWEEN 17 AND 42``
         * ``age < 42 OR (age < 60 AND gender IS NULL)``
         * ``LENGTH(name) > 17``
         * ``favorite_color IN ('blue', 'red')``
 
@@ -190,15 +190,15 @@
             >>> filtered_keyset.dataframe().sort("A", "B").toPandas()
                 A  B
             0  a2  0
             1  a2  1
             2  a2  2
             3  a2  3
         """
-        return KeySet(self.dataframe().filter(expr))
+        return KeySet(self.dataframe().filter(condition))
 
     def __getitem__(self, columns: Union[str, Tuple[str, ...], List[str]]) -> KeySet:
         """``KeySet[col, col, ...]`` returns a KeySet with those columns only.
 
         The returned KeySet contains all unique combinations of values in the
         given columns that were present in the original KeySet.
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/privacy_budget.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/privacy_budget.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Classes for specifying privacy budgets.
 
 For a full introduction to privacy budgets, see the
 :ref:`privacy budget topic guide<Privacy budget fundamentals>`.
 """
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 import math
 from abc import ABC
 from typing import Union
 
 from typeguard import typechecked
 
 from tmlt.core.utils.exact_number import ExactNumber
@@ -33,15 +33,15 @@
 
 
 class PureDPBudget(PrivacyBudget):
     """A privacy budget under pure differential privacy.
 
     This privacy definition is also known as epsilon-differential privacy, and the
     associated value is the epsilon privacy parameter. The privacy definition can
-    be found `here <https://en.wikipedia.org/wiki/Differential_privacy#Definition_of_%CE%B5-differential_privacy>`_
+    be found `here <https://en.wikipedia.org/wiki/Differential_privacy#Definition_of_%CE%B5-differential_privacy>`__.
     """  # pylint: disable=line-too-long
 
     @typechecked
     def __init__(self, epsilon: Union[int, float]):
         """Construct a new PureDPBudget.
 
         Args:
@@ -72,14 +72,86 @@
         if isinstance(other, PureDPBudget):
             return ExactNumber.from_float(
                 self.epsilon, False
             ) == ExactNumber.from_float(other.epsilon, False)
         return False
 
 
+class ApproxDPBudget(PrivacyBudget):
+    """A privacy budget under approximate differential privacy.
+
+    This privacy definition is also known as (ε, δ)-differential privacy, and the
+    associated privacy parameters are epsilon and delta. The formal definition can
+    be found `here <https://desfontain.es/privacy/almost-differential-privacy.html#formal-definition>`__.
+    """  # pylint: disable=line-too-long
+
+    @typechecked
+    def __init__(self, epsilon: Union[int, float], delta: float):
+        """Construct a new ApproxDPBudget.
+
+        Args:
+            epsilon: The epsilon privacy parameter. Must be non-negative.
+                To specify an infinite budget, set epsilon equal to float('inf').
+            delta: The delta privacy parameter. Must be between 0 and 1 (inclusive).
+                If delta is 0, this is equivalent to PureDP.
+        """
+        if math.isnan(epsilon):
+            raise ValueError("Epsilon cannot be a NaN.")
+        if math.isnan(delta):
+            raise ValueError("Delta cannot be a NaN.")
+        if epsilon < 0:
+            raise ValueError(
+                "Epsilon must be non-negative. "
+                f"Cannot construct an ApproxDPBudget with epsilon of {epsilon}."
+            )
+        if delta < 0 or delta > 1:
+            raise ValueError(
+                "Delta must be between 0 and 1 (inclusive). "
+                f"Cannot construct an ApproxDPBudget with delta of {delta}."
+            )
+        self._epsilon = epsilon
+        self._delta = delta
+
+    @property
+    def epsilon(self) -> Union[int, float]:
+        """Returns the value of epsilon."""
+        return self._epsilon
+
+    @property
+    def delta(self) -> float:
+        """Returns the value of delta."""
+        return self._delta
+
+    @property
+    def is_infinite(self) -> bool:
+        """Returns true if epsilon is float('inf') or delta is 1."""
+        return self.epsilon == float("inf") or self.delta == 1
+
+    def __repr__(self) -> str:
+        """Returns the string representation of this ApproxDPBudget."""
+        return f"ApproxDPBudget(epsilon={self.epsilon}, delta={self.delta})"
+
+    def __eq__(self, other) -> bool:
+        """Returns whether two ApproxDPBudgets are equivalent.
+
+        ApproxDPBudgets that provide no privacy guarantee are considered equal (for example, if one has an
+        epsilon of float('inf') and the other has a delta of 1).
+        """
+        if isinstance(other, ApproxDPBudget):
+            are_both_infinite = self.is_infinite and other.is_infinite
+            is_same_epsilon = ExactNumber.from_float(
+                self.epsilon, False
+            ) == ExactNumber.from_float(other.epsilon, False)
+            is_same_delta = ExactNumber.from_float(
+                self.delta, False
+            ) == ExactNumber.from_float(other.delta, False)
+            return are_both_infinite or (is_same_epsilon and is_same_delta)
+        return False
+
+
 class RhoZCDPBudget(PrivacyBudget):
     """A privacy budget under rho-zero-concentrated differential privacy.
 
     The definition of rho-zCDP can be found in
     `this <https://arxiv.org/pdf/1605.02065.pdf>`_ paper under Definition 1.1.
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/protected_change.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/protected_change.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Types for programmatically specifying what changes in input tables are protected."""
 
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # SPDX-License-Identifier: Apache-2.0
 from abc import ABC
 from dataclasses import dataclass
 from typing import Union
 
 from typeguard import check_type
 
@@ -69,14 +69,22 @@
     the dataset, that must be enforced *before* the data is passed to Tumult
     Analytics.
 
     :class:`AddMaxRowsInMaxGroups` is intended for advanced use cases, and its
     use should be considered carefully. Note that it only provides improved
     accuracy when used with zCDP -- with pure DP, it is equivalent to using
     :class:`AddMaxRows` with the same total number of rows to be added/removed.
+
+    The most common case where :class:`AddMaxRowsInMaxGroups` is useful is for
+    dealing with datasets that have already undergone some type of preprocessing
+    before being turned over to an analyst. Where possible, it is preferred to
+    do such processing inside of Tumult Analytics instead, as it allows
+    specifying a simpler protected change (e.g. :class:`AddRowsWithID`)
+    and relying on Analytics' privacy tracking to handle the complex parts
+    of the analysis.
     """
 
     grouping_column: str
     """The name of the column specifying the group."""
     max_groups: int
     """The maximum number of groups that may differ."""
     max_rows_per_group: Union[int, float]
@@ -87,7 +95,37 @@
         check_type("column", self.grouping_column, str)
         check_type("max_groups", self.max_groups, int)
         check_type("max_rows_per_group", self.max_rows_per_group, Union[int, float])
         if self.max_groups < 1:
             raise ValueError("max_groups must be positive")
         if self.max_rows_per_group < 1:
             raise ValueError("max_rows_per_group must be positive")
+
+
+@dataclass(frozen=True)
+class AddRowsWithID(ProtectedChange):
+    """Protect the addition or removal of rows with a specific identifier.
+
+    Instead of limiting the number of rows that may be added or removed,
+    :class:`AddRowsWithID` hides the addition or removal of *all rows*
+    with the same value in the specified column.
+
+    The id column *must* be a string, integer (or long), or date; it cannot
+    be a float or a timestamp.
+    """
+
+    id_column: str
+    """The name of the column containing the identifier."""
+
+    id_space: str = "default_id_space"
+    """The identifier space of the rows that may be added or removed. If not specified,
+    a default will be assigned when using this protected change with
+    :class:`tmlt.analytics.session.Session.from_dataframe`."""
+
+    def __post_init__(self):
+        """Validate attributes."""
+        check_type("id_space", self.id_space, str)
+        if self.id_space == "":
+            raise ValueError("identifier must be non-empty")
+        check_type("id_column", self.id_column, str)
+        if self.id_column == "":
+            raise ValueError("id_column must be non-empty")
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/query_builder.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/query_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,31 +22,33 @@
 :meth:`~tmlt.analytics.query_builder.QueryBuilder.groupby`, yielding a
 :class:`~tmlt.analytics.query_expr.QueryExpr` object. This QueryExpr can then be
 passed to :func:`~tmlt.analytics.session.Session.evaluate` to obtain
 differentially private results to the query.
 """
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 import datetime
 import warnings
 from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 from pyspark.sql import DataFrame
 
 from tmlt.analytics._schema import ColumnDescriptor, ColumnType, Schema
 from tmlt.analytics.binning_spec import BinningSpec, BinT
+from tmlt.analytics.constraints import Constraint
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.query_expr import (
     AverageMechanism,
     CountDistinctMechanism,
     CountMechanism,
     DropInfinity,
     DropNullAndNan,
+    EnforceConstraint,
     Filter,
     FlatMap,
     GroupByBoundedAverage,
     GroupByBoundedSTDEV,
     GroupByBoundedSum,
     GroupByBoundedVariance,
     GroupByCount,
@@ -264,28 +266,41 @@
             public_table=public_table,
             join_columns=list(join_columns) if join_columns is not None else None,
         )
         return self
 
     def join_private(
         self,
-        right_operand: "QueryBuilder",
-        truncation_strategy_left: TruncationStrategy.Type,
-        truncation_strategy_right: TruncationStrategy.Type,
+        right_operand: Union["QueryBuilder", str],
+        truncation_strategy_left: Optional[TruncationStrategy.Type] = None,
+        truncation_strategy_right: Optional[TruncationStrategy.Type] = None,
         join_columns: Optional[Sequence[str]] = None,
     ) -> "QueryBuilder":
         # pylint: disable=protected-access
         """Updates the current query to join with another :class:`QueryBuilder`.
 
-        This operation is a natural join, with the same behavior and
-        requirements as :func:`join_public`. However, there is a key difference:
-        before the join is performed, each table is *truncated* based on the
-        corresponding
+        The current query can also join with a named private table (represented
+        as a string).
+
+        This operation is a natural join, with the same behavior and requirements as
+        :func:`join_public`.
+
+        For operations on tables with a
+        :class:`tmlt.analytics.protected_change.ProtectedChange` that protects adding or
+        removing rows (e.g., :class:`~tmlt.analytics.protected_change.AddMaxRows`),
+        there is a key difference: before the join is performed, each table is
+        *truncated* based on the corresponding
         :class:`~tmlt.analytics.truncation_strategy.TruncationStrategy`.
 
+        In contrast, operations on tables with a
+        :class:`tmlt.analytics.protected_change.AddRowsWithID`
+        :class:`tmlt.analytics.protected_change.ProtectedChange` do not require a
+        :class:`~tmlt.analytics.truncation_strategy.TruncationStrategy`, as no
+        truncation is necessary while performing the join.
+
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
             >>> spark = SparkSession.builder.getOrCreate()
@@ -361,19 +376,23 @@
             0      1
 
         Args:
             right_operand: QueryBuilder object representing the table to be joined with.
                             When calling ``query_a.join_private(query_b, ...)``, we
                             refer to ``query_a`` as the *left table* and ``query_b`` as
                             the *right table*.
+                            ``query_a.join_private("table")`` is shorthand for
+                            ``query_a.join_private(QueryBuilder("table"))``.
             truncation_strategy_left: Strategy for truncation of the left table.
             truncation_strategy_right: Strategy for truncation of the right table.
             join_columns: The columns to join on. If ``join_columns`` is not specified,
                           the tables will be joined on all common columns.
         """
+        if isinstance(right_operand, str):
+            right_operand = QueryBuilder(right_operand)
         self._query_expr = JoinPrivate(
             self._query_expr,
             right_operand._query_expr,
             truncation_strategy_left,
             truncation_strategy_right,
             list(join_columns) if join_columns is not None else None,
         )
@@ -498,15 +517,15 @@
             0  a1  0.0  0.0
             1  a1  NaN -inf
             2  a2  2.0  inf
             >>> sess.private_sources
             ['my_private_data']
             >>> sess.get_schema("my_private_data").column_types
             {'A': 'VARCHAR', 'B': 'DECIMAL', 'X': 'DECIMAL'}
-            >>> # Building a query with a replace_null_and_nan transformation
+            >>> # Building a query with a replace_infinity transformation
             >>> query = (
             ...     QueryBuilder("my_private_data")
             ...     .replace_infinity(
             ...         replace_with={
             ...             "X": (-100, 100),
             ...         },
             ...     )
@@ -776,22 +795,22 @@
         Args:
             column_mapper: A mapping of columns to new column names.
                 Columns not specified in the mapper will remain the same.
         """
         self._query_expr = Rename(child=self._query_expr, column_mapper=column_mapper)
         return self
 
-    def filter(self, predicate: str) -> "QueryBuilder":
-        """Updates the current query to filter for rows matching a predicate.
+    def filter(self, condition: str) -> "QueryBuilder":
+        """Updates the current query to filter for rows matching a condition.
 
-        The ``predicate`` parameter accepts the same syntax as in PySpark's
+        The ``condition`` parameter accepts the same syntax as in PySpark's
         :meth:`~pyspark.sql.DataFrame.filter` method: valid expressions are
         those that can be used in a `WHERE clause
         <https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-where.html>`__
-        in Spark SQL. Examples of valid predicates include:
+        in Spark SQL. Examples of valid conditions include:
 
         * ``age < 42``
         * ``age BETWEEN 17 AND 42``
         * ``age < 42 OR (age < 60 AND gender IS NULL)``
         * ``LENGTH(name) > 17``
         * ``favorite_color IN ('blue', 'red')``
         * ``date = '2022-03-14'``
@@ -838,19 +857,19 @@
             ...     PureDPBudget(float("inf"))
             ... )
             >>> answer.toPandas()
                count
             0      1
 
         Args:
-            predicate: A string of SQL expressions specifying the filter to apply to the
+            condition: A string of SQL expressions specifying the filter to apply to the
                 data. For example, the string "A > B" matches rows where column A is
                 greater than column B.
         """
-        self._query_expr = Filter(child=self._query_expr, predicate=predicate)
+        self._query_expr = Filter(child=self._query_expr, condition=condition)
         return self
 
     def select(self, columns: Sequence[str]) -> "QueryBuilder":
         """Updates the current query to select certain columns.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
@@ -998,25 +1017,31 @@
             augment=augment,
         )
         return self
 
     def flat_map(
         self,
         f: Callable[[Row], List[Row]],
-        max_num_rows: int,
         new_column_types: Mapping[str, Union[str, ColumnDescriptor, ColumnType]],
         augment: bool = False,
         grouping: bool = False,
+        max_num_rows: Optional[int] = None,
     ) -> "QueryBuilder":
         """Updates the current query to apply a flat map.
 
         If you provide only a ColumnType for the new column types, Analytics
         assumes that all new columns created may contain null values (and that
         DECIMAL columns may contain NaN or infinite values).
 
+        Operations on tables with a
+        :class:`tmlt.analytics.protected_change.AddRowsWithID`
+        :class:`tmlt.analytics.protected_change.ProtectedChange` do not require a
+        ``max_num_rows`` argument, since it is not necessary to impose a limit on
+        the number of new rows.
+
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
             >>> from tmlt.analytics.keyset import KeySet
             >>> import pandas as pd
             >>> from pyspark.sql import SparkSession
@@ -1047,21 +1072,21 @@
             >>> sess.get_schema("my_private_data").column_types
             {'A': 'VARCHAR', 'B': 'INTEGER', 'X': 'INTEGER'}
             >>> # Building a query with a flat map transformation
             >>> query = (
             ...     QueryBuilder("my_private_data")
             ...     .flat_map(
             ...         lambda row: [{"i_B": i} for i in range(int(row["B"])+1)],
-            ...         max_num_rows=3,
             ...         new_column_types={"i_B": ColumnDescriptor(
             ...             ColumnType.INTEGER,
             ...             allow_null=False,
             ...         )},
             ...         augment=True,
-            ...         grouping=False
+            ...         grouping=False,
+            ...         max_num_rows=3,
             ...     )
             ...     .groupby(KeySet.from_dict({"B": [0, 1, 2, 3]}))
             ...     .count()
             ... )
             >>> # Answering the query with infinite privacy budget
             >>> answer = sess.evaluate(
             ...     query,
@@ -1080,29 +1105,29 @@
                 its value for that row.
                 This function should return a list of dictionaries.
                 Those dictionaries should always
                 have the same keys regardless of input, and the values in those
                 dictionaries should match the column type specified in
                 ``new_column_types``. The function should not have any side effects
                 (in particular, f cannot raise exceptions).
-            max_num_rows: The enforced limit on the number of rows from each f(row).
-                If f produces more rows than this, only the first ``max_num_rows``
-                rows will be in the output.
             new_column_types: Mapping from column names to types, for new columns
                 produced by f. Using
                 :class:`tmlt.analytics.query_builder.ColumnDescriptor`
                 is preferred.
             augment: If True, add new columns to the existing dataframe (so new
                      schema = old schema + schema_new_columns).
                      If False, make the new dataframe with schema = schema_new_columns
             grouping: Whether this produces a new column that we want to groupby.
                 If True, this requires that any groupby aggregations following this
                 query include the new column as a groupby column. Only one new column
                 is supported, and the new column must have distinct values for each
                 input row.
+            max_num_rows: The enforced limit on the number of rows from each f(row).
+                If f produces more rows than this, only the first ``max_num_rows``
+                rows will be in the output.
         """
         grouping_column: Optional[str]
         if grouping:
             if len(new_column_types) != 1:
                 raise ValueError(
                     "new_column_types contains "
                     f"{len(new_column_types)} "
@@ -1110,23 +1135,23 @@
                 )
             (grouping_column,) = new_column_types
         else:
             grouping_column = None
         self._query_expr = FlatMap(
             child=self._query_expr,
             f=f,
-            max_num_rows=max_num_rows,
             schema_new_columns=Schema(
                 dict(new_column_types),
                 grouping_column=grouping_column,
                 default_allow_null=True,
                 default_allow_nan=True,
                 default_allow_inf=True,
             ),
             augment=augment,
+            max_num_rows=max_num_rows,
         )
         return self
 
     def bin_column(
         self, column: str, spec: BinningSpec, name: Optional[str] = None
     ) -> "QueryBuilder":
         """Create a new column by assigning the values in a given column to bins.
@@ -1291,14 +1316,24 @@
             spec = bin_edges
         if not name:
             name = column + "_binned"
 
         keys = KeySet.from_dict({name: spec.bins()})
         return self.bin_column(column, spec, name).groupby(keys).count()
 
+    def enforce(self, constraint: Constraint) -> "QueryBuilder":
+        """Enforce a :mod:`~tmlt.analytics.constraints.Constraint` on the current table.
+
+        This method can be used to enforce constraints on the current table. See
+        the :mod:`~tmlt.analytics.constraints` module for information about the
+        available constraints and what they are used for.
+        """
+        self._query_expr = EnforceConstraint(self._query_expr, constraint, options={})
+        return self
+
     def groupby(self, keys: KeySet) -> "GroupedQueryBuilder":
         """Groups the query by the given set of keys, returning a GroupedQueryBuilder.
 
         ..
             >>> from tmlt.analytics.privacy_budget import PureDPBudget
             >>> import tmlt.analytics.session
             >>> from tmlt.analytics.protected_change import AddOneRow
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/query_expr.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/query_expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 :class:`tmlt.analytics.query_builder.QueryBuilder` to create them and
 :class:`tmlt.analytics.session.Session` to consume them provide more
 user-friendly features.
 """
 # TODO: Known typeguard issue: https://github.com/agronholm/typeguard/issues/65
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 import datetime
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from enum import Enum, auto
 from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple, Union
 
 from pyspark.sql import DataFrame
 from typeguard import check_type
 
 from tmlt.analytics._coerce_spark_schema import coerce_spark_schema_or_fail
 from tmlt.analytics._schema import Schema
+from tmlt.analytics.constraints import Constraint
 from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.truncation_strategy import TruncationStrategy
 
 Row = Dict[str, Any]
 """Type alias for dictionary with string keys."""
 
 
@@ -224,29 +225,29 @@
     def accept(self, visitor: "QueryExprVisitor") -> Any:
         """Visit this QueryExpr with visitor."""
         return visitor.visit_rename(self)
 
 
 @dataclass
 class Filter(QueryExpr):
-    """Returns the subset of the rows that satisfy the predicate."""
+    """Returns the subset of the rows that satisfy the condition."""
 
     child: QueryExpr
     """The QueryExpr to filter."""
-    predicate: str
+    condition: str
     """A string of SQL expression specifying the filter to apply to the data.
 
     For example, the string "A > B" matches rows where column A is greater than
     column B.
     """
 
     def __post_init__(self):
         """Checks arguments to constructor."""
         check_type("child", self.child, QueryExpr)
-        check_type("predicate", self.predicate, str)
+        check_type("condition", self.condition, str)
 
     def accept(self, visitor: "QueryExprVisitor") -> Any:
         """Visit this QueryExpr with visitor."""
         return visitor.visit_filter(self)
 
 
 @dataclass
@@ -304,22 +305,16 @@
         """Returns true iff self == other.
 
         This uses the bytecode of self.f and other.f to determine if the two
         functions are equal.
         """
         if not isinstance(other, Map):
             return False
-        # This line will incorrectly produce a typing error;
-        # see https://github.com/python/mypy/issues/5485
-        # Also, mypy will only ignore lines if you have a # type: ignore comment
-        # on the end of the line, which makes this line too long.
-        # pylint: disable=line-too-long
-        if self.f != other.f and self.f.__code__.co_code != other.f.__code__.co_code:  # type: ignore
+        if self.f != other.f and self.f.__code__.co_code != other.f.__code__.co_code:
             return False
-        # pylint: enable=line-too-long
         return (
             self.schema_new_columns == other.schema_new_columns
             and self.augment == other.augment
             and self.child == other.child
         )
 
 
@@ -327,38 +322,38 @@
 class FlatMap(QueryExpr):
     """Applies a flat map function to each row of a relation."""
 
     child: QueryExpr
     """The QueryExpr to apply the flat map on."""
     f: Callable[[Row], List[Row]]
     """The flat map function."""
-    max_num_rows: int
-    """The enforced limit on number of rows from each f(row)."""
     schema_new_columns: Schema
     """The expected schema for new columns produced by ``f``.
 
     If the ``schema_new_columns`` has a ``grouping_column``, that means this FlatMap
     produces a column that must be grouped by eventually. It also must be the only
     column in the schema.
     """
     augment: bool
     """Whether to keep the existing columns.
 
     If True, schema = old schema + schema_new_columns, otherwise only keeps the new
-    columns (schema = schema_new_columns).
-    """
+    columns (schema = schema_new_columns)."""
+
+    max_num_rows: Optional[int] = None
+    """The enforced limit on number of rows from each f(row)."""
 
     def __post_init__(self):
         """Checks arguments to constructor."""
         check_type("child", self.child, QueryExpr)
         check_type("f", self.f, Callable[[Row], List[Row]])
-        check_type("max_num_rows", self.max_num_rows, int)
+        check_type("max_num_rows", self.max_num_rows, Optional[int])
         check_type("schema_new_columns", self.schema_new_columns, Schema)
         check_type("augment", self.augment, bool)
-        if self.max_num_rows < 0:
+        if self.max_num_rows and self.max_num_rows < 0:
             raise ValueError(
                 f"Limit on number of rows '{self.max_num_rows}' must be nonnegative."
             )
         if (
             self.schema_new_columns.grouping_column
             and len(self.schema_new_columns) != 1
         ):
@@ -376,22 +371,16 @@
         """Returns true iff self == other.
 
         This uses the bytecode of self.f and other.f to determine if the two
         functions are equal.
         """
         if not isinstance(other, FlatMap):
             return False
-        # This line will incorrectly produce a typing error;
-        # see https://github.com/python/mypy/issues/5485
-        # Also, mypy will only ignore lines if you have a # type: ignore comment
-        # on the end of the line, which makes this line too long.
-        # pylint: disable=line-too-long
-        if self.f != other.f and self.f.__code__.co_code != other.f.__code__.co_code:  # type: ignore
+        if self.f != other.f and self.f.__code__.co_code != other.f.__code__.co_code:
             return False
-        # pylint: enable=line-too-long
         return (
             self.max_num_rows == other.max_num_rows
             and self.schema_new_columns == other.schema_new_columns
             and self.augment == other.augment
             and self.child == other.child
         )
 
@@ -406,34 +395,34 @@
     :meth:`~tmlt.analytics.query_builder.QueryBuilder.join_private`.
     """
 
     child: QueryExpr
     """The QueryExpr to join with right operand."""
     right_operand_expr: QueryExpr
     """The QueryExpr for private source to join with."""
-    truncation_strategy_left: TruncationStrategy.Type
+    truncation_strategy_left: Optional[TruncationStrategy.Type] = None
     """Truncation strategy to be used for the left table."""
-    truncation_strategy_right: TruncationStrategy.Type
+    truncation_strategy_right: Optional[TruncationStrategy.Type] = None
     """Truncation strategy to be used for the right table."""
     join_columns: Optional[List[str]] = None
     """The columns used for joining the tables, or None to use all common columns."""
 
     def __post_init__(self):
         """Checks arguments to constructor."""
         check_type("child", self.child, QueryExpr)
         check_type("right_operand_expr", self.right_operand_expr, QueryExpr)
         check_type(
             "truncation_strategy_left",
             self.truncation_strategy_left,
-            TruncationStrategy.Type,
+            Optional[TruncationStrategy.Type],
         )
         check_type(
             "truncation_strategy_right",
             self.truncation_strategy_right,
-            TruncationStrategy.Type,
+            Optional[TruncationStrategy.Type],
         )
         check_type("join_columns", self.join_columns, Optional[List[str]])
 
         if self.join_columns is not None:
             if len(self.join_columns) == 0:
                 raise ValueError("Provided join columns must not be empty")
             if len(self.join_columns) != len(set(self.join_columns)):
@@ -657,14 +646,33 @@
         check_type("columns", self.columns, List[str])
 
     def accept(self, visitor: "QueryExprVisitor") -> Any:
         """Visit this QueryExpr with visitor."""
         return visitor.visit_drop_infinity(self)
 
 
+@dataclass(frozen=True)
+class EnforceConstraint(QueryExpr):
+    """Enforces a constraint on the data."""
+
+    child: QueryExpr
+    """The QueryExpr to which the constraint will be applied."""
+    constraint: Constraint
+    """A constraint to be enforced."""
+    options: Dict[str, Any] = field(default_factory=dict)
+    """Options to be used when enforcing the constraint.
+
+    Appropriate values here vary depending on the constraint. These options are
+    to support advanced use cases, and generally should not be used."""
+
+    def accept(self, visitor: "QueryExprVisitor") -> Any:
+        """Visit this QueryExpr with visitor."""
+        return visitor.visit_enforce_constraint(self)
+
+
 @dataclass
 class GroupByCount(QueryExpr):
     """Returns the count of each combination of the groupby domains."""
 
     child: QueryExpr
     """The QueryExpr to measure."""
     groupby_keys: KeySet
@@ -739,17 +747,21 @@
     groupby_keys: KeySet
     """The keys of the resulting aggregated data."""
     measure_column: str
     """The column to compute the quantile over."""
     quantile: float
     """The quantile to compute (between 0 and 1)."""
     low: float
-    """The lower bound for clamping the ``measure_column``."""
+    """The lower bound for clamping the ``measure_column``.
+    Should be less than ``high``.
+    """
     high: float
-    """The upper bound for clamping the ``measure_column``."""
+    """The upper bound for clamping the ``measure_column``.
+    Should be greater than ``low``.
+    """
     output_column: str = "quantile"
     """The name of the column to store the quantiles in."""
 
     def __post_init__(self):
         """Checks arguments to constructor."""
         check_type("child", self.child, QueryExpr)
         check_type("groupby_keys", self.groupby_keys, KeySet)
@@ -763,17 +775,17 @@
             raise ValueError(
                 f"Quantile must be between 0 and 1, and not '{self.quantile}'."
             )
         if type(self.low) != type(self.high):  # pylint: disable=unidiomatic-typecheck
             # If one is int and other is float; silently cast to float
             self.low = float(self.low)
             self.high = float(self.high)
-        if self.low > self.high:
+        if self.low >= self.high:
             raise ValueError(
-                f"Lower bound '{self.low}' can not be greater than "
+                f"Lower bound '{self.low}' must be less than "
                 f"the upper bound '{self.high}'."
             )
 
     def accept(self, visitor: "QueryExprVisitor") -> Any:
         """Visit this QueryExpr with visitor."""
         return visitor.visit_groupby_quantile(self)
 
@@ -791,17 +803,21 @@
     child: QueryExpr
     """The QueryExpr to measure."""
     groupby_keys: KeySet
     """The keys of the resulting aggregated data."""
     measure_column: str
     """The column to compute the sum over."""
     low: float
-    """The lower bound for clamping the ``measure_column``."""
+    """The lower bound for clamping the ``measure_column``.
+    Should be less than ``high``.
+    """
     high: float
-    """The upper bound for clamping the ``measure_column``."""
+    """The upper bound for clamping the ``measure_column``.
+    Should be greater than ``low``.
+    """
     output_column: str = "sum"
     """The name of the column to store the sums in."""
     mechanism: SumMechanism = SumMechanism.DEFAULT
     """Choice of noise mechanism.
 
     By DEFAULT, the framework automatically selects an
     appropriate mechanism.
@@ -817,17 +833,17 @@
         check_type("output_column", self.output_column, str)
         check_type("mechanism", self.mechanism, SumMechanism)
 
         if type(self.low) != type(self.high):  # pylint: disable=unidiomatic-typecheck
             # If one is int and other is float; silently cast to float
             self.low = float(self.low)
             self.high = float(self.high)
-        if self.low > self.high:
+        if self.low >= self.high:
             raise ValueError(
-                f"Lower bound '{self.low}' can not be greater than "
+                f"Lower bound '{self.low}' must be less than "
                 f"the upper bound '{self.high}'."
             )
 
     def accept(self, visitor: "QueryExprVisitor") -> Any:
         """Visit this QueryExpr with visitor."""
         return visitor.visit_groupby_bounded_sum(self)
 
@@ -845,17 +861,21 @@
     child: QueryExpr
     """The QueryExpr to measure."""
     groupby_keys: KeySet
     """The keys of the resulting aggregated data."""
     measure_column: str
     """The column to compute the average over."""
     low: float
-    """The lower bound for clamping the ``measure_column``."""
+    """The lower bound for clamping the ``measure_column``.
+    Should be less than ``high``.
+    """
     high: float
-    """The upper bound for clamping the ``measure_column``."""
+    """The upper bound for clamping the ``measure_column``.
+    Should be greater than ``low``.
+    """
     output_column: str = "average"
     """The name of the column to store the averages in."""
     mechanism: AverageMechanism = AverageMechanism.DEFAULT
     """Choice of noise mechanism.
 
     By DEFAULT, the framework automatically selects an
     appropriate mechanism.
@@ -871,17 +891,17 @@
         check_type("output_column", self.output_column, str)
         check_type("mechanism", self.mechanism, AverageMechanism)
 
         if type(self.low) != type(self.high):  # pylint: disable=unidiomatic-typecheck
             # If one is int and other is float; silently cast to float
             self.low = float(self.low)
             self.high = float(self.high)
-        if self.low > self.high:
+        if self.low >= self.high:
             raise ValueError(
-                f"Lower bound '{self.low}' can not be greater than "
+                f"Lower bound '{self.low}' must be less than "
                 f"the upper bound '{self.high}'."
             )
 
     def accept(self, visitor: "QueryExprVisitor") -> Any:
         """Visit this QueryExpr with visitor."""
         return visitor.visit_groupby_bounded_average(self)
 
@@ -899,17 +919,21 @@
     child: QueryExpr
     """The QueryExpr to measure."""
     groupby_keys: KeySet
     """The keys of the resulting aggregated data."""
     measure_column: str
     """The column to compute the variance over."""
     low: float
-    """The lower bound for clamping the ``measure_column``."""
+    """The lower bound for clamping the ``measure_column``.
+    Should be less than ``high``.
+    """
     high: float
-    """The upper bound for clamping the ``measure_column``."""
+    """The upper bound for clamping the ``measure_column``.
+    Should be greater than ``low``.
+    """
     output_column: str = "variance"
     """The name of the column to store the variances in."""
     mechanism: VarianceMechanism = VarianceMechanism.DEFAULT
     """Choice of noise mechanism.
 
     By DEFAULT, the framework automatically selects an
     appropriate mechanism.
@@ -925,17 +949,17 @@
         check_type("output_column", self.output_column, str)
         check_type("mechanism", self.mechanism, VarianceMechanism)
 
         if type(self.low) != type(self.high):  # pylint: disable=unidiomatic-typecheck
             # If one is int and other is float; silently cast to float
             self.low = float(self.low)
             self.high = float(self.high)
-        if self.low > self.high:
+        if self.low >= self.high:
             raise ValueError(
-                f"Lower bound '{self.low}' can not be greater than "
+                f"Lower bound '{self.low}' must be less than "
                 f"the upper bound '{self.high}'."
             )
 
     def accept(self, visitor: "QueryExprVisitor") -> Any:
         """Visit this QueryExpr with visitor."""
         return visitor.visit_groupby_bounded_variance(self)
 
@@ -953,17 +977,21 @@
     child: QueryExpr
     """The QueryExpr to measure."""
     groupby_keys: KeySet
     """The keys of the resulting aggregated data."""
     measure_column: str
     """The column to compute the standard deviation over."""
     low: float
-    """The lower bound for clamping the ``measure_column``."""
+    """The lower bound for clamping the ``measure_column``.
+    Should be less than ``high``.
+    """
     high: float
-    """The upper bound for clamping the ``measure_column``."""
+    """The upper bound for clamping the ``measure_column``.
+    Should be greater than ``low``.
+    """
     output_column: str = "stdev"
     """The name of the column to store the stdev in."""
     mechanism: StdevMechanism = StdevMechanism.DEFAULT
     """Choice of noise mechanism.
 
     By DEFAULT, the framework automatically selects an
     appropriate mechanism.
@@ -980,17 +1008,17 @@
         check_type("mechanism", self.mechanism, StdevMechanism)
 
         if type(self.low) != type(self.high):  # pylint: disable=unidiomatic-typecheck
             # If one is int and other is float; silently cast to float
             self.low = float(self.low)
             self.high = float(self.high)
 
-        if self.low > self.high:
+        if self.low >= self.high:
             raise ValueError(
-                f"Lower bound '{self.low}' can not be greater than "
+                f"Lower bound '{self.low}' must be less than "
                 f"the upper bound '{self.high}'."
             )
 
     def accept(self, visitor: "QueryExprVisitor") -> Any:
         """Visit this QueryExpr with visitor."""
         return visitor.visit_groupby_bounded_stdev(self)
 
@@ -1055,14 +1083,19 @@
 
     @abstractmethod
     def visit_drop_infinity(self, expr: DropInfinity) -> Any:
         """Visit a :class:`DropInfinity`."""
         raise NotImplementedError
 
     @abstractmethod
+    def visit_enforce_constraint(self, expr: EnforceConstraint) -> Any:
+        """Visit a :class:`EnforceConstraint`."""
+        raise NotImplementedError
+
+    @abstractmethod
     def visit_groupby_count(self, expr: GroupByCount) -> Any:
         """Visit a :class:`GroupByCount`."""
         raise NotImplementedError
 
     @abstractmethod
     def visit_groupby_count_distinct(self, expr: GroupByCountDistinct) -> Any:
         """Visit a :class:`GroupByCountDistinct`."""
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/session.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/session.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,84 +15,110 @@
 each of the private tables, provided that the private data is not used elsewhere
 in the computation of the queries.
 
 More details on the exact privacy promise provided by :class:`Session` can be
 found in the :ref:`Privacy promise topic guide <Privacy promise>`.
 """
 
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 # SPDX-License-Identifier: Apache-2.0
 from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Union, cast
 from warnings import warn
 
 import pandas as pd  # pylint: disable=unused-import
 import sympy as sp
 from pyspark.sql import SparkSession  # pylint: disable=unused-import
 from pyspark.sql import DataFrame
 from typeguard import check_type, typechecked
 
-from tmlt.analytics._catalog import Catalog
+from tmlt.analytics._catalog import Catalog, PrivateTable, PublicTable
 from tmlt.analytics._coerce_spark_schema import (
     SUPPORTED_SPARK_TYPES,
     TYPE_COERCION_MAP,
     coerce_spark_schema_or_fail,
 )
-from tmlt.analytics._neighboring_relation_visitor import NeighboringRelationCoreVisitor
-from tmlt.analytics._neighboring_relations import (
+from tmlt.analytics._neighboring_relation import (
+    AddRemoveKeys,
     AddRemoveRows,
     AddRemoveRowsAcrossGroups,
     Conjunction,
     NeighboringRelation,
 )
+from tmlt.analytics._neighboring_relation_visitor import NeighboringRelationCoreVisitor
 from tmlt.analytics._noise_info import _noise_from_measurement
 from tmlt.analytics._privacy_budget_rounding_helper import get_adjusted_budget
 from tmlt.analytics._query_expr_compiler import QueryExprCompiler
 from tmlt.analytics._schema import (
     Schema,
     spark_dataframe_domain_to_analytics_columns,
     spark_schema_to_analytics_columns,
 )
-from tmlt.analytics.privacy_budget import PrivacyBudget, PureDPBudget, RhoZCDPBudget
+from tmlt.analytics._table_identifier import Identifier, NamedTable, TableCollection
+from tmlt.analytics._table_reference import (
+    TableReference,
+    find_named_tables,
+    find_reference,
+    lookup_domain,
+    lookup_metric,
+)
+from tmlt.analytics._transformation_utils import (
+    delete_table,
+    get_table_from_ref,
+    persist_table,
+    rename_table,
+    unpersist_table,
+)
+from tmlt.analytics.constraints import Constraint, MaxGroupsPerID
+from tmlt.analytics.privacy_budget import (
+    ApproxDPBudget,
+    PrivacyBudget,
+    PureDPBudget,
+    RhoZCDPBudget,
+)
 from tmlt.analytics.protected_change import (
     AddMaxRows,
     AddMaxRowsInMaxGroups,
     AddOneRow,
+    AddRowsWithID,
     ProtectedChange,
 )
 from tmlt.analytics.query_builder import ColumnType, QueryBuilder
 from tmlt.analytics.query_expr import QueryExpr
 from tmlt.core.domains.collections import DictDomain
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.interactive_measurements import (
     InactiveAccountantError,
     InsufficientBudgetError,
     PrivacyAccountant,
     PrivacyAccountantState,
     SequentialComposition,
 )
-from tmlt.core.measures import PureDP, RhoZCDP
-from tmlt.core.metrics import DictMetric, IfGroupedBy, SymmetricDifference
-from tmlt.core.transformations.dictionary import (
-    AugmentDictTransformation,
-    CreateDictFromValue,
-    GetValue,
-    Subset,
-    create_transform_value,
+from tmlt.core.measures import ApproxDP, PureDP, RhoZCDP
+from tmlt.core.metrics import AddRemoveKeys as AddRemoveKeysMetric
+from tmlt.core.metrics import (
+    DictMetric,
+    IfGroupedBy,
+    RootSumOfSquared,
+    SumOf,
+    SymmetricDifference,
 )
+from tmlt.core.transformations.base import Transformation
+from tmlt.core.transformations.dictionary import CreateDictFromValue
+from tmlt.core.transformations.identity import Identity
 from tmlt.core.transformations.spark_transformations.partition import PartitionByKeys
-from tmlt.core.transformations.spark_transformations.persist import Persist, Unpersist
 from tmlt.core.utils.configuration import SparkConfigError, check_java11
 from tmlt.core.utils.exact_number import ExactNumber
+from tmlt.core.utils.type_utils import assert_never
 
 __all__ = ["Session", "SUPPORTED_SPARK_TYPES", "TYPE_COERCION_MAP"]
 
 
 class _PrivateSourceTuple(NamedTuple):
-    """Named tuple of private Dataframe, domain and stability."""
+    """Named tuple of private Dataframe, domain and protected change."""
 
     dataframe: DataFrame
     """Private DataFrame."""
 
     protected_change: ProtectedChange
     """Protected change for this private source."""
 
@@ -101,30 +127,41 @@
 
 
 def _generate_neighboring_relation(
     sources: Dict[str, _PrivateSourceTuple]
 ) -> Conjunction:
     """Convert a collection of private source tuples into a neighboring relation."""
     relations: List[NeighboringRelation] = []
+    # this is used only for AddRemoveKeys.
+    protected_ids_dict: Dict[str, Dict[str, str]] = {}
+
     for name, (_, protected_change, _) in sources.items():
         if isinstance(protected_change, AddMaxRows):
             relations.append(AddRemoveRows(name, protected_change.max_rows))
         elif isinstance(protected_change, AddMaxRowsInMaxGroups):
             relations.append(
                 AddRemoveRowsAcrossGroups(
                     name,
                     protected_change.grouping_column,
                     max_groups=protected_change.max_groups,
                     per_group=protected_change.max_rows_per_group,
                 )
             )
+        elif isinstance(protected_change, AddRowsWithID):
+            if protected_ids_dict.get(protected_change.id_space) is None:
+                protected_ids_dict[protected_change.id_space] = {}
+            protected_ids_dict[protected_change.id_space][
+                name
+            ] = protected_change.id_column
         else:
             raise ValueError(
                 f"Unsupported ProtectedChange type: {type(protected_change)}"
             )
+    for identifier, table_to_key_column in protected_ids_dict.items():
+        relations.append(AddRemoveKeys(identifier, table_to_key_column))
     return Conjunction(relations)
 
 
 class Session:
     """Allows differentially private query evaluation on sensitive data.
 
     Sessions should not be directly constructed. Instead, they should be created
@@ -135,62 +172,48 @@
         """Builder for :class:`Session`."""
 
         def __init__(self):
             """Constructor."""
             self._privacy_budget: Optional[PrivacyBudget] = None
             self._private_sources: Dict[str, _PrivateSourceTuple] = {}
             self._public_sources: Dict[str, DataFrame] = {}
+            self._id_spaces: List[str] = []
 
         def build(self) -> "Session":
             """Builds Session with specified configuration."""
             if self._privacy_budget is None:
                 raise ValueError("Privacy budget must be specified.")
             if not self._private_sources:
                 raise ValueError("At least one private source must be provided.")
-
-            output_measure: Union[PureDP, RhoZCDP]
-            sympy_budget: sp.Expr
-            if isinstance(self._privacy_budget, PureDPBudget):
-                output_measure = PureDP()
-                sympy_budget = ExactNumber.from_float(
-                    self._privacy_budget.epsilon, round_up=False
-                ).expr
-            elif isinstance(self._privacy_budget, RhoZCDPBudget):
-                output_measure = RhoZCDP()
-                sympy_budget = ExactNumber.from_float(
-                    self._privacy_budget.rho, round_up=False
-                ).expr
-            else:
-                raise ValueError(
-                    f"Unsupported PrivacyBudget variant: {type(self._privacy_budget)}"
-                )
-
             neighboring_relation = _generate_neighboring_relation(self._private_sources)
             tables = {
                 source_id: source_tuple.dataframe
                 for source_id, source_tuple in self._private_sources.items()
             }
-            domain, metric, distance, dataframes = neighboring_relation.accept(
-                NeighboringRelationCoreVisitor(tables, output_measure)
+            sess = (
+                Session._from_neighboring_relation(  # pylint: disable=protected-access
+                    self._privacy_budget, tables, neighboring_relation
+                )
             )
+            # check list of ARK identifiers agains session's ID spaces
+            assert isinstance(neighboring_relation, Conjunction)
+            for child in neighboring_relation.children:
+                if isinstance(child, AddRemoveKeys):
+                    if child.id_space not in self._id_spaces:
+                        raise ValueError(
+                            "An AddRowsWithID protected change was specified without "
+                            "an associated identifier space for the session.\n"
+                            f"AddRowsWithID identifier provided: {child.id_space}\n"
+                            f"Identifier spaces for the session: {self._id_spaces}"
+                        )
+            # add public sources
+            for source_id, dataframe in self._public_sources.items():
+                sess.add_public_dataframe(source_id, dataframe)
 
-            compiler = QueryExprCompiler(output_measure=output_measure)
-            measurement = SequentialComposition(
-                input_domain=domain,
-                input_metric=metric,
-                d_in=distance,
-                privacy_budget=sympy_budget,
-                output_measure=output_measure,
-            )
-            accountant = PrivacyAccountant.launch(measurement, dataframes)
-            return Session(
-                accountant=accountant,
-                public_sources=self._public_sources,
-                compiler=compiler,
-            )
+            return sess
 
         def with_privacy_budget(
             self, privacy_budget: PrivacyBudget
         ) -> "Session.Builder":
             """Sets the privacy budget for the Session to be built.
 
             Args:
@@ -246,35 +269,54 @@
                         " protected_change."
                     )
                 self._private_sources[source_id] = _PrivateSourceTuple(
                     dataframe, protected_change, domain
                 )
                 return self
 
-            # TODO(#2302): All paths through the below need deprecation
+            # TODO(#2722): All paths through the below need deprecation
             #     warnings, for either the use of stability/grouping_column or
             #     the assumption of AddOneRow() if no stability is specified.
             if stability is None:
+                warn(
+                    "Using a default for protected_change is deprecated. Future"
+                    " code should explicitly specify protected_change=AddOneRow()",
+                    DeprecationWarning,
+                )
                 if grouping_column is None:
                     protected_change = AddOneRow()
                 else:
+                    warn(
+                        "Providing a grouping_column parameter instead of a"
+                        " protected_change parameter is deprecated",
+                        DeprecationWarning,
+                    )
                     protected_change = AddMaxRowsInMaxGroups(grouping_column, 1, 1)
                     grouping_column = None
             else:
+                warn(
+                    "Providing a stability instead of a protected_change is deprecated",
+                    DeprecationWarning,
+                )
                 if stability < 1:
                     raise ValueError("Stability must be a positive integer.")
 
                 if grouping_column is None:
                     if not isinstance(stability, int):
                         raise ValueError(
                             "stability must be an integer when no grouping column is"
                             " specified"
                         )
                     protected_change = AddMaxRows(stability)
                 else:
+                    warn(
+                        "Providing a grouping_column parameter instead of a"
+                        " protected_change parameter is deprecated",
+                        DeprecationWarning,
+                    )
                     if not isinstance(stability, (int, float)):
                         raise ValueError("stability must be a numeric value")
                     protected_change = AddMaxRowsInMaxGroups(
                         grouping_column, max_groups=1, max_rows_per_group=stability
                     )
                     grouping_column = None
 
@@ -299,14 +341,32 @@
             _assert_is_identifier(source_id)
             if source_id in self._private_sources or source_id in self._public_sources:
                 raise ValueError(f"Duplicate source id: '{source_id}'")
             dataframe = coerce_spark_schema_or_fail(dataframe)
             self._public_sources[source_id] = dataframe
             return self
 
+        def with_id_space(self, id_space: str) -> "Session.Builder":
+            """Sets the identifier space for the session.
+
+            This defines the space of identifiers that map 1-to-1 to the identifiers
+            being protected. Any IDs table must have exactly one column containing
+            those identifiers.
+
+            Args:
+                id_space: The identifier space for the session.
+            """
+            _assert_is_identifier(id_space)
+            if id_space in self._id_spaces:
+                raise ValueError(
+                    f"This Builder already has an ID space of the name: {id_space}."
+                )
+            self._id_spaces.append(id_space)
+            return self
+
     def __init__(
         self,
         accountant: PrivacyAccountant,
         public_sources: Dict[str, DataFrame],
         compiler: Optional[QueryExprCompiler] = None,
     ) -> None:
         """Initializes a DP session from a queryable.
@@ -338,30 +398,39 @@
             ) from exc
 
         check_type("accountant", accountant, PrivacyAccountant)
         check_type("public_sources", public_sources, Dict[str, DataFrame])
         check_type("compiler", compiler, Optional[QueryExprCompiler])
 
         self._accountant = accountant
+        if isinstance(self._accountant.output_measure, ApproxDP):
+            raise ValueError(
+                "Accountant is using ApproxDP, which is not yet supported. This is"
+                " probably a bug, please let us know so we can fix it!"
+            )
+
         if not isinstance(self._accountant.output_measure, (PureDP, RhoZCDP)):
-            raise ValueError("Accountant is not using PureDP or RhoZCDP privacy.")
+            raise ValueError("Accountant is not using PureDP or RhoZCDP.")
         if not isinstance(self._accountant.input_metric, DictMetric):
             raise ValueError("The input metric to a session must be a DictMetric.")
         if not isinstance(self._accountant.input_domain, DictDomain):
             raise ValueError("The input domain to a session must be a DictDomain.")
         self._public_sources = public_sources
         if compiler is None:
             compiler = QueryExprCompiler(output_measure=self._accountant.output_measure)
         if self._accountant.output_measure != compiler.output_measure:
             raise ValueError(
                 "PrivacyAccountant's output measure is"
                 f" {self._accountant.output_measure}, but compiler output measure is"
                 f" {compiler.output_measure}."
             )
         self._compiler = compiler
+        self._table_constraints: Dict[Identifier, List[Constraint]] = {
+            NamedTable(t): [] for t in self.private_sources
+        }
 
     # pylint: disable=line-too-long
     @classmethod
     @typechecked
     def from_dataframe(
         cls,
         privacy_budget: PrivacyBudget,
@@ -432,20 +501,100 @@
                 source_id=source_id,
                 dataframe=dataframe,
                 stability=stability,
                 grouping_column=grouping_column,
                 protected_change=protected_change,
             )
         )
+        if isinstance(protected_change, AddRowsWithID):
+            session_builder.with_id_space(protected_change.id_space)
         return session_builder.build()
 
+    @classmethod
+    @typechecked
+    def _from_neighboring_relation(
+        cls,
+        privacy_budget: PrivacyBudget,
+        private_sources: Dict[str, DataFrame],
+        relation: NeighboringRelation,
+    ) -> "Session":
+        """Initializes a DP session using the provided :class:`NeighboringRelation`.
+
+        Args:
+            privacy_budget: The total privacy budget allocated to this session.
+            private_sources: The private data to be used in the session.
+                Provided as a dictionary {source_id: Dataframe}.
+            relation: the :class:`NeighboringRelation` to be used in the session.
+        """
+        output_measure: Union[ApproxDP, PureDP, RhoZCDP]
+        sympy_budget: sp.Expr
+        if isinstance(privacy_budget, PureDPBudget):
+            output_measure = PureDP()
+            sympy_budget = ExactNumber.from_float(
+                privacy_budget.epsilon, round_up=False
+            ).expr
+        elif isinstance(privacy_budget, ApproxDPBudget):
+            output_measure = PureDP()
+            if privacy_budget.is_infinite:
+                warn(
+                    "The use of ApproxDP is not yet fully supported. Because you"
+                    " selected an infinite ApproxDP budget, your session will be"
+                    " initialized with PureDP using an infinite epsilon budget.",
+                    UserWarning,
+                )
+                sympy_budget = ExactNumber.from_float(float("inf"), round_up=False).expr
+            else:
+                warn(
+                    "The use of ApproxDP is not yet fully supported. Your session"
+                    " will be initialized with PureDP using the epsilon provided.",
+                    UserWarning,
+                )
+                sympy_budget = ExactNumber.from_float(
+                    privacy_budget.epsilon, round_up=False
+                ).expr
+        elif isinstance(privacy_budget, RhoZCDPBudget):
+            output_measure = RhoZCDP()
+            sympy_budget = ExactNumber.from_float(
+                privacy_budget.rho, round_up=False
+            ).expr
+        else:
+            raise ValueError(
+                f"Unsupported PrivacyBudget variant: {type(privacy_budget)}"
+            )
+        # ensure we have a valid source dict for the NeighboringRelation,
+        # raising exception if not.
+        relation.validate_input(private_sources)
+
+        # Wrap relation in a Conjunction so that output is appropriate for
+        # PrivacyAccountant
+        domain, metric, distance, dataframes = Conjunction(relation).accept(
+            NeighboringRelationCoreVisitor(private_sources, output_measure)
+        )
+
+        compiler = QueryExprCompiler(output_measure=output_measure)
+
+        measurement = SequentialComposition(
+            input_domain=domain,
+            input_metric=metric,
+            d_in=distance,
+            privacy_budget=sympy_budget,
+            output_measure=output_measure,
+        )
+        accountant = PrivacyAccountant.launch(measurement, dataframes)
+        return Session(accountant=accountant, public_sources={}, compiler=compiler)
+
     @property
     def private_sources(self) -> List[str]:
         """Returns the ids of the private sources."""
-        return list(self._input_domain.key_to_domain)
+        table_refs = find_named_tables(self._input_domain)
+        return [
+            t.identifier.name
+            for t in table_refs
+            if isinstance(t.identifier, NamedTable)
+        ]
 
     @property
     def public_sources(self) -> List[str]:
         """Returns the ids of the public sources."""
         return list(self._public_sources)
 
     @property
@@ -456,17 +605,24 @@
     @property
     def remaining_privacy_budget(self) -> Union[PureDPBudget, RhoZCDPBudget]:
         """Returns the remaining privacy_budget left in the session.
 
         The type of the budget (e.g., PureDP or rho-zCDP) will be the same as
         the type of the budget the Session was initialized with.
         """
+        output_measure = self._accountant.output_measure
+        if isinstance(output_measure, ApproxDP):
+            raise ValueError(
+                "Accountant is using ApproxDP, which is not yet supported. This is"
+                " probably a bug, please let us know so we can fix it!"
+            )
+
         sympy_budget = self._accountant.privacy_budget
         budget_value = ExactNumber(sympy_budget).to_float(round_up=False)
-        output_measure = self._accountant.output_measure
+
         if output_measure == PureDP():
             return PureDPBudget(budget_value)
         if output_measure == RhoZCDP():
             return RhoZCDPBudget(budget_value)
         raise RuntimeError(
             "Unexpected behavior in remaining_privacy_budget. Please file a bug report."
         )
@@ -476,58 +632,59 @@
         """Returns the input domain of the underlying queryable."""
         if not isinstance(self._accountant.input_domain, DictDomain):
             raise AssertionError(
                 "Session accountant's input domain has an incorrect type. This is "
                 "probably a bug; please let us know about it so we can "
                 "fix it!"
             )
-        return cast(DictDomain, self._accountant.input_domain)
+        return self._accountant.input_domain
 
     @property
     def _input_metric(self) -> DictMetric:
         """Returns the input metric of the underlying accountant."""
         if not isinstance(self._accountant.input_metric, DictMetric):
             raise AssertionError(
                 "Session accountant's input metric has an incorrect type. This is "
                 "probably a bug; please let us know about it so we can "
                 "fix it!"
             )
-        return cast(DictMetric, self._accountant.input_metric)
-
-    @property
-    def _stability(self) -> Dict[str, sp.Expr]:
-        """Returns the unmodified stability of the underlying PrivacyAccountant."""
-        return {
-            source_id: ExactNumber(d_in_i).expr
-            for source_id, d_in_i in self._accountant.d_in.items()
-        }
+        return self._accountant.input_metric
 
     @typechecked
     def get_schema(self, source_id: str) -> Schema:
         """Returns the schema for any data source.
 
         This includes information on whether the columns are nullable.
 
         Args:
             source_id: The ID for the data source whose column types
                 are being retrieved.
         """
-        # TODO(#2172):replace old source indexing method with use of new lookup feature
-        if source_id in self._input_domain.key_to_domain:
+        ref = find_reference(source_id, self._input_domain)
+        id_space: Optional[str] = None
+        if source_id in self.private_sources:
+            id_space = self.get_id_space(source_id)
+        if ref is not None:
+            domain = lookup_domain(self._input_domain, ref)
             return Schema(
-                spark_dataframe_domain_to_analytics_columns(
-                    self._input_domain[source_id]
-                )
+                spark_dataframe_domain_to_analytics_columns(domain), id_space=id_space
             )
         else:
-            return Schema(
-                spark_schema_to_analytics_columns(
-                    self.public_source_dataframes[source_id].schema
+            try:
+                return Schema(
+                    spark_schema_to_analytics_columns(
+                        self.public_source_dataframes[source_id].schema
+                    ),
+                    id_space=id_space,
                 )
-            )
+            except KeyError:
+                raise KeyError(
+                    f"Table '{source_id}' does not exist. Available tables "
+                    f"are: {', '.join(self.private_sources + self.public_sources)}"
+                ) from None
 
     @typechecked
     def get_column_types(self, source_id: str) -> Dict[str, ColumnType]:
         """Returns the column types for any data source.
 
         This does *not* include information on whether the columns are nullable.
         """
@@ -543,60 +700,105 @@
         When a groupby aggregation is appended to any query on this table, it
         must include this column as a groupby column.
 
         Args:
             source_id: The ID for the data source whose grouping column
                 is being retrieved.
         """
-        try:
-            if isinstance(self._input_metric[source_id], IfGroupedBy):
-                inner_metric = cast(IfGroupedBy, self._input_metric[source_id])
-                return inner_metric.column
-            return None
-        except KeyError as e:
+        ref = find_reference(source_id, self._input_domain)
+        if ref is None:
+            if source_id in self.public_sources:
+                raise ValueError(
+                    f"Table '{source_id}' is a public table, which cannot have a "
+                    "grouping column."
+                )
+            raise KeyError(
+                f"Private table '{source_id}' does not exist. "
+                f"Available private tables are: {', '.join(self.private_sources)}"
+            )
+        metric = lookup_metric(self._input_metric, ref)
+        if isinstance(metric, IfGroupedBy) and isinstance(
+            metric.inner_metric, (SumOf, RootSumOfSquared)
+        ):
+            return metric.column
+        return None
+
+    @typechecked
+    def get_id_column(self, source_id: str) -> Optional[str]:
+        """Returns the ID column of a table, if it has one.
+
+        Args:
+            source_id: The name of the table whose ID column is being retrieved.
+        """
+        ref = find_reference(source_id, self._input_domain)
+        if ref is None:
+            if source_id in self.public_sources:
+                raise ValueError(
+                    f"Table '{source_id}' is a public table, which cannot have a "
+                    "grouping column."
+                )
+            raise KeyError(
+                f"Private table '{source_id}' does not exist. "
+                f"Available private tables are: {', '.join(self.private_sources)}"
+            )
+        metric = lookup_metric(self._input_metric, ref)
+        if isinstance(metric, IfGroupedBy) and isinstance(
+            metric.inner_metric, SymmetricDifference
+        ):
+            return metric.column
+        return None
+
+    @typechecked
+    def get_id_space(self, source_id: str) -> Optional[str]:
+        """Returns the ID space of a table, if it has one.
+
+        Args:
+            source_id: The name of the table whose ID space is being retrieved.
+        """
+        # Make sure the table exists
+        ref = find_reference(source_id, self._input_domain)
+        if ref is None:
             if source_id in self.public_sources:
                 raise ValueError(
-                    f"'{source_id}' does not have a grouping column, "
-                    "because it is not a private table."
+                    f"Table '{source_id}' is a public table, which cannot have an "
+                    "ID space."
                 )
-            raise e
+            raise KeyError(
+                f"Private table '{source_id}' does not exist. "
+                f"Available private tables are: {', '.join(self.private_sources)}"
+            )
+        # Tables not in an ID space will have a parent of ([])
+        if ref.parent == TableReference([]):
+            return None
+        # Otherwise, the parent should be a TableCollection("id_space")
+        parent_identifier = ref.parent.identifier
+        assert isinstance(parent_identifier, TableCollection), (
+            "Expected parent to be a table collection but got"
+            f" {parent_identifier} instead. This is probably a bug; please let us know"
+            " about it so we can fix it!"
+        )
+        return parent_identifier.name
 
     @property
     def _catalog(self) -> Catalog:
-        """Returns the catalog."""
+        """Returns a Catalog of tables in the Session."""
         catalog = Catalog()
-        primary_source_id = list(self.private_sources)[0]
-        view_source_ids = [
-            source_id
-            for source_id in self.private_sources
-            if source_id != primary_source_id
-        ]
-        catalog.add_private_source(
-            source_id=primary_source_id,
-            col_types=self.get_schema(primary_source_id),
-            # Catalogs require an integral stability. The catalog is only used for query
-            # validation, so using the incorrect stability (if the true stability is
-            # non-integral) is ok.
-            stability=int(self._stability[primary_source_id]),
-            grouping_column=self.get_grouping_column(primary_source_id),
-        )
-        for view_source_id in view_source_ids:
-            catalog.add_private_view(
-                view_source_id,
-                self.get_schema(view_source_id),
-                # Catalogs require integral stability, see note above.
-                int(self._stability[view_source_id]),
-                self.get_grouping_column(view_source_id),
-            )
-
-        for public_source_id in self.public_sources:
-            catalog.add_public_source(
-                public_source_id,
+        for table in self.private_sources:
+            catalog.add_private_table(
+                table,
+                self.get_schema(table),
+                grouping_column=self.get_grouping_column(table),
+                id_column=self.get_id_column(table),
+                id_space=self.get_id_space(table),
+            )
+        for table in self.public_sources:
+            catalog.add_public_table(
+                table,
                 spark_schema_to_analytics_columns(
-                    self.public_source_dataframes[public_source_id].schema
+                    self.public_source_dataframes[table].schema
                 ),
             )
         return catalog
 
     # pylint: disable=line-too-long
     @typechecked
     def add_public_dataframe(self, source_id: str, dataframe: DataFrame):
@@ -645,43 +847,41 @@
 
         Args:
             source_id: The name of the public data source.
             dataframe: The public data source corresponding to the ``source_id``.
         """
         # pylint: enable=line-too-long
         _assert_is_identifier(source_id)
-        if source_id in self._public_sources:
-            raise ValueError(
-                "This session already has a public source with the source_id"
-                f" {source_id}"
-            )
+        if source_id in self.public_sources or source_id in self.private_sources:
+            raise ValueError(f"This session already has a table named '{source_id}'.")
         dataframe = coerce_spark_schema_or_fail(dataframe)
         self._public_sources[source_id] = dataframe
 
     def _compile_and_get_budget(
         self, query_expr: QueryExpr, privacy_budget: PrivacyBudget
     ) -> Tuple[Measurement, ExactNumber]:
         """Pre-processing needed for evaluate() and _noise_info()."""
         check_type("query_expr", query_expr, QueryExpr)
         check_type("privacy_budget", privacy_budget, PrivacyBudget)
 
         self._validate_budget_type_matches_session(privacy_budget)
-        if privacy_budget == PureDPBudget(0) or privacy_budget == RhoZCDPBudget(0):
+        if privacy_budget in [PureDPBudget(0), ApproxDPBudget(0, 0), RhoZCDPBudget(0)]:
             raise ValueError("You need a non-zero privacy budget to evaluate a query.")
 
         adjusted_budget = self._process_requested_budget(privacy_budget)
 
         measurement = self._compiler(
             queries=[query_expr],
             privacy_budget=adjusted_budget.expr,
-            stability=self._stability,
+            stability=self._accountant.d_in,
             input_domain=self._input_domain,
             input_metric=self._input_metric,
             public_sources=self._public_sources,
             catalog=self._catalog,
+            table_constraints=self._table_constraints,
         )
         return (measurement, adjusted_budget)
 
     def _noise_info(
         self, query_expr: QueryExpr, privacy_budget: PrivacyBudget
     ) -> List[Dict[str, Any]]:
         """Get noise information about a query.
@@ -787,34 +987,41 @@
                 raise ValueError(
                     "With these inputs and this privacy budget, "
                     "similar inputs will *not* produce similar outputs. "
                 )
             try:
                 answers = self._accountant.measure(measurement, d_out=adjusted_budget)
             except InsufficientBudgetError:
-                approx_budget_needed = adjusted_budget.to_float(round_up=True)
+                if not isinstance(self._accountant.privacy_budget, ExactNumber):
+                    raise ValueError(
+                        "Expected privacy_budget to be an ExactNumber, but instead"
+                        f" received {type(self._accountant.privacy_budget)}."
+                    )
+
+                approximate_budget_needed = adjusted_budget.to_float(round_up=True)
                 if not isinstance(self._accountant.privacy_budget, ExactNumber):
                     raise AssertionError(
                         "Unable to convert privacy budget of"
                         f" {self._accountant.privacy_budget} to float. This is probably"
                         " a bug; please let us know about it so we can fix it!"
                     )
-                approx_budget_left = self._accountant.privacy_budget.to_float(
+                approximate_budget_left = self._accountant.privacy_budget.to_float(
                     round_up=False
                 )
-                approx_diff = abs(
+                approximate_diff = abs(
                     (self._accountant.privacy_budget - adjusted_budget).to_float(
                         round_up=True
                     )
                 )
                 raise RuntimeError(
                     "Cannot answer query without exceeding privacy budget: it needs"
-                    f" approximately {approx_budget_needed:.3f}, but the remaining"
-                    f" budget is approximately {approx_budget_left:.3f} (difference:"
-                    f" {approx_diff:.3e})"
+                    f" approximately {approximate_budget_needed:.3f}, but the remaining"
+                    " budget is approximately"
+                    f" {approximate_budget_left:.3f} (difference:"
+                    f" {approximate_diff:.3e})"
                 )
             if len(answers) != 1:
                 raise AssertionError(
                     "Expected exactly one answer, but got "
                     f"{len(answers)} answers instead. This is "
                     "probably a bug; please let us know about it so "
                     "we can fix it!"
@@ -876,15 +1083,15 @@
             ... )
             >>> sess.create_view(
             ...     join_query,
             ...     source_id="private_public_join",
             ...     cache=True
             ... )
             >>> sess.private_sources
-            ['my_private_data', 'private_public_join']
+            ['private_public_join', 'my_private_data']
             >>> sess.get_schema("private_public_join").column_types # doctest: +NORMALIZE_WHITESPACE
             {'A': 'VARCHAR', 'B': 'INTEGER', 'C': 'INTEGER'}
             >>> # Delete the view
             >>> sess.delete_view("private_public_join")
             >>> sess.private_sources
             ['my_private_data']
 
@@ -892,89 +1099,87 @@
             query_expr: A query that performs a transformation.
             source_id: The name, or unique identifier, of the view.
             cache: Whether or not to cache the view.
         """
         # pylint: enable=line-too-long
         _assert_is_identifier(source_id)
         self._activate_accountant()
-        if source_id in self._input_domain.key_to_domain:
-            raise ValueError(f"ID {source_id} already exists.")
+        if source_id in self.private_sources or source_id in self.public_sources:
+            raise ValueError(f"Table '{source_id}' already exists.")
 
         if isinstance(query_expr, QueryBuilder):
             query_expr = query_expr.query_expr
 
         if not isinstance(query_expr, QueryExpr):
             raise ValueError("query_expr must be of type QueryBuilder or QueryExpr.")
-        transformation = self._compiler.build_transformation(
+        transformation, ref, constraints = self._compiler.build_transformation(
             query=query_expr,
             input_domain=self._input_domain,
             input_metric=self._input_metric,
             public_sources=self._public_sources,
             catalog=self._catalog,
+            table_constraints=self._table_constraints,
         )
         if cache:
-            transformation = transformation | Persist(
-                domain=cast(SparkDataFrameDomain, transformation.output_domain),
-                metric=transformation.output_metric,
+            transformation, ref = persist_table(
+                base_transformation=transformation, base_ref=ref
             )
 
-        dict_transformation = AugmentDictTransformation(
-            transformation
-            | CreateDictFromValue(
-                input_domain=transformation.output_domain,
-                input_metric=transformation.output_metric,
-                key=source_id,
-            )
+        transformation, _ = rename_table(
+            base_transformation=transformation,
+            base_ref=ref,
+            new_table_id=NamedTable(source_id),
         )
-
-        # This is a transform-in-place against the privacy accountant
-        self._accountant.transform_in_place(dict_transformation)
+        self._accountant.transform_in_place(transformation)
+        self._table_constraints[NamedTable(source_id)] = constraints
 
     def delete_view(self, source_id: str):
         """Deletes a view and decaches it if it was cached.
 
         Args:
             source_id: The name of the view.
         """
-        if source_id not in self._input_domain.key_to_domain:
-            raise ValueError(f"ID {source_id} does not exist.")
         self._activate_accountant()
 
-        # Unpersist does nothing if the DataFrame isn't persisted
-        domain = cast(SparkDataFrameDomain, self._input_domain.key_to_domain[source_id])
-        metric = self._input_metric.key_to_metric[source_id]
-        unpersist_source = create_transform_value(
-            input_domain=cast(DictDomain, self._accountant.input_domain),
-            input_metric=cast(DictMetric, self._accountant.input_metric),
-            key=source_id,
-            transformation=Unpersist(domain, metric),
-            hint=lambda d_in, _: d_in,
+        ref = find_reference(source_id, self._input_domain)
+        if ref is None:
+            raise KeyError(
+                f"Private table '{source_id}' does not exist. "
+                f"Available tables are: {', '.join(self.private_sources)}"
+            )
+
+        domain = lookup_domain(self._input_domain, ref)
+        if not isinstance(domain, SparkDataFrameDomain):
+            raise RuntimeError(
+                "Table domain is not SparkDataFrameDomain. This is probably a bug; "
+                "please let us know so we can fix it!"
+            )
+
+        unpersist_source: Transformation = Identity(
+            domain=self._input_domain, metric=self._input_metric
         )
-        self._accountant.transform_in_place(
-            unpersist_source, d_out=self._accountant.d_in
+        # Unpersist does nothing if the DataFrame isn't persisted
+        unpersist_source = unpersist_table(
+            base_transformation=unpersist_source, base_ref=ref
         )
 
-        transformation = Subset(
-            input_domain=self._input_domain,
-            input_metric=self._input_metric,
-            keys=list(set(self._input_domain.key_to_domain.keys()) - {source_id}),
+        transformation = delete_table(
+            base_transformation=unpersist_source, base_ref=ref
         )
-        d_out = {k: v for k, v in self._accountant.d_in.items() if k != source_id}
-        self._accountant.transform_in_place(transformation, d_out)
+        self._accountant.transform_in_place(transformation)
+        self._table_constraints.pop(ref.identifier, None)
 
     # pylint: disable=line-too-long
-    # TODO(#2199): remove the attr_name argument
     @typechecked
     def partition_and_create(
         self,
         source_id: str,
         privacy_budget: PrivacyBudget,
         column: Optional[str] = None,
         splits: Optional[Union[Dict[str, str], Dict[str, int]]] = None,
-        attr_name: Optional[str] = None,
     ) -> Dict[str, "Session"]:
         """Returns new sessions from a partition mapped to split name/``source_id``.
 
         The type of privacy budget that you use must match the type your Session was
         initialized with (i.e., you cannot use a RhoZCDPBudget to partition your
         Session if the Session was created using a PureDPBudget, and vice versa).
 
@@ -1050,54 +1255,74 @@
 
         Args:
             source_id: The private source to partition.
             privacy_budget: Amount of privacy budget to pass to each new session.
             column: The name of the column partitioning on.
             splits: Mapping of split name to value of partition.
                 Split name is ``source_id`` in new session.
-            attr_name: Deprecated synonym for ``column``. Using the ``column`` argument
-                is preferred.
         """
         # pylint: enable=line-too-long
-        if column is None and attr_name is None:
-            raise ValueError("Please specify a column using the column parameter")
-        if column is not None and attr_name is not None:
-            raise ValueError("You cannot specify both a column and an attr_name")
-        if attr_name is not None:
-            warn(
-                "The attr_name argument is deprecated and will be removed in a future"
-                " release",
-                DeprecationWarning,
-            )
-            column = attr_name
         if splits is None:
             raise ValueError(
                 "You must provide a dictionary mapping split names (new source_ids) to"
                 " values on which to partition"
             )
         # If you remove this if-block, mypy will complain
         if column is None:
             raise AssertionError(
                 "column is None, even though either column or attr_name were provided."
                 " This is probably a bug; please let us know about it so we can fix it!"
             )
         self._validate_budget_type_matches_session(privacy_budget)
         self._activate_accountant()
 
-        transformation = GetValue(
-            input_domain=self._input_domain,
-            input_metric=self._input_metric,
-            key=source_id,
+        transformation: Transformation = Identity(
+            domain=self._input_domain, metric=self._input_metric
         )
-        d_mid = self._accountant.d_in[source_id]
-        if not transformation.stability_relation(self._accountant.d_in, d_mid):
-            raise ValueError(
-                "This partition is unstable: close inputs will not produce "
-                "close outputs."
+        table_ref = find_reference(source_id, self._input_domain)
+        assert isinstance(table_ref, TableReference)
+
+        # Either DictMetric or AddRemoveKeys
+        parent_metric = lookup_metric(self._input_metric, table_ref.parent)
+        table_has_ids: bool = isinstance(parent_metric, AddRemoveKeysMetric)
+        if table_has_ids:
+            parent_last_element = table_ref.parent.identifier
+            constraints = self._table_constraints.get(NamedTable(source_id))
+            if constraints is None:
+                raise AssertionError(
+                    f"Table '{source_id}' has no constraints. This is probably a"
+                    " bug; please let us know about it so we can fix it!"
+                )
+
+            constraint = next(
+                (
+                    c
+                    for c in constraints
+                    if (isinstance(c, MaxGroupsPerID) and c.grouping_column == column)
+                ),
+                None,
+            )
+
+            if constraint is None:
+                raise ValueError(
+                    "You must create MaxGroupsPerID constraint before using"
+                    " partition_and_create on tables with the AddRowsWithID"
+                    " protected change."
+                )
+
+            (
+                transformation,
+                table_ref,
+            ) = constraint._enforce(  # pylint: disable=protected-access
+                child_transformation=transformation,
+                child_ref=table_ref,
+                update_metric=True,
+                use_l2=isinstance(self._compiler.output_measure, RhoZCDP),
             )
+        transformation = get_table_from_ref(transformation, table_ref)
         if not isinstance(
             transformation.output_metric, (IfGroupedBy, SymmetricDifference)
         ):
             raise AssertionError(
                 "Transformation has an unrecognized output metric. This is "
                 "probably a bug; please let us know about it so we can fix it!"
             )
@@ -1128,36 +1353,48 @@
                 raise TypeError(
                     f"'{column}' column is of type '{attr_type.data_type}'; "
                     f"'{attr_type.data_type}' column not compatible with splits "
                     f"value type '{type(split_val).__name__}'"
                 )
             new_sources.append(split_name)
             split_vals.append((split_val,))
+
         element_metric: Union[IfGroupedBy, SymmetricDifference]
-        if (
+        if isinstance(transformation.output_metric, SymmetricDifference) or (
             isinstance(transformation.output_metric, IfGroupedBy)
             and column != transformation.output_metric.column
         ):
             element_metric = transformation.output_metric
+        elif (
+            isinstance(transformation.output_metric, IfGroupedBy)
+            and column == transformation.output_metric.column
+        ):
+            assert isinstance(
+                transformation.output_metric.inner_metric,
+                (IfGroupedBy, RootSumOfSquared, SumOf),
+            )
+            assert isinstance(
+                transformation.output_metric.inner_metric.inner_metric,
+                (IfGroupedBy, SymmetricDifference),
+            )
+            element_metric = transformation.output_metric.inner_metric.inner_metric
         else:
-            element_metric = SymmetricDifference()
+            raise AssertionError(
+                "Transformation has an unrecognized output metric. This is "
+                "probably a bug; please let us know about it so  we can fix it!"
+            )
+
         partition_transformation = PartitionByKeys(
             input_domain=transformation_domain,
             input_metric=transformation.output_metric,
             use_l2=isinstance(self._compiler.output_measure, RhoZCDP),
             keys=[column],
             list_values=split_vals,
         )
         chained_partition = transformation | partition_transformation
-        if transformation.stability_function(self._accountant.d_in) != d_mid:
-            raise AssertionError(
-                "Transformation's stability function does not match "
-                "transformed data. This is probably a bug; please let us "
-                "know about it so we can fix it!"
-            )
 
         adjusted_budget = self._process_requested_budget(privacy_budget)
 
         try:
             new_accountants = self._accountant.split(
                 chained_partition, privacy_budget=adjusted_budget
             )
@@ -1165,43 +1402,63 @@
             raise RuntimeError(
                 "This session is no longer active. Either it was manually stopped"
                 "with session.stop(), or it was stopped indirectly by the "
                 "activity of other sessions. See partition_and_create "
                 "for more information."
             )
         except InsufficientBudgetError:
-            approx_budget_needed = adjusted_budget.to_float(round_up=True)
+            if not isinstance(self._accountant.privacy_budget, ExactNumber):
+                raise ValueError(
+                    "Expected privacy_budget to be an ExactNumber, but instead"
+                    f" received {type(self._accountant.privacy_budget)}."
+                )
+
+            approximate_budget_needed = adjusted_budget.to_float(round_up=True)
             if not isinstance(self._accountant.privacy_budget, ExactNumber):
                 raise AssertionError(
                     "Unable to convert privacy budget of"
                     f" {self._accountant.privacy_budget} to float. This is probably a"
                     " bug; please let us know about it so we can fix it!"
                 )
 
-            approx_budget_left = self._accountant.privacy_budget.to_float(
+            approximate_budget_left = self._accountant.privacy_budget.to_float(
                 round_up=False
             )
-            approx_diff = abs(
+            approximate_diff = abs(
                 (self._accountant.privacy_budget - adjusted_budget).to_float(
                     round_up=True
                 )
             )
             raise RuntimeError(
                 "Cannot perform this partition without exceeding privacy budget: it"
-                f" needs approximately {approx_budget_needed:.3f}, but the remaining"
-                f" budget is approximately {approx_budget_left:.3f} (difference:"
-                f" {approx_diff:.3e})"
+                f" needs approximately {approximate_budget_needed:.3f}, but the"
+                " remaining budget is approximately"
+                f" {approximate_budget_left:.3f} (difference: {approximate_diff:.3e})"
             )
 
         for i, source in enumerate(new_sources):
-            dict_transformation_wrapper = CreateDictFromValue(
-                input_domain=transformation_domain,
-                input_metric=element_metric,
-                key=source,
-            )
+            if table_has_ids:
+                create_dict = CreateDictFromValue(
+                    input_domain=transformation_domain,
+                    input_metric=element_metric,
+                    key=NamedTable(source),
+                    use_add_remove_keys=True,
+                )
+                dict_transformation_wrapper = create_dict | CreateDictFromValue(
+                    input_domain=create_dict.output_domain,
+                    input_metric=create_dict.output_metric,
+                    key=parent_last_element,
+                )
+            else:
+                dict_transformation_wrapper = CreateDictFromValue(
+                    input_domain=transformation_domain,
+                    input_metric=element_metric,
+                    key=NamedTable(source),
+                )
+
             new_accountants[i].queue_transformation(
                 transformation=dict_transformation_wrapper
             )
 
         new_sessions = dict()
         for new_accountant, source in zip(new_accountants, new_sources):
             new_sessions[source] = Session(
@@ -1219,14 +1476,32 @@
         if not isinstance(remaining_budget, ExactNumber):
             raise AssertionError(
                 f"Cannot understand remaining budget of {remaining_budget}. This is"
                 " probably a bug; please let us know about it so we can fix it!"
             )
         if isinstance(privacy_budget, PureDPBudget):
             return get_adjusted_budget(privacy_budget.epsilon, remaining_budget)
+
+        if isinstance(privacy_budget, ApproxDPBudget):
+            if privacy_budget.is_infinite:
+                warn(
+                    "The use of ApproxDP is not yet fully supported. Because you"
+                    " selected an infinite ApproxDP budget, your budget request"
+                    " will be processed as PureDP with an infinite epsilon budget.",
+                    UserWarning,
+                )
+                return ExactNumber.from_float(float("inf"), round_up=False)
+            else:
+                warn(
+                    "The use of ApproxDP is not yet fully supported. your budget"
+                    " request will be processed as PureDP using the epsilon"
+                    " provided.",
+                    UserWarning,
+                )
+                return get_adjusted_budget(privacy_budget.epsilon, remaining_budget)
         elif isinstance(privacy_budget, RhoZCDPBudget):
             return get_adjusted_budget(privacy_budget.rho, remaining_budget)
         else:
             raise ValueError(
                 f"Unsupported variant of PrivacyBudget. Found {type(privacy_budget)}"
             )
 
@@ -1238,18 +1513,21 @@
         Args:
             privacy_budget: The requested budget.
         """
         output_measure = self._accountant.output_measure
         matches_puredp = isinstance(output_measure, PureDP) and isinstance(
             privacy_budget, PureDPBudget
         )
+        matches_approxdp = isinstance(output_measure, PureDP) and isinstance(
+            privacy_budget, ApproxDPBudget
+        )
         matches_zcdp = isinstance(output_measure, RhoZCDP) and isinstance(
             privacy_budget, RhoZCDPBudget
         )
-        if not (matches_puredp or matches_zcdp):
+        if not (matches_puredp or matches_approxdp or matches_zcdp):
             raise ValueError(
                 "Your requested privacy budget type must match the type of the privacy"
                 " budget your Session was created with."
             )
 
     def _activate_accountant(self) -> None:
         if self._accountant.state == PrivacyAccountantState.ACTIVE:
@@ -1271,20 +1549,161 @@
             )
         self._accountant.force_activate()
 
     def stop(self) -> None:
         """Close out this session, allowing other sessions to become active."""
         self._accountant.retire()
 
+    def describe(self, x: Optional[Union[QueryExpr, QueryBuilder, str]] = None) -> None:
+        """Describe this session, or a query, or a table.
+
+        If ``x`` is ``None``, ``session._describe(x)`` will describe the session.
+
+        If ``x`` is a
+        :class:`~tmlt.analytics.query_expr.QueryExpr`,
+        ``session._describe(x)`` will describe
+        the schema resulting from that query expression.
+
+        If x is a
+        :class:`~tmlt.analytics.query_builder.QueryBuilder`,
+        ``session._describe(x) will describe the query constructed by the
+        query builder. This is equivalent to calling
+        ``session._describe(x.query_expr)``.
+
+        If x is a string, x is assumed to be a table name. In this case,
+        ``session._describe(x)`` is equivalent to
+        ``session._describe(QueryBuilder(x))``.
+        """
+        if x is None:
+            self._describe_self()
+        elif isinstance(x, QueryExpr):
+            self._describe_query(x)
+        elif isinstance(x, QueryBuilder):
+            self._describe_query(x.query_expr)
+        elif isinstance(x, str):
+            self._describe_query(QueryBuilder(x).query_expr)
+        else:
+            assert_never(x)
+
+    def _describe_self(self) -> None:
+        """Describe the current state of this session."""
+        out = []
+        state = self._accountant.state
+        if state == PrivacyAccountantState.ACTIVE:
+            # Don't add anything to output if the session is active
+            pass
+        elif state == PrivacyAccountantState.RETIRED:
+            out.append("This session has been stopped, and can no longer be used.")
+        elif state == PrivacyAccountantState.WAITING_FOR_CHILDREN:
+            out.append(
+                "This session is waiting for its children (created with"
+                " `partition_and_create`) to finish."
+            )
+        elif state == PrivacyAccountantState.WAITING_FOR_SIBLING:
+            out.append(
+                "This session is waiting for its sibling(s) (created with"
+                " `partition_and_create`) to finish."
+            )
+        else:
+            raise AssertionError(
+                f"Unrecognized accountant state {out}. This is probably a bug; please"
+                " let us know about it so we can fix it!"
+            )
+        budget: PrivacyBudget = self.remaining_privacy_budget
+        out.append(f"The session has a remaining privacy budget of {budget}.")
+        if len(self._catalog.tables) == 0:
+            out.append("The session has no tables available.")
+        else:
+            public_table_descs = []
+            private_table_descs = []
+            for name, table in self._catalog.tables.items():
+                column_strs = ["\t" + e for e in _describe_schema(table.schema)]
+                columns_desc = "\n".join(column_strs)
+                if isinstance(table, PublicTable):
+                    table_desc = f"Public table '{name}':\n" + columns_desc
+                    public_table_descs.append(table_desc)
+                elif isinstance(table, PrivateTable):
+                    table_desc = f"Table '{name}':\n"
+                    table_desc += columns_desc
+
+                    constraints: Optional[
+                        List[Constraint]
+                    ] = self._table_constraints.get(NamedTable(name))
+                    if not constraints:
+                        table_desc = (
+                            f"Table '{name}' (no constraints):\n" + columns_desc
+                        )
+                    else:
+                        table_desc = (
+                            f"Table '{name}':\n" + columns_desc + "\n\tConstraints:\n"
+                        )
+                        constraints_strs = [f"\t\t- {e}" for e in constraints]
+                        table_desc += "\n".join(constraints_strs)
+
+                    private_table_descs.append(table_desc)
+                else:
+                    raise AssertionError(
+                        f"Table {name} has an unrecognized type: {type(table)}. This is"
+                        " probably a bug; please let us know about it so we can"
+                        " fix it!"
+                    )
+            if len(private_table_descs) != 0:
+                out.append(
+                    "The following private tables are available:\n"
+                    + "\n".join(private_table_descs)
+                )
+            if len(public_table_descs) != 0:
+                out.append(
+                    "The following public tables are available:\n"
+                    + "\n".join(public_table_descs)
+                )
+        print("\n".join(out))
+
+    def _describe_query(self, query: QueryExpr):
+        """Describe the output schema of a query and the constraints on it."""
+        schema = self._compiler.query_schema(query, self._catalog)
+        out = _describe_schema(schema)
+        print("\n".join(out))
+
 
 def _assert_is_identifier(source_id: str):
     """Checks that the ``source_id`` is a valid Python identifier.
 
     Args:
         source_id: The name of the dataframe or transformation.
     """
     if not source_id.isidentifier():
         raise ValueError(
             "The string passed as source_id must be a valid Python identifier: it can"
             " only contain alphanumeric letters (a-z) and (0-9), or underscores (_),"
             " and it cannot start with a number, or contain any spaces."
         )
+
+
+def _describe_schema(schema: Schema) -> List[str]:
+    """Get a list of strings to print that describe columns of a schema.
+
+    This is a list so that it's easy to append tabs to each line.
+    """
+    description = ["Columns:"]
+    # We actually care about the maximum length of the column name
+    # *as enclosed in quotes*,
+    # so we add 2 to account for the opening and closing quotation marks
+    column_length = (
+        max(len(column_name) for column_name in schema.column_descs.keys()) + 2
+    )
+    for column_name, cd in schema.column_descs.items():
+        quoted_column_name = f"'{column_name}'"
+        column_str = f"\t- {quoted_column_name:<{column_length}}  {cd.column_type}"
+        if column_name == schema.id_column:
+            column_str += f", ID column (in ID space {schema.id_space})"
+        if column_name == schema.grouping_column:
+            column_str += ", grouping column"
+        if not cd.allow_null:
+            column_str += ", not null"
+        if cd.column_type == ColumnType.DECIMAL:
+            if not cd.allow_nan:
+                column_str += ", not NaN"
+            if not cd.allow_inf:
+                column_str += ", not infinity"
+        description.append(column_str)
+    return description
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/truncation_strategy.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/truncation_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Defines strategies for performing truncation in private joins."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
 
 from abc import ABC
 from dataclasses import dataclass
 
 from typeguard import check_type
```

### Comparing `tmlt_analytics-0.6.1/tmlt/analytics/utils.py` & `tmlt_analytics-0.7.0rc1/tmlt/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.6.1/setup.py` & `tmlt_analytics-0.7.0rc1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['tmlt', 'tmlt.analytics', 'tmlt.analytics._query_expr_compiler']
+['tmlt',
+ 'tmlt.analytics',
+ 'tmlt.analytics._query_expr_compiler',
+ 'tmlt.analytics.constraints']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.2.0,<2.0.0',
  'pyspark[sql]>=3.0.0,<3.4.0',
  'sympy>=1.8,<1.10',
- 'tmlt.core>=0.6.0,<0.7.0',
+ 'tmlt.core>=0.9.0,<0.10.0',
  'typeguard>=2.12.1,<2.13.0',
  'typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'tmlt-analytics',
-    'version': '0.6.1',
+    'version': '0.7.0rc1',
     'description': "Tumult's differential privacy analytics API",
-    'long_description': '# Tumult Analytics\n\nTumult Analytics is a library that allows users to execute differentially private operations on\ndata without having to worry about the privacy implementation, which is handled\nautomatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).\n\n## Installation\n\nSee the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)\nfor information about setting up prerequisites such as Spark.\n\nOnce the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project.pip).\n\n```bash\npip install tmlt.analytics\n```\n\n## Documentation\n\nThe full documentation is located at https://docs.tmlt.dev/analytics/latest/.\n\n## Support\n\nIf you have any questions/concerns, please [create an issue](https://gitlab.com/tumult-labs/analytics/-/issues) or reach out to us on [Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\n## Contributing\n\nWe are not yet accepting external contributions, but please let us know if you are interested in contributing [via Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.\n\n## License\n\nCopyright Tumult Labs 2022\n\nThe Tumult Platform source code is licensed under the Apache License, version 2.0 (Apache-2.0).\nThe Tumult Platform documentation is licensed under\nCreative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).\n',
+    'long_description': '# Tumult Analytics\n\nTumult Analytics is a library that allows users to execute differentially private operations on\ndata without having to worry about the privacy implementation, which is handled\nautomatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).\n\n## Installation\n\nSee the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)\nfor information about setting up prerequisites such as Spark.\n\nOnce the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project/pip).\n\n```bash\npip install tmlt.analytics\n```\n\n## Documentation\n\nThe full documentation is located at https://docs.tmlt.dev/analytics/latest/.\n\n## Support\n\nIf you have any questions/concerns, please [create an issue](https://gitlab.com/tumult-labs/analytics/-/issues) or reach out to us on [Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\n## Contributing\n\nWe are not yet accepting external contributions, but please let us know if you are interested in contributing [via Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.\n\n## Citing Tumult Analytics\n\nIf you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.\n\n```\n@software{tumultanalyticssoftware,\n    author = {Tumult Labs},\n    title = {Tumult {{Analytics}}},\n    month = dec,\n    year = 2022,\n    version = {latest},\n    url = {https://tmlt.dev}\n}\n```\n\n```\n@article{tumultanalyticswhitepaper,\n  title={Tumult {{Analytics}}: a robust, easy-to-use, scalable, and expressive framework for differential privacy},\n  author={Berghel, Skye and Bohannon, Philip and Desfontaines, Damien and Estes, Charles and Haney, Sam and Hartman, Luke and Hay, Michael and Machanavajjhala, Ashwin and Magerlein, Tom and Miklau, Gerome and Pai, Amritha and Sexton, William and Shrestha, Ruchit},\n  journal={arXiv preprint arXiv:2212.04133},\n  month = dec,\n  year={2022}\n}\n```\n\n## License\n\nCopyright Tumult Labs 2023\n\nThe Tumult Platform source code is licensed under the Apache License, version 2.0 (Apache-2.0).\nThe Tumult Platform documentation is licensed under\nCreative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.tmlt.dev/',
     'packages': packages,
     'package_data': package_data,
```

