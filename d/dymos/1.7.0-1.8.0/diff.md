# Comparing `tmp/dymos-1.7.0.tar.gz` & `tmp/dymos-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dymos-1.7.0.tar", last modified: Thu Feb  9 20:35:24 2023, max compression
+gzip compressed data, was "dymos-1.8.0.tar", last modified: Tue Apr 18 15:54:58 2023, max compression
```

## Comparing `dymos-1.7.0.tar` & `dymos-1.8.0.tar`

### file list

```diff
@@ -1,522 +1,525 @@
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.907888 dymos-1.7.0/
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10760 2021-07-01 16:42:29.000000 dymos-1.7.0/LICENSE
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1445 2023-02-09 20:35:24.907888 dymos-1.7.0/PKG-INFO
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.757888 dymos-1.7.0/dymos/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      363 2023-02-09 20:33:55.000000 dymos-1.7.0/dymos/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.757888 dymos-1.7.0/dymos/examples/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.767888 dymos-1.7.0/dymos/examples/aircraft_steady_flight/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.767888 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      970 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/aero_coef_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1662 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/aero_forces_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1288 2022-10-06 21:20:20.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/aerodynamics_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    42766 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/crm_data.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.767888 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/data/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      680 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/data/CRM_aero_inputs.dat
--rw-r--r--   0 swryan    (1000) swryan    (1000)    53416 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/data/CRM_aero_outputs.dat
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5242 2022-10-06 21:20:20.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/interpND_aero_coef_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.767888 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13557 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/test/test_aero_coef_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15403 2022-10-06 21:20:20.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/test/test_interpND_aero_coef_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2769 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/aircraft_ode.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1084 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/dynamic_pressure_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.777888 dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2553 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/lift_equilibrium_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2629 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/steady_flight_equilibrium_group.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.777888 dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2699 2022-10-06 21:20:20.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/test/test_flight_equilibrium_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2756 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/thrust_equilibrium_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1579 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/mass_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.777888 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1263 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/fuel_burn_rate_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1291 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/max_thrust_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2255 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/propulsion_group.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.777888 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1519 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/test/test_propulsion_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1235 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/throttle_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1521 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/thrust_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1254 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/tsfc_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1283 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/range_rate_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1306 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/steady_flight_path_angle_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.777888 dymos-1.7.0/dymos/examples/aircraft_steady_flight/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8917 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/test/test_aircraft_cruise.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2059 2022-10-06 21:20:20.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/test/test_aircraft_ode.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5053 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/test/test_ex_aircraft_steady_flight.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1041 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/aircraft_steady_flight/true_airspeed_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.777888 dymos-1.7.0/dymos/examples/balanced_field/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/balanced_field/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5737 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/examples/balanced_field/balanced_field_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.777888 dymos-1.7.0/dymos/examples/balanced_field/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/balanced_field/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15584 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/balanced_field/doc/test_doc_balanced_field_length.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.777888 dymos-1.7.0/dymos/examples/balanced_field/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/balanced_field/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15837 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/balanced_field/test/test_balanced_field_func_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    26837 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/balanced_field/test/test_balanced_field_length.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.777888 dymos-1.7.0/dymos/examples/battery_multibranch/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/battery_multibranch/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4635 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/battery_multibranch/batteries.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1751 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/battery_multibranch/battery_multibranch_ode.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2079 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/battery_multibranch/motors.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.787888 dymos-1.7.0/dymos/examples/battery_multibranch/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/battery_multibranch/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    16029 2021-08-05 15:28:04.000000 dymos-1.7.0/dymos/examples/battery_multibranch/test/test_multibranch_trajectory.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.787888 dymos-1.7.0/dymos/examples/brachistochrone/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      130 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/brachistochrone/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3495 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/examples/brachistochrone/brachistochrone_ode.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2644 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/examples/brachistochrone/brachistochrone_vector_states_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.787888 dymos-1.7.0/dymos/examples/brachistochrone/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/brachistochrone/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2691 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/examples/brachistochrone/doc/brachistochrone_ode.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13513 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6298 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_static_gravity.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5603 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_tandem_phases.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5661 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_upstream_control.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6338 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_upstream_state.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.797888 dymos-1.7.0/dymos/examples/brachistochrone/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4002 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/ex_brachistochrone.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3405 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/ex_brachistochrone_vector_states.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14007 2023-02-09 20:33:55.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_callable_ode_class.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    34881 2022-11-03 19:05:18.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_control_rate_targets.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5482 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_external_control.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2386 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_implicit_recorder.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10346 2021-08-05 15:28:04.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_integrated_control.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9452 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_integrated_parameter.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2299 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_path_constraint.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6389 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_quick_start.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5774 2021-08-05 15:28:04.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_simulate_options.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    19943 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_solve_segments.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10550 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_static_gravity.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13344 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_subprob_reports.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6576 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_timeseries_feedback.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6003 2021-08-05 15:28:04.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_varying_order_control_simulation.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9610 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_boundary_constraints.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    24656 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_path_constraints.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1225 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_states_ode.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    34394 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_doc_brachistochrone_polynomial_controls.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23787 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_duplicate_constraints.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4843 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_duplicate_timeseries_inputs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4290 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4209 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone_refine_grid.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3960 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone_vector_states.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11586 2022-05-05 14:58:21.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_path_constraints.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3878 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_simulate_units.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    40940 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_state_rate_introspection.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6189 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_static_outputs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6334 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_tandem_phases.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5265 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/brachistochrone/test/test_timeseries_units.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.797888 dymos-1.7.0/dymos/examples/cannonball/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/cannonball/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2428 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/cannonball/cannonball_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.797888 dymos-1.7.0/dymos/examples/cannonball/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/cannonball/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15241 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/cannonball/doc/test_doc_two_phase_cannonball.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1607 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/cannonball/size_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.807888 dymos-1.7.0/dymos/examples/cannonball/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/cannonball/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5342 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/cannonball/test/test_cannonball_expr_constraint.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15757 2022-05-05 14:58:21.000000 dymos-1.7.0/dymos/examples/cannonball/test/test_cannonball_matrix_state.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8833 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/cannonball/test/test_connect_control_to_parameter.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8042 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/cannonball/test/test_load_case_missing_phase.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    32815 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/cannonball/test/test_phase_linkage_compliance.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22154 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/cannonball/test/test_two_phase_cannonball_ode_output_linkage.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.807888 dymos-1.7.0/dymos/examples/cart_pole/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/examples/cart_pole/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2438 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/examples/cart_pole/animate_cartpole.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6012 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/examples/cart_pole/cartpole_dynamics.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.807888 dymos-1.7.0/dymos/examples/double_integrator/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/double_integrator/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.807888 dymos-1.7.0/dymos/examples/double_integrator/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/double_integrator/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3737 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/double_integrator/doc/test_doc_double_integrator.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      726 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/double_integrator/double_integrator_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.807888 dymos-1.7.0/dymos/examples/double_integrator/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/double_integrator/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8818 2021-08-05 15:28:04.000000 dymos-1.7.0/dymos/examples/double_integrator/test/test_double_integrator.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4206 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/examples/double_integrator/test/test_double_integrator_timeseries_units.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.807888 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.807888 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11488 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/doc/test_doc_finite_burn_orbit_raise.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6486 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/finite_burn_eom.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14061 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/finite_burn_orbit_raise_problem.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.807888 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1868 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10890 2022-10-06 21:20:20.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise_bokeh_plots.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1646 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise_mpi.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2523 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_finite_burn_eom.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6301 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_multi_phase_restart.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    52681 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_two_burn_orbit_raise_linkages.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.807888 dymos-1.7.0/dymos/examples/flying_robot/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/flying_robot/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      899 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/flying_robot/flying_robot_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.807888 dymos-1.7.0/dymos/examples/flying_robot/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/flying_robot/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3659 2021-08-05 15:28:04.000000 dymos-1.7.0/dymos/examples/flying_robot/test/test_flying_robot.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.817888 dymos-1.7.0/dymos/examples/hull_problem/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/hull_problem/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      762 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/hull_problem/hull_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.817888 dymos-1.7.0/dymos/examples/hull_problem/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/hull_problem/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3455 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/hull_problem/test/test_hull_problem.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.817888 dymos-1.7.0/dymos/examples/hyper_sensitive/
--rw-r--r--   0 swryan    (1000) swryan    (1000)       51 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/hyper_sensitive/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.817888 dymos-1.7.0/dymos/examples/hyper_sensitive/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/hyper_sensitive/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4010 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/hyper_sensitive/doc/test_doc_hyper_sensitive.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1334 2022-03-04 14:52:23.000000 dymos-1.7.0/dymos/examples/hyper_sensitive/hyper_sensitive_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.817888 dymos-1.7.0/dymos/examples/hyper_sensitive/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/hyper_sensitive/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5570 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/hyper_sensitive/test/test_hyper_sensitive.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.817888 dymos-1.7.0/dymos/examples/length_constrained_brachistochrone/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/length_constrained_brachistochrone/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1049 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/length_constrained_brachistochrone/arc_length_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.817888 dymos-1.7.0/dymos/examples/length_constrained_brachistochrone/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/length_constrained_brachistochrone/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4761 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/length_constrained_brachistochrone/doc/test_doc_length_constrained_brachistochrone.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.817888 dymos-1.7.0/dymos/examples/min_time_climb/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.817888 dymos-1.7.0/dymos/examples/min_time_climb/aero/
--rw-r--r--   0 swryan    (1000) swryan    (1000)       28 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2744 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/aero.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1310 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/cd0_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1445 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/cd_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      950 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/cl_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1405 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/cla_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      934 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/dynamic_pressure_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1431 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/kappa_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2114 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/lift_drag_force_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1076 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/mach_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.817888 dymos-1.7.0/dymos/examples/min_time_climb/aero/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2514 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/test/test_aerodynamics.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1729 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/test/test_cd0_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1739 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/test/test_cla_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1467 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/aero/test/test_kappa_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.827888 dymos-1.7.0/dymos/examples/min_time_climb/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3357 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/doc/aero_partial_coloring.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1041 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/min_time_climb/doc/dynamic_pressure_comp_partial_coloring.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1786 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/doc/min_time_climb_ode_partial_coloring.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1451 2022-04-08 21:48:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/min_time_climb_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.827888 dymos-1.7.0/dymos/examples/min_time_climb/prop/
--rw-r--r--   0 swryan    (1000) swryan    (1000)       68 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/prop/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3621 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/min_time_climb/prop/max_thrust_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1243 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/prop/mdot_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1742 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/prop/prop.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.827888 dymos-1.7.0/dymos/examples/min_time_climb/prop/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/prop/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1164 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/prop/test/test_max_thrust_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1174 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/prop/thrust_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.827888 dymos-1.7.0/dymos/examples/min_time_climb/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/min_time_climb/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4530 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/min_time_climb/test/test_doc_min_time_climb_partial_coloring.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12359 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/min_time_climb/test/test_ex_min_time_climb.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4311 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/examples/min_time_climb/test/test_min_time_climb_simulate_failure.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7241 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/min_time_climb/test/test_refine_with_shaped_parameter.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.827888 dymos-1.7.0/dymos/examples/oscillator/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/oscillator/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1224 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/oscillator/oscillator_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.827888 dymos-1.7.0/dymos/examples/oscillator/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/oscillator/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    19004 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/oscillator/test/test_oscillator.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1612 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/plotting.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/racecar/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1000 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/racecar/Track.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3523 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/accelerationODE.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12989 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/carODE.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2984 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/combinedODE.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1216 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/curvature.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1096 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/linewidthhelper.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5039 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/normalForceODE.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4208 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/spline.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/racecar/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/racecar/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    16980 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/racecar/test/test_racecar.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1056 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/timeAdder.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4684 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/timeODE.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8124 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/tireConstraintODE.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7944 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/tireODE.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9063 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/racecar/tracks.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/robertson_problem/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/robertson_problem/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/robertson_problem/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/robertson_problem/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1722 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/robertson_problem/doc/robertson_ode.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3609 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/examples/robertson_problem/doc/test_doc_robertson_problem.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/robot_arm/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/robot_arm/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/robot_arm/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/robot_arm/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4709 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/robot_arm/doc/test_doc_robot_arm.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4233 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/robot_arm/robot_arm_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/robot_arm/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/robot_arm/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7070 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/robot_arm/test/test_robot_arm.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/shuttle_reentry/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/shuttle_reentry/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2710 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/shuttle_reentry/aerodynamics_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1127 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/shuttle_reentry/atmosphere_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/shuttle_reentry/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/shuttle_reentry/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5354 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/shuttle_reentry/doc/test_doc_reentry.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7705 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/shuttle_reentry/flight_dynamics_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2364 2022-10-06 21:20:20.000000 dymos-1.7.0/dymos/examples/shuttle_reentry/heating_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1628 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/shuttle_reentry/shuttle_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/shuttle_reentry/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/shuttle_reentry/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12041 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/shuttle_reentry/test/test_reentry.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/ssto/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/ssto/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/ssto/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/ssto/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5060 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/ssto/doc/test_doc_ssto_earth.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12049 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/ssto/doc/test_doc_ssto_linear_tangent_guidance.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12406 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/ssto/doc/test_doc_ssto_polynomial_control.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3987 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/ssto/launch_vehicle_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.837888 dymos-1.7.0/dymos/examples/ssto/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/ssto/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12525 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/ssto/test/test_simulate_root_trajectory.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/examples/vanderpol/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/vanderpol/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/examples/vanderpol/doc/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/vanderpol/doc/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5493 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/vanderpol/doc/test_doc_vanderpol.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/examples/vanderpol/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/vanderpol/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3665 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/examples/vanderpol/test/test_vanderpol.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3936 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/examples/vanderpol/vanderpol_dymos.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3876 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/examples/vanderpol/vanderpol_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/examples/water_rocket/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/water_rocket/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10549 2022-03-04 14:52:23.000000 dymos-1.7.0/dymos/examples/water_rocket/phases.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/examples/water_rocket/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/examples/water_rocket/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11001 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/examples/water_rocket/test/test_water_rocket.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6402 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/water_rocket/water_engine_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3020 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/examples/water_rocket/water_propulsion_ode.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/grid_refinement/
--rwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/grid_refinement/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    17995 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/grid_refinement/error_estimation.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9692 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/grid_refinement/grid_refinement_ode_system.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/grid_refinement/hp_adaptive/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/grid_refinement/hp_adaptive/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    27515 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/grid_refinement/hp_adaptive/hp_adaptive.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/grid_refinement/ph_adaptive/
--rwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/grid_refinement/ph_adaptive/__init__.py
--rwxr-xr-x   0 swryan    (1000) swryan    (1000)     4793 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/grid_refinement/ph_adaptive/ph_adaptive.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3165 2022-07-15 18:00:33.000000 dymos-1.7.0/dymos/grid_refinement/refinement.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3728 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/grid_refinement/write_iteration.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10395 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/load_case.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/models/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/models/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/models/atmosphere/
--rw-r--r--   0 swryan    (1000) swryan    (1000)       38 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/models/atmosphere/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)   159829 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/models/atmosphere/atmos_1976.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/models/atmosphere/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/models/atmosphere/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4116 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/models/atmosphere/test/test_atmos.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/models/eom/
--rw-r--r--   0 swryan    (1000) swryan    (1000)       48 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/models/eom/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6105 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/models/eom/flight_path_eom_2d.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.847888 dymos-1.7.0/dymos/models/eom/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/models/eom/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5197 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/models/eom/test/test_flight_path_eom_2d.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      680 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/options.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.857888 dymos-1.7.0/dymos/phase/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      113 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/phase/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23887 2022-10-17 17:59:13.000000 dymos-1.7.0/dymos/phase/analytic_phase.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    38142 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/phase/options.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)   125026 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/phase/phase.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18082 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/phase/simulation_phase.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.857888 dymos-1.7.0/dymos/phase/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/phase/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9475 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/phase/test/test_add_boundary_constraint.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2449 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/phase/test/test_add_parameter_types.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7059 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/phase/test/test_add_path_constraint.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    24998 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/phase/test/test_analytic_phase.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4482 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/phase/test/test_input_parameter_connections.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6078 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/phase/test/test_interp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    29516 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/phase/test/test_phase.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9904 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/phase/test/test_set_time_options.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3106 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/phase/test/test_simulate.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10163 2022-03-31 18:16:47.000000 dymos-1.7.0/dymos/phase/test/test_sized_input_parameters.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8845 2022-10-17 17:59:13.000000 dymos-1.7.0/dymos/phase/test/test_state_discovery.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    17325 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/phase/test/test_time_targets.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2356 2022-11-14 17:54:57.000000 dymos-1.7.0/dymos/phase/test/test_time_units.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    31923 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/phase/test/test_timeseries.py
--rwxr-xr-x   0 swryan    (1000) swryan    (1000)     5728 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/run_problem.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.857888 dymos-1.7.0/dymos/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    20271 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/test/test_check_partials.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6021 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/test/test_lint_docstrings.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10035 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/test/test_load_case.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1990 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/test/test_options.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2472 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/test/test_pycodestyle.py
--rwxr-xr-x   0 swryan    (1000) swryan    (1000)    38198 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/test/test_run_problem.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    34041 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/test/test_upgrade_guide.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.857888 dymos-1.7.0/dymos/trajectory/
--rw-r--r--   0 swryan    (1000) swryan    (1000)       35 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/trajectory/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4739 2023-01-25 18:06:21.000000 dymos-1.7.0/dymos/trajectory/options.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5252 2023-01-25 18:06:21.000000 dymos-1.7.0/dymos/trajectory/phase_linkage_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.867888 dymos-1.7.0/dymos/trajectory/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/trajectory/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4466 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/trajectory/test/test_phase_linkage_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18090 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/trajectory/test/test_t_initial_bounds.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    94867 2023-01-25 18:06:21.000000 dymos-1.7.0/dymos/trajectory/test/test_trajectory.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    30896 2023-01-25 18:06:21.000000 dymos-1.7.0/dymos/trajectory/test/test_trajectory_parameters.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    65043 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/trajectory/trajectory.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.867888 dymos-1.7.0/dymos/transcriptions/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      240 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/transcriptions/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.867888 dymos-1.7.0/dymos/transcriptions/analytic/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-10-17 17:59:13.000000 dymos-1.7.0/dymos/transcriptions/analytic/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18867 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/analytic/analytic.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8095 2022-10-17 17:59:13.000000 dymos-1.7.0/dymos/transcriptions/analytic/analytic_timeseries_output_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.867888 dymos-1.7.0/dymos/transcriptions/common/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      306 2022-11-03 19:05:18.000000 dymos-1.7.0/dymos/transcriptions/common/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    17726 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/transcriptions/common/continuity_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    16596 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/transcriptions/common/control_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8174 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/common/parameter_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13034 2023-01-25 18:06:21.000000 dymos-1.7.0/dymos/transcriptions/common/polynomial_control_group.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.867888 dymos-1.7.0/dymos/transcriptions/common/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/transcriptions/common/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8568 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/transcriptions/common/test/test_continuity_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    19491 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/common/test/test_control_interp_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23740 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/common/test/test_polynomial_control_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4901 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/common/test/test_time_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3556 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/common/time_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1280 2022-11-03 19:05:18.000000 dymos-1.7.0/dymos/transcriptions/common/timeseries_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2692 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/common/timeseries_output_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.867888 dymos-1.7.0/dymos/transcriptions/explicit_shooting/
--rw-r--r--   0 swryan    (1000) swryan    (1000)       48 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    42938 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/explicit_shooting.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10973 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/explicit_shooting_continuity_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5146 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/explicit_shooting_timeseries_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18359 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/ode_evaluation_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    40007 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/ode_integration_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2899 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/state_rate_collector_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5184 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/tau_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.877888 dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    20433 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/test_control_interpolation_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    29765 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/test_explicit_shooting.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2589 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/test_ode_evaluation_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11800 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/test_ode_integration_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1919 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/test_tau_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18137 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/transcriptions/explicit_shooting/vandermonde_control_interp_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    26433 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/transcriptions/grid_data.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.877888 dymos-1.7.0/dymos/transcriptions/pseudospectral/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.877888 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      371 2022-01-05 13:33:54.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6696 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/collocation_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4583 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/control_endpoint_defect_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6435 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/gauss_lobatto_interleave_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8130 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/pseudospectral_timeseries_output_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8911 2022-10-17 17:59:13.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/state_independents.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12474 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/state_interp_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.877888 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3852 2022-10-17 17:59:13.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_opt.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9542 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_sol_opt.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15775 2021-07-01 17:27:39.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_solver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2606 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_control_endpoint_defect_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4290 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_gauss_lobatto_interleave_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15790 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_state_interp_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    31127 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/gauss_lobatto.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    29478 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/pseudospectral_base.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22395 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/radau_pseudospectral.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.877888 dymos-1.7.0/dymos/transcriptions/pseudospectral/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4707 2022-11-03 19:05:18.000000 dymos-1.7.0/dymos/transcriptions/pseudospectral/test/test_ps_base.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.877888 dymos-1.7.0/dymos/transcriptions/solve_ivp/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.887888 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      602 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6994 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/ode_integration_interface.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10634 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/ode_integration_interface_system.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4638 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/odeint_control_interpolation_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13275 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/segment_simulation_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2332 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/segment_state_mux_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10918 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/solve_ivp_control_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13119 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/solve_ivp_polynomial_control_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7222 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/solve_ivp_timeseries_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1927 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/state_rate_collector_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.887888 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2789 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/components/test/test_segment_simulation_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    28240 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/transcriptions/solve_ivp/solve_ivp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    30235 2023-01-25 18:06:27.000000 dymos-1.7.0/dymos/transcriptions/transcription_base.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.897888 dymos-1.7.0/dymos/utils/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/utils/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      407 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/utils/constants.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4198 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/utils/hermite.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3791 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/utils/indexing.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7821 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/utils/interpolate.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    58970 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/utils/introspection.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1815 2022-10-17 17:59:13.000000 dymos-1.7.0/dymos/utils/lagrange.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2931 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/utils/lg.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3409 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/utils/lgl.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4061 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/utils/lgr.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6123 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/utils/misc.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.897888 dymos-1.7.0/dymos/utils/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/utils/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2225 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/utils/test/test_hermite.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1305 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/utils/test/test_indexing.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1524 2022-03-04 14:52:23.000000 dymos-1.7.0/dymos/utils/test/test_introspection.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1256 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/utils/test/test_lg.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1686 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/utils/test/test_lgl.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1966 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/utils/test/test_lgr.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      632 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/utils/test/test_misc.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23115 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/utils/test/test_testing_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    17867 2022-09-16 16:16:20.000000 dymos-1.7.0/dymos/utils/testing_utils.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.897888 dymos-1.7.0/dymos/visualization/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.7.0/dymos/visualization/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.897888 dymos-1.7.0/dymos/visualization/linkage/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-08-08 20:47:06.000000 dymos-1.7.0/dymos/visualization/linkage/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.897888 dymos-1.7.0/dymos/visualization/linkage/js/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2445 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageCellRenderer.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1438 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageDiagram.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2802 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageLegend.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14276 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageMatrix.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3069 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageMatrixCell.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)      898 2022-08-08 20:47:06.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageModelData.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3472 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageStyle.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1371 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageSymbolType.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5196 2023-01-03 17:56:55.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageTreeNode.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)      723 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageUserInterface.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)      605 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/visualization/linkage/js/DmLinkage_main.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13064 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/visualization/linkage/report.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14463 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/visualization/linkage/report_template.html
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.907888 dymos-1.7.0/dymos/visualization/linkage/style/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1905 2022-08-05 15:09:01.000000 dymos-1.7.0/dymos/visualization/linkage/style/linkage_report.css
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.907888 dymos-1.7.0/dymos/visualization/linkage/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-08-08 20:47:06.000000 dymos-1.7.0/dymos/visualization/linkage/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    30639 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/visualization/linkage/test/linkage_report_ui_test.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      245 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/visualization/linkage/test/test_gui.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.907888 dymos-1.7.0/dymos/visualization/test/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-08-08 20:47:06.000000 dymos-1.7.0/dymos/visualization/test/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    25863 2023-01-09 19:10:23.000000 dymos-1.7.0/dymos/visualization/test/test_timeseries_plots.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18287 2023-02-07 21:41:37.000000 dymos-1.7.0/dymos/visualization/timeseries_plots.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-02-09 20:35:24.757888 dymos-1.7.0/dymos.egg-info/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1445 2023-02-09 20:35:24.000000 dymos-1.7.0/dymos.egg-info/PKG-INFO
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22022 2023-02-09 20:35:24.000000 dymos-1.7.0/dymos.egg-info/SOURCES.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)        1 2023-02-09 20:35:24.000000 dymos-1.7.0/dymos.egg-info/dependency_links.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)       94 2023-02-09 20:35:24.000000 dymos-1.7.0/dymos.egg-info/entry_points.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)        1 2023-02-09 20:35:24.000000 dymos-1.7.0/dymos.egg-info/not-zip-safe
--rw-r--r--   0 swryan    (1000) swryan    (1000)      432 2023-02-09 20:35:24.000000 dymos-1.7.0/dymos.egg-info/requires.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)        6 2023-02-09 20:35:24.000000 dymos-1.7.0/dymos.egg-info/top_level.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)       38 2023-02-09 20:35:24.907888 dymos-1.7.0/setup.cfg
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2769 2023-02-09 20:33:55.000000 dymos-1.7.0/setup.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.253609 dymos-1.8.0/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10760 2021-07-01 16:42:29.000000 dymos-1.8.0/LICENSE
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1445 2023-04-18 15:54:58.253609 dymos-1.8.0/PKG-INFO
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      364 2023-04-18 15:53:33.000000 dymos-1.8.0/dymos/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      893 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/_options.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/aircraft_steady_flight/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      970 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/aero_coef_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1662 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/aero_forces_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1288 2022-10-06 21:20:20.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/aerodynamics_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    42766 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/crm_data.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/data/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      680 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/data/CRM_aero_inputs.dat
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    53416 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/data/CRM_aero_outputs.dat
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5242 2022-10-06 21:20:20.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/interpND_aero_coef_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13557 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/test/test_aero_coef_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15403 2022-10-06 21:20:20.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/test/test_interpND_aero_coef_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2769 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/aircraft_ode.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1084 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/dynamic_pressure_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2553 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/lift_equilibrium_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2629 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/steady_flight_equilibrium_group.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2699 2022-10-06 21:20:20.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/test/test_flight_equilibrium_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2756 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/thrust_equilibrium_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1579 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/mass_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1263 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/fuel_burn_rate_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1291 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/max_thrust_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2255 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/propulsion_group.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1519 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/test/test_propulsion_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1235 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/throttle_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1521 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/thrust_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1254 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/tsfc_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1283 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/range_rate_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1306 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/steady_flight_path_angle_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/aircraft_steady_flight/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8917 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/test/test_aircraft_cruise.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2059 2022-10-06 21:20:20.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/test/test_aircraft_ode.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5053 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/test/test_ex_aircraft_steady_flight.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1041 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/aircraft_steady_flight/true_airspeed_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos/examples/balanced_field/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/balanced_field/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5737 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/examples/balanced_field/balanced_field_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/balanced_field/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/balanced_field/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13662 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/balanced_field/doc/test_doc_balanced_field_length.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/balanced_field/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/balanced_field/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15837 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/examples/balanced_field/test/test_balanced_field_func_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    27597 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/balanced_field/test/test_balanced_field_length.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/battery_multibranch/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/battery_multibranch/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4635 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/battery_multibranch/batteries.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1751 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/battery_multibranch/battery_multibranch_ode.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2079 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/battery_multibranch/motors.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/battery_multibranch/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/battery_multibranch/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    16029 2021-08-05 15:28:04.000000 dymos-1.8.0/dymos/examples/battery_multibranch/test/test_multibranch_trajectory.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/brachistochrone/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      130 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/brachistochrone/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3495 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/examples/brachistochrone/brachistochrone_ode.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2644 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/examples/brachistochrone/brachistochrone_vector_states_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/brachistochrone/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/brachistochrone/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2691 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/examples/brachistochrone/doc/brachistochrone_ode.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13513 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6298 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_static_gravity.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5603 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_tandem_phases.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5661 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_upstream_control.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6338 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_upstream_state.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/brachistochrone/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4212 2023-03-30 13:48:25.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/ex_brachistochrone.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3405 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/ex_brachistochrone_vector_states.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13993 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_callable_ode_class.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    33657 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_control_rate_targets.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5482 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_external_control.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2386 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_implicit_recorder.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10346 2021-08-05 15:28:04.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_integrated_control.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9452 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_integrated_parameter.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2299 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_path_constraint.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6389 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_quick_start.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5774 2021-08-05 15:28:04.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_simulate_options.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    19943 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_solve_segments.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10550 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_static_gravity.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13368 2023-03-30 13:48:25.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_subprob_reports.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6576 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_timeseries_feedback.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5989 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_varying_order_control_simulation.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9610 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_boundary_constraints.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    24656 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_path_constraints.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1225 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_states_ode.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    34394 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_doc_brachistochrone_polynomial_controls.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23787 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_duplicate_constraints.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4843 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_duplicate_timeseries_inputs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4283 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4202 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone_refine_grid.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3953 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone_vector_states.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12529 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_path_constraints.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3864 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_simulate_units.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    40940 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_state_rate_introspection.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6189 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_static_outputs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6334 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_tandem_phases.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5354 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/brachistochrone/test/test_timeseries_units.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/cannonball/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/cannonball/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2428 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/cannonball/cannonball_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/cannonball/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/cannonball/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14402 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/cannonball/doc/test_doc_two_phase_cannonball.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1607 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/cannonball/size_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/cannonball/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/cannonball/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5342 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/examples/cannonball/test/test_cannonball_expr_constraint.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15757 2022-05-05 14:58:21.000000 dymos-1.8.0/dymos/examples/cannonball/test/test_cannonball_matrix_state.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8826 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/cannonball/test/test_connect_control_to_parameter.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8042 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/cannonball/test/test_load_case_missing_phase.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    32815 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/cannonball/test/test_phase_linkage_compliance.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    19035 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/cannonball/test/test_two_phase_cannonball_ode_output_linkage.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/cart_pole/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/examples/cart_pole/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2438 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/examples/cart_pole/animate_cartpole.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6012 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/examples/cart_pole/cartpole_dynamics.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/double_integrator/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/double_integrator/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/double_integrator/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/double_integrator/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3737 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/double_integrator/doc/test_doc_double_integrator.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      726 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/double_integrator/double_integrator_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/double_integrator/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/double_integrator/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8818 2021-08-05 15:28:04.000000 dymos-1.8.0/dymos/examples/double_integrator/test/test_double_integrator.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4266 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/double_integrator/test/test_double_integrator_timeseries_units.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.213609 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11488 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/doc/test_doc_finite_burn_orbit_raise.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6486 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/finite_burn_eom.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14061 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/finite_burn_orbit_raise_problem.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1868 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10509 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise_bokeh_plots.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1646 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise_mpi.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2523 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_finite_burn_eom.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6301 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_multi_phase_restart.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    58278 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_two_burn_orbit_raise_linkages.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/flying_robot/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/flying_robot/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      899 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/flying_robot/flying_robot_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/flying_robot/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/flying_robot/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3659 2021-08-05 15:28:04.000000 dymos-1.8.0/dymos/examples/flying_robot/test/test_flying_robot.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/hull_problem/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/examples/hull_problem/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      762 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/examples/hull_problem/hull_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/hull_problem/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/examples/hull_problem/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3640 2023-03-30 13:48:25.000000 dymos-1.8.0/dymos/examples/hull_problem/test/test_hull_problem.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/hyper_sensitive/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       51 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/hyper_sensitive/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/hyper_sensitive/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/hyper_sensitive/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4010 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/hyper_sensitive/doc/test_doc_hyper_sensitive.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1334 2022-03-04 14:52:23.000000 dymos-1.8.0/dymos/examples/hyper_sensitive/hyper_sensitive_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/hyper_sensitive/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/hyper_sensitive/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5570 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/examples/hyper_sensitive/test/test_hyper_sensitive.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/length_constrained_brachistochrone/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/length_constrained_brachistochrone/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1049 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/length_constrained_brachistochrone/arc_length_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/length_constrained_brachistochrone/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/length_constrained_brachistochrone/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4761 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/length_constrained_brachistochrone/doc/test_doc_length_constrained_brachistochrone.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/min_time_climb/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/min_time_climb/aero/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       28 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2744 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/aero.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1310 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/cd0_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1445 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/cd_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      950 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/cl_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1405 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/cla_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      934 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/dynamic_pressure_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1431 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/kappa_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2114 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/lift_drag_force_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1076 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/mach_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/min_time_climb/aero/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2514 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/test/test_aerodynamics.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1729 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/test/test_cd0_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1739 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/test/test_cla_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1467 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/aero/test/test_kappa_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/min_time_climb/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3357 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/doc/aero_partial_coloring.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1041 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/examples/min_time_climb/doc/dynamic_pressure_comp_partial_coloring.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1786 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/doc/min_time_climb_ode_partial_coloring.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1451 2022-04-08 21:48:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/min_time_climb_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/min_time_climb/prop/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       68 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/prop/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3621 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/min_time_climb/prop/max_thrust_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1243 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/prop/mdot_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1742 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/prop/prop.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/min_time_climb/prop/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/prop/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1164 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/prop/test/test_max_thrust_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1174 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/prop/thrust_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/min_time_climb/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/min_time_climb/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4530 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/min_time_climb/test/test_doc_min_time_climb_partial_coloring.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12359 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/min_time_climb/test/test_ex_min_time_climb.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4311 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/examples/min_time_climb/test/test_min_time_climb_simulate_failure.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7241 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/min_time_climb/test/test_refine_with_shaped_parameter.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/oscillator/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/oscillator/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1224 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/examples/oscillator/oscillator_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/oscillator/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/examples/oscillator/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    19004 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/examples/oscillator/test/test_oscillator.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1612 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/plotting.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/racecar/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1000 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/racecar/Track.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3523 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/accelerationODE.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12989 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/carODE.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2984 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/combinedODE.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1216 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/curvature.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1096 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/linewidthhelper.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5039 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/normalForceODE.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4208 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/spline.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/racecar/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/examples/racecar/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    16980 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/examples/racecar/test/test_racecar.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1056 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/timeAdder.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4684 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/timeODE.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8124 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/tireConstraintODE.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7944 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/tireODE.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9063 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/racecar/tracks.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/robertson_problem/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/robertson_problem/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/robertson_problem/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/robertson_problem/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1722 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/robertson_problem/doc/robertson_ode.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3631 2023-03-30 13:48:25.000000 dymos-1.8.0/dymos/examples/robertson_problem/doc/test_doc_robertson_problem.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/robot_arm/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/robot_arm/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/robot_arm/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/robot_arm/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4709 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/examples/robot_arm/doc/test_doc_robot_arm.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4233 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/robot_arm/robot_arm_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.223609 dymos-1.8.0/dymos/examples/robot_arm/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/robot_arm/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7070 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/examples/robot_arm/test/test_robot_arm.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/shuttle_reentry/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/shuttle_reentry/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2710 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/shuttle_reentry/aerodynamics_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1127 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/shuttle_reentry/atmosphere_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/shuttle_reentry/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/shuttle_reentry/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5354 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/shuttle_reentry/doc/test_doc_reentry.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7705 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/shuttle_reentry/flight_dynamics_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2364 2022-10-06 21:20:20.000000 dymos-1.8.0/dymos/examples/shuttle_reentry/heating_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1628 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/shuttle_reentry/shuttle_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/shuttle_reentry/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/shuttle_reentry/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12041 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/examples/shuttle_reentry/test/test_reentry.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/ssto/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/ssto/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/ssto/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/ssto/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5060 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/ssto/doc/test_doc_ssto_earth.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12049 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/ssto/doc/test_doc_ssto_linear_tangent_guidance.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12406 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/ssto/doc/test_doc_ssto_polynomial_control.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3987 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/ssto/launch_vehicle_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/ssto/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/ssto/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12525 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/ssto/test/test_simulate_root_trajectory.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/vanderpol/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/vanderpol/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/vanderpol/doc/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/vanderpol/doc/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5493 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/vanderpol/doc/test_doc_vanderpol.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/vanderpol/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/vanderpol/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3665 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/examples/vanderpol/test/test_vanderpol.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3936 2023-04-17 17:05:57.000000 dymos-1.8.0/dymos/examples/vanderpol/vanderpol_dymos.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3876 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/examples/vanderpol/vanderpol_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/water_rocket/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/water_rocket/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10549 2022-03-04 14:52:23.000000 dymos-1.8.0/dymos/examples/water_rocket/phases.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/examples/water_rocket/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/examples/water_rocket/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11001 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/examples/water_rocket/test/test_water_rocket.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6402 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/water_rocket/water_engine_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3020 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/examples/water_rocket/water_propulsion_ode.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/grid_refinement/
+-rwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/grid_refinement/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    17944 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/grid_refinement/error_estimation.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9692 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/grid_refinement/grid_refinement_ode_system.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/grid_refinement/hp_adaptive/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/grid_refinement/hp_adaptive/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    27515 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/grid_refinement/hp_adaptive/hp_adaptive.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/grid_refinement/ph_adaptive/
+-rwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/grid_refinement/ph_adaptive/__init__.py
+-rwxr-xr-x   0 swryan    (1000) swryan    (1000)     4793 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/grid_refinement/ph_adaptive/ph_adaptive.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3165 2023-04-18 15:52:32.000000 dymos-1.8.0/dymos/grid_refinement/refinement.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3728 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/grid_refinement/write_iteration.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10467 2023-04-10 20:00:04.000000 dymos-1.8.0/dymos/load_case.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/models/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/models/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/models/atmosphere/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       38 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/models/atmosphere/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   159829 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/models/atmosphere/atmos_1976.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/models/atmosphere/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/models/atmosphere/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4116 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/models/atmosphere/test/test_atmos.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/models/eom/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       48 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/models/eom/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6105 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/models/eom/flight_path_eom_2d.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/models/eom/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/models/eom/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5197 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/models/eom/test/test_flight_path_eom_2d.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/phase/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      113 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/phase/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23887 2022-10-17 17:59:13.000000 dymos-1.8.0/dymos/phase/analytic_phase.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    39016 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/phase/options.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   125193 2023-04-18 15:52:32.000000 dymos-1.8.0/dymos/phase/phase.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18228 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/phase/simulation_phase.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/phase/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/phase/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9475 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/phase/test/test_add_boundary_constraint.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2449 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/phase/test/test_add_parameter_types.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7059 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/phase/test/test_add_path_constraint.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    24991 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/phase/test/test_analytic_phase.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4482 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/phase/test/test_input_parameter_connections.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6078 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/phase/test/test_interp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    30206 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/phase/test/test_phase.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9904 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/phase/test/test_set_time_options.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3106 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/phase/test/test_simulate.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10163 2022-03-31 18:16:47.000000 dymos-1.8.0/dymos/phase/test/test_sized_input_parameters.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8845 2022-10-17 17:59:13.000000 dymos-1.8.0/dymos/phase/test/test_state_discovery.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    17570 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/phase/test/test_time_targets.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2356 2022-11-14 17:54:57.000000 dymos-1.8.0/dymos/phase/test/test_time_units.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    32019 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/phase/test/test_timeseries.py
+-rwxr-xr-x   0 swryan    (1000) swryan    (1000)     6387 2023-04-18 15:52:32.000000 dymos-1.8.0/dymos/run_problem.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    20295 2023-03-30 13:48:25.000000 dymos-1.8.0/dymos/test/test_check_partials.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6021 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/test/test_lint_docstrings.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10031 2023-04-18 15:52:32.000000 dymos-1.8.0/dymos/test/test_load_case.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1990 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/test/test_options.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2472 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/test/test_pycodestyle.py
+-rwxr-xr-x   0 swryan    (1000) swryan    (1000)    38786 2023-04-18 15:52:14.000000 dymos-1.8.0/dymos/test/test_run_problem.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    33952 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/test/test_upgrade_guide.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/trajectory/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       35 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/trajectory/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4739 2023-01-25 18:06:21.000000 dymos-1.8.0/dymos/trajectory/options.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5253 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/trajectory/phase_linkage_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.233609 dymos-1.8.0/dymos/trajectory/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/trajectory/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4466 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/trajectory/test/test_phase_linkage_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18090 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/trajectory/test/test_t_initial_bounds.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    94961 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/trajectory/test/test_trajectory.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    31537 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/trajectory/test/test_trajectory_parameters.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    65977 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/trajectory/trajectory.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      240 2023-01-25 18:06:27.000000 dymos-1.8.0/dymos/transcriptions/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/analytic/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-10-17 17:59:13.000000 dymos-1.8.0/dymos/transcriptions/analytic/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18867 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/analytic/analytic.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8095 2022-10-17 17:59:13.000000 dymos-1.8.0/dymos/transcriptions/analytic/analytic_timeseries_output_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/common/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      306 2022-11-03 19:05:18.000000 dymos-1.8.0/dymos/transcriptions/common/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    17727 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/common/continuity_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    16597 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/common/control_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7446 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/common/parameter_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13035 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/common/polynomial_control_group.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/common/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/transcriptions/common/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8568 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/transcriptions/common/test/test_continuity_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    19491 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/common/test/test_control_interp_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23740 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/common/test/test_polynomial_control_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4901 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/common/test/test_time_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3557 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/common/time_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1280 2022-11-03 19:05:18.000000 dymos-1.8.0/dymos/transcriptions/common/timeseries_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2693 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/common/timeseries_output_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/explicit_shooting/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       48 2023-01-25 18:06:27.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    43905 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/explicit_shooting.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10973 2023-01-25 18:06:27.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/explicit_shooting_continuity_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5147 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/explicit_shooting_timeseries_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18359 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/ode_evaluation_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    40008 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/ode_integration_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2897 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/state_rate_collector_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5185 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/tau_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    20433 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/test_control_interpolation_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    29914 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/test_explicit_shooting.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2589 2023-01-25 18:06:27.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/test_ode_evaluation_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11805 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/test_ode_integration_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1919 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/test_tau_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18137 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/transcriptions/explicit_shooting/vandermonde_control_interp_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    26433 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/transcriptions/grid_data.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/pseudospectral/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      371 2022-01-05 13:33:54.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6697 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/collocation_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4584 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/control_endpoint_defect_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6436 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/gauss_lobatto_interleave_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8130 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/pseudospectral_timeseries_output_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8912 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/state_independents.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12475 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/state_interp_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3852 2022-10-17 17:59:13.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_opt.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9542 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_sol_opt.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15775 2021-07-01 17:27:39.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_solver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2605 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_control_endpoint_defect_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4290 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_gauss_lobatto_interleave_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15790 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_state_interp_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    31127 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/gauss_lobatto.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    29478 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/pseudospectral_base.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22395 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/radau_pseudospectral.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/pseudospectral/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4707 2022-11-03 19:05:18.000000 dymos-1.8.0/dymos/transcriptions/pseudospectral/test/test_ps_base.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/solve_ivp/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      602 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6994 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/ode_integration_interface.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10634 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/ode_integration_interface_system.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4638 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/odeint_control_interpolation_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13275 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/segment_simulation_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2332 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/segment_state_mux_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10980 2023-03-14 20:49:24.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/solve_ivp_control_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13119 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/solve_ivp_polynomial_control_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7222 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/solve_ivp_timeseries_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1928 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/state_rate_collector_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2789 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/components/test/test_segment_simulation_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    28240 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/transcriptions/solve_ivp/solve_ivp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    31611 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/transcriptions/transcription_base.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.243609 dymos-1.8.0/dymos/utils/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/utils/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      407 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/utils/constants.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4198 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/utils/hermite.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3791 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/utils/indexing.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7821 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/utils/interpolate.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    58957 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/utils/introspection.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1815 2022-10-17 17:59:13.000000 dymos-1.8.0/dymos/utils/lagrange.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2931 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/utils/lg.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3409 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/utils/lgl.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4061 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/utils/lgr.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6123 2022-09-16 16:16:20.000000 dymos-1.8.0/dymos/utils/misc.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.253609 dymos-1.8.0/dymos/utils/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/utils/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2225 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/utils/test/test_hermite.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1305 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/utils/test/test_indexing.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1524 2022-03-04 14:52:23.000000 dymos-1.8.0/dymos/utils/test/test_introspection.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1256 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/utils/test/test_lg.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1686 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/utils/test/test_lgl.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1966 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/utils/test/test_lgr.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      632 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/utils/test/test_misc.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23115 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/utils/test/test_testing_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    17883 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/utils/testing_utils.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.253609 dymos-1.8.0/dymos/visualization/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-07-01 16:42:29.000000 dymos-1.8.0/dymos/visualization/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.253609 dymos-1.8.0/dymos/visualization/linkage/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-08-08 20:47:06.000000 dymos-1.8.0/dymos/visualization/linkage/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.253609 dymos-1.8.0/dymos/visualization/linkage/js/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2445 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageCellRenderer.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1438 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageDiagram.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2802 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageLegend.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14276 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageMatrix.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3069 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageMatrixCell.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      898 2022-08-08 20:47:06.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageModelData.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3472 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageStyle.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1371 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageSymbolType.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5196 2023-01-03 17:56:55.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageTreeNode.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      723 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageUserInterface.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      605 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/visualization/linkage/js/DmLinkage_main.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13064 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/visualization/linkage/report.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14463 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/visualization/linkage/report_template.html
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.253609 dymos-1.8.0/dymos/visualization/linkage/style/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1905 2022-08-05 15:09:01.000000 dymos-1.8.0/dymos/visualization/linkage/style/linkage_report.css
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.253609 dymos-1.8.0/dymos/visualization/linkage/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-08-08 20:47:06.000000 dymos-1.8.0/dymos/visualization/linkage/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    30639 2023-02-07 21:41:37.000000 dymos-1.8.0/dymos/visualization/linkage/test/linkage_report_ui_test.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      245 2023-01-09 19:10:23.000000 dymos-1.8.0/dymos/visualization/linkage/test/test_gui.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.253609 dymos-1.8.0/dymos/visualization/test/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2022-08-08 20:47:06.000000 dymos-1.8.0/dymos/visualization/test/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    28070 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/visualization/test/test_timeseries_plots.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.253609 dymos-1.8.0/dymos/visualization/timeseries/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/visualization/timeseries/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    16279 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/visualization/timeseries/bokeh_timeseries_report.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    19015 2023-04-17 16:11:21.000000 dymos-1.8.0/dymos/visualization/timeseries_plots.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2023-04-18 15:54:58.203609 dymos-1.8.0/dymos.egg-info/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1445 2023-04-18 15:54:58.000000 dymos-1.8.0/dymos.egg-info/PKG-INFO
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22124 2023-04-18 15:54:58.000000 dymos-1.8.0/dymos.egg-info/SOURCES.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        1 2023-04-18 15:54:58.000000 dymos-1.8.0/dymos.egg-info/dependency_links.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       94 2023-04-18 15:54:58.000000 dymos-1.8.0/dymos.egg-info/entry_points.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        1 2023-04-18 15:54:58.000000 dymos-1.8.0/dymos.egg-info/not-zip-safe
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      476 2023-04-18 15:54:58.000000 dymos-1.8.0/dymos.egg-info/requires.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        6 2023-04-18 15:54:58.000000 dymos-1.8.0/dymos.egg-info/top_level.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       38 2023-04-18 15:54:58.253609 dymos-1.8.0/setup.cfg
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2813 2023-04-18 15:53:33.000000 dymos-1.8.0/setup.py
```

### Comparing `dymos-1.7.0/LICENSE` & `dymos-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/PKG-INFO` & `dymos-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dymos
-Version: 1.7.0
+Version: 1.8.0
 Summary: Open-Source Optimization of Dynamic Multidisciplinary Systems
 Home-page: https://github.com/OpenMDAO/dymos
 License: Apache License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/aero_coef_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/aero_coef_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/aero_forces_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/aero_forces_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/aerodynamics_group.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/aerodynamics_group.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/crm_data.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/crm_data.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/data/CRM_aero_inputs.dat` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/data/CRM_aero_inputs.dat`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/data/CRM_aero_outputs.dat` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/data/CRM_aero_outputs.dat`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/interpND_aero_coef_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/interpND_aero_coef_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/test/test_aero_coef_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/test/test_aero_coef_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/aero/test/test_interpND_aero_coef_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/aero/test/test_interpND_aero_coef_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/aircraft_ode.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/aircraft_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/dynamic_pressure_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/dynamic_pressure_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/lift_equilibrium_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/lift_equilibrium_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/steady_flight_equilibrium_group.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/steady_flight_equilibrium_group.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/test/test_flight_equilibrium_group.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/test/test_flight_equilibrium_group.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/thrust_equilibrium_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/flight_equlibrium/thrust_equilibrium_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/mass_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/mass_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/fuel_burn_rate_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/fuel_burn_rate_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/max_thrust_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/max_thrust_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/propulsion_group.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/propulsion_group.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/test/test_propulsion_group.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/test/test_propulsion_group.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/throttle_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/throttle_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/thrust_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/thrust_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/propulsion/tsfc_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/propulsion/tsfc_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/range_rate_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/range_rate_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/steady_flight_path_angle_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/steady_flight_path_angle_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/test/test_aircraft_cruise.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/test/test_aircraft_cruise.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/test/test_aircraft_ode.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/test/test_aircraft_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/test/test_ex_aircraft_steady_flight.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/test/test_ex_aircraft_steady_flight.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/aircraft_steady_flight/true_airspeed_comp.py` & `dymos-1.8.0/dymos/examples/aircraft_steady_flight/true_airspeed_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/balanced_field/balanced_field_ode.py` & `dymos-1.8.0/dymos/examples/balanced_field/balanced_field_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/balanced_field/doc/test_doc_balanced_field_length.py` & `dymos-1.8.0/dymos/examples/balanced_field/doc/test_doc_balanced_field_length.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,33 +7,32 @@
 
 
 @use_tempdirs
 class TestBalancedFieldLengthForDocs(unittest.TestCase):
 
     @require_pyoptsparse(optimizer='IPOPT')
     def test_balanced_field_length_for_docs(self):
-        import matplotlib.pyplot as plt
         import openmdao.api as om
         from openmdao.utils.general_utils import set_pyoptsparse_opt
-        from openmdao.utils.assert_utils import assert_near_equal
         import dymos as dm
         from dymos.examples.balanced_field.balanced_field_ode import BalancedFieldODEComp
 
         p = om.Problem()
 
         _, optimizer = set_pyoptsparse_opt('IPOPT', fallback=True)
 
-        p.driver = om.pyOptSparseDriver()
-        p.driver.declare_coloring()
+        dm.options['plots'] = 'bokeh'
 
         # Use IPOPT if available, with fallback to SLSQP
+        p.driver = om.pyOptSparseDriver(optimizer='SNOPT')
         p.driver.options['optimizer'] = optimizer
+        p.driver.declare_coloring()
         p.driver.options['print_results'] = False
         if optimizer == 'IPOPT':
-            p.driver.opt_settings['print_level'] = 0
+            p.driver.opt_settings['print_level'] = 5
             p.driver.opt_settings['derivative_test'] = 'first-order'
 
         # First Phase: Brake release to V1 - both engines operable
         br_to_v1 = dm.Phase(ode_class=BalancedFieldODEComp, transcription=dm.Radau(num_segments=3),
                             ode_init_kwargs={'mode': 'runway'})
         br_to_v1.set_time_options(fix_initial=True, duration_bounds=(1, 1000), duration_ref=10.0)
         br_to_v1.add_state('r', fix_initial=True, lower=0, ref=1000.0, defect_ref=1000.0)
@@ -192,14 +191,20 @@
         climb.add_boundary_constraint('h', loc='final', equals=35, ref=35, units='ft', linear=True)
         climb.add_boundary_constraint('gam', loc='final', equals=5, ref=5, units='deg', linear=True)
         climb.add_path_constraint('gam', lower=0, upper=5, ref=5, units='deg')
         climb.add_boundary_constraint('v_over_v_stall', loc='final', lower=1.25, ref=1.25)
 
         rto.add_objective('r', loc='final', ref=1.0)
 
+        for phase_name, phase in traj._phases.items():
+            phase.add_timeseries_output('T_nominal', output_name='T')
+            phase.add_timeseries_output('T_engine_out', output_name='T')
+            phase.add_timeseries_output('T_shutdown', output_name='T')
+            phase.add_timeseries_output('alpha')
+
         #
         # Setup the problem and set the initial guess
         #
         p.setup(check=True)
 
         p.set_val('traj.br_to_v1.t_initial', 0)
         p.set_val('traj.br_to_v1.t_duration', 35)
@@ -229,52 +234,8 @@
         p.set_val('traj.climb.t_duration', 15)
         p.set_val('traj.climb.states:r', climb.interp('r', [5000, 5500.0]), units='ft')
         p.set_val('traj.climb.states:v', climb.interp('v', [160, 170.0]), units='kn')
         p.set_val('traj.climb.states:h', climb.interp('h', [0, 35.0]), units='ft')
         p.set_val('traj.climb.states:gam', climb.interp('gam', [0, 5.0]), units='deg')
         p.set_val('traj.climb.controls:alpha', 5.0, units='deg')
 
-        dm.run_problem(p, run_driver=True, simulate=True)
-
-        # Test this example in Dymos' continuous integration
-        assert_near_equal(p.get_val('traj.rto.states:r')[-1], 2188.2, tolerance=0.01)
-
-        sim_case = om.CaseReader('dymos_solution.db').get_case('final')
-
-        fig, axes = plt.subplots(2, 1, sharex=True, gridspec_kw={'top': 0.92})
-        for phase in ['br_to_v1', 'rto', 'v1_to_vr', 'rotate', 'climb']:
-            r = sim_case.get_val(f'traj.{phase}.timeseries.states:r', units='ft')
-            v = sim_case.get_val(f'traj.{phase}.timeseries.states:v', units='kn')
-            t = sim_case.get_val(f'traj.{phase}.timeseries.time', units='s')
-            axes[0].plot(t, r, '-', label=phase)
-            axes[1].plot(t, v, '-', label=phase)
-        fig.suptitle('Balanced Field Length')
-        axes[1].set_xlabel('time (s)')
-        axes[0].set_ylabel('range (ft)')
-        axes[1].set_ylabel('airspeed (kts)')
-        axes[0].grid(True)
-        axes[1].grid(True)
-
-        tv1 = sim_case.get_val('traj.br_to_v1.timeseries.time', units='s')[-1, 0]
-        v1 = sim_case.get_val('traj.br_to_v1.timeseries.states:v', units='kn')[-1, 0]
-
-        tf_rto = sim_case.get_val('traj.rto.timeseries.time', units='s')[-1, 0]
-        rf_rto = sim_case.get_val('traj.rto.timeseries.states:r', units='ft')[-1, 0]
-
-        axes[0].annotate(f'field length = {r[-1, 0]:5.1f} ft', xy=(t[-1, 0], r[-1, 0]),
-                         xycoords='data', xytext=(0.7, 0.5),
-                         textcoords='axes fraction', arrowprops=dict(arrowstyle='->'),
-                         horizontalalignment='center', verticalalignment='top')
-
-        axes[0].annotate(f'', xy=(tf_rto, rf_rto),
-                         xycoords='data', xytext=(0.7, 0.5),
-                         textcoords='axes fraction', arrowprops=dict(arrowstyle='->'),
-                         horizontalalignment='center', verticalalignment='top')
-
-        axes[1].annotate(f'$v1$ = {v1:5.1f} kts', xy=(tv1, v1), xycoords='data', xytext=(0.5, 0.5),
-                         textcoords='axes fraction', arrowprops=dict(arrowstyle='->'),
-                         horizontalalignment='center', verticalalignment='top')
-
-        plt.legend()
-
-        if SHOW_PLOTS:
-            plt.show()
+        dm.run_problem(p, run_driver=True, simulate=True, make_plots=True)
```

### Comparing `dymos-1.7.0/dymos/examples/balanced_field/test/test_balanced_field_func_comp.py` & `dymos-1.8.0/dymos/examples/balanced_field/test/test_balanced_field_func_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/balanced_field/test/test_balanced_field_length.py` & `dymos-1.8.0/dymos/examples/balanced_field/test/test_balanced_field_length.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+from packaging.version import Version
 import unittest
 
 import numpy as np
 
+import openmdao
 import openmdao.api as om
 from openmdao.utils.testing_utils import use_tempdirs, require_pyoptsparse
 from openmdao.utils.assert_utils import assert_near_equal
 
 import dymos as dm
 from dymos.examples.balanced_field.balanced_field_ode import BalancedFieldODEComp
 
 
 @use_tempdirs
 class TestBalancedFieldLengthRestart(unittest.TestCase):
 
     def _make_problem(self):
-        p = om.Problem()
+        p = om.Problem(reports=True)
 
         p.driver = om.pyOptSparseDriver()
         p.driver.options['optimizer'] = 'IPOPT'
+        p.driver.options['invalid_desvar_behavior'] = 'ignore'
         p.driver.opt_settings['print_level'] = 0
         p.driver.opt_settings['derivative_test'] = 'first-order'
 
         p.driver.declare_coloring()
 
         # First Phase: Brake release to V1 - both engines operable
         br_to_v1 = dm.Phase(ode_class=BalancedFieldODEComp, transcription=dm.Radau(num_segments=3),
@@ -214,14 +217,23 @@
         p.set_val('traj.climb.states:h', climb.interp('h', [0, 35.0]), units='ft')
         p.set_val('traj.climb.states:gam', climb.interp('gam', [0, 5.0]), units='deg')
         p.set_val('traj.climb.controls:alpha', 5.0, units='deg')
 
         return p
 
     @require_pyoptsparse(optimizer='IPOPT')
+    @unittest.skipUnless(Version(openmdao.__version__) > Version("3.23"),
+                         reason='Test requires OpenMDAO 3.23.0 or later.')
+    def test_make_plots(self):
+        p = self._make_problem()
+        dm.run_problem(p, run_driver=True, simulate=True, make_plots=True)
+
+    @require_pyoptsparse(optimizer='IPOPT')
+    @unittest.skipUnless(Version(openmdao.__version__) > Version("3.23"),
+                         reason='Test requires OpenMDAO 3.23.0 or later.')
     def test_restart_from_sol(self):
         p = self._make_problem()
         dm.run_problem(p, run_driver=True, simulate=False)
 
         sol_results = om.CaseReader('dymos_solution.db').get_case('final')
 
         assert_near_equal(sol_results.get_val('traj.climb.timeseries.states:r')[-1], 2016, tolerance=0.01)
@@ -234,14 +246,16 @@
         assert_near_equal(sol_results.get_val('traj.climb.timeseries.states:r')[-1], 2016, tolerance=0.01)
         assert_near_equal(sim_results.get_val('traj.climb.timeseries.states:r')[-1], 2016, tolerance=0.01)
 
         assert_near_equal(sol_results.get_val('traj.rto.timeseries.states:r')[-1], 2016, tolerance=0.01)
         assert_near_equal(sim_results.get_val('traj.rto.timeseries.states:r')[-1], 2016, tolerance=0.01)
 
     @require_pyoptsparse(optimizer='IPOPT')
+    @unittest.skipUnless(Version(openmdao.__version__) > Version("3.23"),
+                         reason='Test requires OpenMDAO 3.23.0 or later.')
     def test_restart_from_sim(self):
         p = self._make_problem()
         dm.run_problem(p, run_driver=True, simulate=True)
 
         sol_results = om.CaseReader('dymos_solution.db').get_case('final')
 
         assert_near_equal(sol_results.get_val('traj.climb.timeseries.states:r')[-1], 2016,
```

### Comparing `dymos-1.7.0/dymos/examples/battery_multibranch/batteries.py` & `dymos-1.8.0/dymos/examples/battery_multibranch/batteries.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/battery_multibranch/battery_multibranch_ode.py` & `dymos-1.8.0/dymos/examples/battery_multibranch/battery_multibranch_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/battery_multibranch/motors.py` & `dymos-1.8.0/dymos/examples/battery_multibranch/motors.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/battery_multibranch/test/test_multibranch_trajectory.py` & `dymos-1.8.0/dymos/examples/battery_multibranch/test/test_multibranch_trajectory.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/brachistochrone_ode.py` & `dymos-1.8.0/dymos/examples/brachistochrone/brachistochrone_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/brachistochrone_vector_states_ode.py` & `dymos-1.8.0/dymos/examples/brachistochrone/brachistochrone_vector_states_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/doc/brachistochrone_ode.py` & `dymos-1.8.0/dymos/examples/brachistochrone/doc/brachistochrone_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone.py` & `dymos-1.8.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_static_gravity.py` & `dymos-1.8.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_static_gravity.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_tandem_phases.py` & `dymos-1.8.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_tandem_phases.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_upstream_control.py` & `dymos-1.8.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_upstream_control.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_upstream_state.py` & `dymos-1.8.0/dymos/examples/brachistochrone/doc/test_doc_brachistochrone_upstream_state.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/ex_brachistochrone.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/ex_brachistochrone.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,17 +74,23 @@
     p.setup(check=['unconnected_inputs'], force_alloc_complex=force_alloc_complex)
 
     phase.set_simulate_options(method='RK23')
 
     p['traj0.phase0.t_initial'] = 0.0
     p['traj0.phase0.t_duration'] = 2.0
 
-    p['traj0.phase0.states:x'] = phase.interp('x', [0, 10])
-    p['traj0.phase0.states:y'] = phase.interp('y', [10, 5])
-    p['traj0.phase0.states:v'] = phase.interp('v', [0, 9.9])
+    if transcription.startswith('shooting'):
+        p['traj0.phase0.initial_states:x'] = 0
+        p['traj0.phase0.initial_states:y'] = 10
+        p['traj0.phase0.initial_states:v'] = 0
+    else:
+        p['traj0.phase0.states:x'] = phase.interp('x', [0, 10])
+        p['traj0.phase0.states:y'] = phase.interp('y', [10, 5])
+        p['traj0.phase0.states:v'] = phase.interp('v', [0, 9.9])
+
     p['traj0.phase0.controls:theta'] = phase.interp('theta', [5, 100])
     p['traj0.phase0.parameters:g'] = 9.80665
 
     dm.run_problem(p, run_driver=run_driver, simulate=True, make_plots=True)
 
     return p
```

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/ex_brachistochrone_vector_states.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/ex_brachistochrone_vector_states.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_callable_ode_class.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_callable_ode_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
             y0 = p.get_val('traj0.phase0.timeseries.states:y')[0]
             yf = p.get_val('traj0.phase0.timeseries.states:y')[-1]
 
             v0 = p.get_val('traj0.phase0.timeseries.states:v')[0]
             vf = p.get_val('traj0.phase0.timeseries.states:v')[-1]
 
-            g = p.get_val('traj0.phase0.timeseries.parameters:g')[0]
+            g = p.get_val('traj0.phase0.parameter_vals:g')[0]
 
             thetaf = p.get_val('traj0.phase0.timeseries.controls:theta')[-1]
 
             assert_near_equal(t_initial, 0.0)
             assert_near_equal(x0, 0.0)
             assert_near_equal(y0, 10.0)
             assert_near_equal(v0, 0.0)
@@ -313,15 +313,15 @@
 
             y0 = p.get_val('traj0.phase0.timeseries.states:y')[0]
             yf = p.get_val('traj0.phase0.timeseries.states:y')[-1]
 
             v0 = p.get_val('traj0.phase0.timeseries.states:v')[0]
             vf = p.get_val('traj0.phase0.timeseries.states:v')[-1]
 
-            g = p.get_val('traj0.phase0.timeseries.parameters:g')[0]
+            g = p.get_val('traj0.phase0.parameter_vals:g')[0]
 
             thetaf = p.get_val('traj0.phase0.timeseries.controls:theta')[-1]
 
             assert_near_equal(t_initial, 0.0)
             assert_near_equal(x0, 0.0)
             assert_near_equal(y0, 10.0)
             assert_near_equal(v0, 0.0)
```

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_control_rate_targets.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_control_rate_targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -923,52 +923,15 @@
 
         p['phase0.states:x'] = phase.interp('x', [0, 10])
         p['phase0.states:y'] = phase.interp('y', [10, 5])
         p['phase0.states:v'] = phase.interp('v', [0, 9.9])
         p['phase0.polynomial_controls:theta'] = [0, 10, 40, 60, 80, 100]
 
         # Solve for the optimal trajectory
-        p.run_driver()
+        dm.run_problem(p, simulate=True)
 
         # Test the results
         assert_near_equal(p.get_val('phase0.timeseries.time')[-1], 1.8016, tolerance=1.0E-3)
 
-        # Generate the explicitly simulated trajectory
-        exp_out = phase.simulate()
-
-        fig, ax = plt.subplots()
-        fig.suptitle('Brachistochrone Solution')
-
-        x_imp = p.get_val('phase0.timeseries.states:x')
-        y_imp = p.get_val('phase0.timeseries.states:y')
-
-        x_exp = exp_out.get_val('phase0.timeseries.states:x')
-        y_exp = exp_out.get_val('phase0.timeseries.states:y')
-
-        ax.plot(x_imp, y_imp, 'ro', label='solution')
-        ax.plot(x_exp, y_exp, 'b-', label='simulated')
-
-        ax.set_xlabel('x (m)')
-        ax.set_ylabel('y (m)')
-        ax.grid(True)
-        ax.legend(loc='upper right')
-
-        fig, ax = plt.subplots()
-
-        t_imp = p.get_val('phase0.timeseries.time')
-        theta_imp = p.get_val('phase0.timeseries.polynomial_control_rates:theta_rate')
-        t_exp = exp_out.get_val('phase0.timeseries.time')
-        theta_exp = exp_out.get_val('phase0.timeseries.polynomial_control_rates:theta_rate')
-
-        ax.plot(t_imp, theta_imp, 'ro', label='solution')
-        ax.plot(t_exp, theta_exp, 'b-', label='simulated')
-
-        ax.set_xlabel('time (s)')
-        ax.set_ylabel(r'$\theta$ (deg)')
-        ax.grid(True)
-        ax.legend(loc='upper right')
-
-        plt.show()
-
 
 if __name__ == '__main__':  # pragma: no cover
     unittest.main()
```

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_external_control.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_external_control.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_implicit_recorder.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_implicit_recorder.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_integrated_control.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_integrated_control.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_integrated_parameter.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_integrated_parameter.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_path_constraint.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_path_constraint.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_quick_start.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_quick_start.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_simulate_options.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_simulate_options.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_solve_segments.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_solve_segments.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_static_gravity.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_static_gravity.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_subprob_reports.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_subprob_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,17 @@
 
     phase.add_objective('time', loc='final')
 
     prob.setup(force_alloc_complex=True)
 
     prob.set_val('phase0.t_initial', 0.0)
     prob.set_val('phase0.t_duration', 2)
-    prob.set_val('phase0.states:x', 0.0)
-    prob.set_val('phase0.states:y', 10.0)
-    prob.set_val('phase0.states:v', 1.0E-6)
+    prob.set_val('phase0.initial_states:x', 0.0)
+    prob.set_val('phase0.initial_states:y', 10.0)
+    prob.set_val('phase0.initial_states:v', 1.0E-6)
     prob.set_val('phase0.parameters:g', 1.0, units='m/s**2')
     prob.set_val('phase0.controls:theta', phase.interp('theta', ys=[0.01, 90]), units='deg')
 
     dm.run_problem(prob, run_driver=True, simulate=False)
 
     return prob
```

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_timeseries_feedback.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_timeseries_feedback.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_varying_order_control_simulation.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_varying_order_control_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         y0 = p.get_val('phase0.timeseries.states:y')[0]
         yf = p.get_val('phase0.timeseries.states:y')[-1]
 
         v0 = p.get_val('phase0.timeseries.states:v')[0]
         vf = p.get_val('phase0.timeseries.states:v')[-1]
 
-        g = p.get_val('phase0.timeseries.parameters:g')[0]
+        g = p.get_val('phase0.parameter_vals:g')[0]
 
         thetaf = exp_out.get_val('phase0.timeseries.controls:theta')[-1]
 
         assert_almost_equal(t_initial, 0.0)
         assert_almost_equal(x0, 0.0)
         assert_almost_equal(y0, 10.0)
         assert_almost_equal(v0, 0.0)
@@ -147,15 +147,15 @@
 
         y0 = p.get_val('phase0.timeseries.states:y')[0]
         yf = p.get_val('phase0.timeseries.states:y')[-1]
 
         v0 = p.get_val('phase0.timeseries.states:v')[0]
         vf = p.get_val('phase0.timeseries.states:v')[-1]
 
-        g = p.get_val('phase0.timeseries.parameters:g')[0]
+        g = p.get_val('phase0.parameter_vals:g')[0]
 
         thetaf = exp_out.get_val('phase0.timeseries.controls:theta')[-1]
 
         assert_almost_equal(t_initial, 0.0)
         assert_almost_equal(x0, 0.0)
         assert_almost_equal(y0, 10.0)
         assert_almost_equal(v0, 0.0)
```

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_boundary_constraints.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_boundary_constraints.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_path_constraints.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_path_constraints.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_states_ode.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_brachistochrone_vector_states_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_doc_brachistochrone_polynomial_controls.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_doc_brachistochrone_polynomial_controls.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_duplicate_constraints.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_duplicate_constraints.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_duplicate_timeseries_inputs.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_duplicate_timeseries_inputs.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         y0 = p.get_val('traj0.phase0.timeseries.states:y')[0]
         yf = p.get_val('traj0.phase0.timeseries.states:y')[-1]
 
         v0 = p.get_val('traj0.phase0.timeseries.states:v')[0]
         vf = p.get_val('traj0.phase0.timeseries.states:v')[-1]
 
-        g = p.get_val('traj0.phase0.timeseries.parameters:g')[0]
+        g = p.get_val('traj0.phase0.parameter_vals:g')[0]
 
         thetaf = p.get_val('traj0.phase0.timeseries.controls:theta')[-1]
 
         assert_almost_equal(t_initial, 0.0)
         assert_almost_equal(x0, 0.0)
         assert_almost_equal(y0, 10.0)
         assert_almost_equal(v0, 0.0)
```

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone_refine_grid.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone_refine_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
         y0 = p.get_val('traj0.phase0.timeseries.states:y')[0]
         yf = p.get_val('traj0.phase0.timeseries.states:y')[-1]
 
         v0 = p.get_val('traj0.phase0.timeseries.states:v')[0]
         vf = p.get_val('traj0.phase0.timeseries.states:v')[-1]
 
-        g = p.get_val('traj0.phase0.timeseries.parameters:g')[0]
+        g = p.get_val('traj0.phase0.parameter_vals:g')[0]
 
         thetaf = p.get_val('traj0.phase0.timeseries.controls:theta')[-1]
 
         assert_almost_equal(t_initial, 0.0)
         assert_almost_equal(x0, 0.0)
         assert_almost_equal(y0, 10.0)
         assert_almost_equal(v0, 0.0)
```

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone_vector_states.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_ex_brachistochrone_vector_states.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         y0 = p.get_val('traj0.phase0.timeseries.states:pos')[0, 1]
         yf = p.get_val('traj0.phase0.timeseries.states:pos')[-1, 1]
 
         v0 = p.get_val('traj0.phase0.timeseries.states:v')[0, 0]
         vf = p.get_val('traj0.phase0.timeseries.states:v')[-1, 0]
 
-        g = p.get_val('traj0.phase0.timeseries.parameters:g')
+        g = p.get_val('traj0.phase0.parameter_vals:g')
 
         thetaf = p.get_val('traj0.phase0.timeseries.controls:theta')[-1, 0]
 
         assert_almost_equal(t_initial, 0.0)
         assert_almost_equal(x0, 0.0)
         assert_almost_equal(y0, 10.0)
         assert_almost_equal(v0, 0.0)
```

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_path_constraints.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_path_constraints.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 
+import numpy as np
 from openmdao.utils.testing_utils import use_tempdirs, require_pyoptsparse
 
 
 @use_tempdirs
 class TestBrachistochronePathConstraints(unittest.TestCase):
 
     def test_control_rate_path_constraint_gl(self):
@@ -95,22 +96,24 @@
 
         p['phase0.states:x'] = phase.interp('x', [0, 10])
         p['phase0.states:y'] = phase.interp('y', [10, 5])
         p['phase0.states:v'] = phase.interp('v', [0, 9.9])
         p['phase0.controls:theta'] = phase.interp('theta', [5, 100.5])
 
         # Solve for the optimal trajectory
-        p.run_driver()
+        failed = p.run_driver()
+        self.assertFalse(failed, msg='optimization failed')
 
         # Test the results
-        assert_near_equal(p.get_val('phase0.timeseries.time')[-1], 1.8016, tolerance=1.0E-3)
+        rate_path = 'control_rates:theta_rate2' if dm.options['use_timeseries_prefix'] else 'theta_rate2'
+        self.assertGreaterEqual(np.min(p.get_val(f'phase0.timeseries.{rate_path}')), -200.000001)
+        self.assertLessEqual(np.max(p.get_val(f'phase0.timeseries.{rate_path}')), 200.000001)
 
     def test_control_rate_path_constraint_radau(self):
         import openmdao.api as om
-        from openmdao.utils.assert_utils import assert_near_equal
         import dymos as dm
         from dymos.examples.brachistochrone.brachistochrone_ode import BrachistochroneODE
 
         p = om.Problem(model=om.Group())
         p.driver = om.ScipyOptimizeDriver()
 
         phase = dm.Phase(ode_class=BrachistochroneODE,
@@ -144,18 +147,21 @@
 
         p['phase0.states:x'] = phase.interp('x', ys=[0, 10])
         p['phase0.states:y'] = phase.interp('y', ys=[10, 5])
         p['phase0.states:v'] = phase.interp('v', ys=[0, 9.9])
         p['phase0.controls:theta'] = phase.interp('theta', ys=[0.9, 101.5])
 
         # Solve for the optimal trajectory
-        p.run_driver()
+        failed = p.run_driver()
+        self.assertFalse(failed, msg='optimization failed')
 
         # Test the results
-        assert_near_equal(p.get_val('phase0.timeseries.time')[-1], 1.8016, tolerance=1.0E-3)
+        rate_path = 'control_rates:theta_rate' if dm.options['use_timeseries_prefix'] else 'theta_rate'
+        self.assertGreaterEqual(np.min(p.get_val(f'phase0.timeseries.{rate_path}')), -0.000001)
+        self.assertLessEqual(np.max(p.get_val(f'phase0.timeseries.{rate_path}')), 100.000001)
 
     def test_control_rate2_path_constraint_radau(self):
         import openmdao.api as om
         from openmdao.utils.assert_utils import assert_near_equal
         import dymos as dm
         from dymos.examples.brachistochrone.brachistochrone_ode import BrachistochroneODE
 
@@ -195,23 +201,25 @@
 
         p['phase0.states:x'] = phase.interp('x', [0, 10])
         p['phase0.states:y'] = phase.interp('y', [10, 5])
         p['phase0.states:v'] = phase.interp('v', [0, 9.9])
         p['phase0.controls:theta'] = phase.interp('theta', [5, 100.5])
 
         # Solve for the optimal trajectory
-        p.run_driver()
+        failed = p.run_driver()
+        self.assertFalse(failed, msg='optimization failed')
 
         # Test the results
-        assert_near_equal(p.get_val('phase0.timeseries.time')[-1], 1.8016, tolerance=1.0E-3)
+        rate_path = 'control_rates:theta_rate2' if dm.options['use_timeseries_prefix'] else 'theta_rate2'
+        self.assertGreaterEqual(np.min(p.get_val(f'phase0.timeseries.{rate_path}')), -200.000001)
+        self.assertLessEqual(np.max(p.get_val(f'phase0.timeseries.{rate_path}')), 200.000001)
 
     @require_pyoptsparse(optimizer='IPOPT')
     def test_state_path_constraint_radau(self):
         import openmdao.api as om
-        from openmdao.utils.assert_utils import assert_near_equal
         import dymos as dm
         from dymos.examples.brachistochrone.brachistochrone_ode import BrachistochroneODE
 
         p = om.Problem(model=om.Group())
         p.driver = om.pyOptSparseDriver(optimizer='IPOPT')
 
         traj = dm.Trajectory()
@@ -249,23 +257,24 @@
 
         p['traj0.phase0.states:x'] = phase.interp('x', ys=[0, 10])
         p['traj0.phase0.states:y'] = phase.interp('y', ys=[10, 5])
         p['traj0.phase0.states:v'] = phase.interp('v', ys=[0, 9.9])
         p['traj0.phase0.controls:theta'] = phase.interp('theta', ys=[0.9, 101.5])
 
         # Solve for the optimal trajectory
-        p.run_driver()
+        failed = p.run_driver()
+        self.assertFalse(failed, msg='optimization failed')
 
         # Test the results
-        assert_near_equal(p.get_val('traj0.phase0.timeseries.time')[-1], 1.8029, tolerance=1.0E-3)
+        state_path = 'states:y' if dm.options['use_timeseries_prefix'] else 'x'
+        self.assertGreaterEqual(np.min(p.get_val(f'traj0.phase0.timeseries.{state_path}')), 4.999999)
 
     @require_pyoptsparse(optimizer='IPOPT')
     def test_state_path_constraint_gl(self):
         import openmdao.api as om
-        from openmdao.utils.assert_utils import assert_near_equal
         import dymos as dm
         from dymos.examples.brachistochrone.brachistochrone_ode import BrachistochroneODE
 
         p = om.Problem(model=om.Group())
         p.driver = om.pyOptSparseDriver(optimizer='IPOPT')
 
         traj = dm.Trajectory()
@@ -303,15 +312,17 @@
 
         p['traj0.phase0.states:x'] = phase.interp('x', ys=[0, 10])
         p['traj0.phase0.states:y'] = phase.interp('y', ys=[10, 5])
         p['traj0.phase0.states:v'] = phase.interp('v', ys=[0, 9.9])
         p['traj0.phase0.controls:theta'] = phase.interp('theta', ys=[0.9, 101.5])
 
         # Solve for the optimal trajectory
-        p.run_driver()
+        failed = p.run_driver()
+        self.assertFalse(failed, msg='optimization failed')
 
         # Test the results
-        assert_near_equal(p.get_val('traj0.phase0.timeseries.time')[-1], 1.8029, tolerance=1.0E-3)
+        state_path = 'states:y' if dm.options['use_timeseries_prefix'] else 'x'
+        self.assertGreaterEqual(np.min(p.get_val(f'traj0.phase0.timeseries.{state_path}')), 4.999999)
 
 
 if __name__ == '__main__':  # pragma: no cover
     unittest.main()
```

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_simulate_units.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_simulate_units.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,12 +88,12 @@
 
         # Run the driver to solve the problem
         dm.run_problem(p, simulate=True)
 
         sol_case = om.CaseReader('dymos_solution.db').get_case('final')
         sim_case = om.CaseReader('dymos_simulation.db').get_case('final')
 
-        assert_near_equal(sim_case.get_val('traj.phase0.timeseries.parameters:g', units='m/s**2')[0],
-                          sol_case.get_val('traj.phase0.timeseries.parameters:g', units='m/s**2')[0])
+        assert_near_equal(sim_case.get_val('traj.phase0.parameter_vals:g', units='m/s**2')[0],
+                          sol_case.get_val('traj.phase0.parameter_vals:g', units='m/s**2')[0])
 
         assert_near_equal(sol_case.get_val('traj.phase0.timeseries.time')[-1], 1.8016, tolerance=1.0E-4)
         assert_near_equal(sim_case.get_val('traj.phase0.timeseries.time')[-1], 1.8016, tolerance=1.0E-4)
```

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_state_rate_introspection.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_state_rate_introspection.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_static_outputs.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_static_outputs.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_tandem_phases.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_tandem_phases.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/brachistochrone/test/test_timeseries_units.py` & `dymos-1.8.0/dymos/examples/brachistochrone/test/test_timeseries_units.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,24 +61,26 @@
         # to a top-level input named 'v' in the ODE, and connect to nothing if it's not found.
         phase.add_state('v', fix_initial=True, fix_final=False, solve_segments=solve_segments)
 
         phase.add_control('theta',
                           continuity=True, rate_continuity=True,
                           units='deg', lower=0.01, upper=179.9)
 
-        phase.add_parameter('g', units='m/s**2', static_target=True)
+        phase.add_parameter('g', units='m/s**2', static_target=True, include_timeseries=True)
 
         phase.add_boundary_constraint('x', loc='final', equals=10)
         phase.add_boundary_constraint('y', loc='final', equals=5)
         # Minimize time at the end of the phase
         phase.add_objective('time_phase', loc='final', scaler=10)
 
         phase.add_timeseries_output('xdot', units='degF')
         phase.add_timeseries_output('ydot', units='degC')
 
+        phase.timeseries_options['include_state_rates'] = True
+
         p.setup(check=['unconnected_inputs'], force_alloc_complex=force_alloc_complex)
 
         p['traj0.phase0.t_initial'] = 0.0
         p['traj0.phase0.t_duration'] = 2.0
 
         p['traj0.phase0.states:x'] = phase.interp('x', [0, 10])
         p['traj0.phase0.states:y'] = phase.interp('y', [10, 5])
```

### Comparing `dymos-1.7.0/dymos/examples/cannonball/cannonball_ode.py` & `dymos-1.8.0/dymos/examples/cannonball/cannonball_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/cannonball/doc/test_doc_two_phase_cannonball.py` & `dymos-1.8.0/dymos/examples/cannonball/doc/test_doc_two_phase_cannonball.py`

 * *Files 3% similar despite different names*

```diff
@@ -320,29 +320,12 @@
             axes[i].set_ylabel(state)
 
             axes[i].plot(time_imp['ascent'], x_imp['ascent'], 'bo')
             axes[i].plot(time_imp['descent'], x_imp['descent'], 'ro')
             axes[i].plot(time_exp['ascent'], x_exp['ascent'], 'b--')
             axes[i].plot(time_exp['descent'], x_exp['descent'], 'r--')
 
-        params = ['m', 'S']
-        fig, axes = plt.subplots(nrows=6, ncols=1, figsize=(12, 6))
-        for i, param in enumerate(params):
-            p_imp = {
-                'ascent': p.get_val(f'traj.ascent.timeseries.parameters:{param}'),
-                'descent': p.get_val(f'traj.descent.timeseries.parameters:{param}')}
-
-            p_exp = {'ascent': exp_out.get_val(f'traj.ascent.timeseries.parameters:{param}'),
-                     'descent': exp_out.get_val(f'traj.descent.timeseries.parameters:{param}')}
-
-            axes[i].set_ylabel(param)
-
-            axes[i].plot(time_imp['ascent'], p_imp['ascent'], 'bo')
-            axes[i].plot(time_imp['descent'], p_imp['descent'], 'ro')
-            axes[i].plot(time_exp['ascent'], p_exp['ascent'], 'b--')
-            axes[i].plot(time_exp['descent'], p_exp['descent'], 'r--')
-
         plt.show()
 
 
 if __name__ == '__main__':  # pragma: no cover
     unittest.main()
```

### Comparing `dymos-1.7.0/dymos/examples/cannonball/size_comp.py` & `dymos-1.8.0/dymos/examples/cannonball/size_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/cannonball/test/test_cannonball_expr_constraint.py` & `dymos-1.8.0/dymos/examples/cannonball/test/test_cannonball_expr_constraint.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/cannonball/test/test_cannonball_matrix_state.py` & `dymos-1.8.0/dymos/examples/cannonball/test/test_cannonball_matrix_state.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/cannonball/test/test_connect_control_to_parameter.py` & `dymos-1.8.0/dymos/examples/cannonball/test/test_connect_control_to_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,12 +202,12 @@
         p.set_val('traj.descent.states:v', descent.interp('v', [150, 200]))
         p.set_val('traj.descent.states:gam', descent.interp('gam', [0, -45]), units='deg')
 
         dm.run_problem(p, simulate=True, make_plots=True)
 
         assert_near_equal(p.get_val('traj.descent.states:r')[-1], 3183.25, tolerance=1.0E-2)
         assert_near_equal(p.get_val('traj.ascent.timeseries.controls:CD')[-1],
-                          p.get_val('traj.descent.timeseries.parameters:CD')[0])
+                          p.get_val('traj.descent.parameter_vals:CD')[0])
 
 
 if __name__ == '__main__':  # pragma: no cover
     unittest.main()
```

### Comparing `dymos-1.7.0/dymos/examples/cannonball/test/test_load_case_missing_phase.py` & `dymos-1.8.0/dymos/examples/cannonball/test/test_load_case_missing_phase.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/cannonball/test/test_phase_linkage_compliance.py` & `dymos-1.8.0/dymos/examples/cannonball/test/test_phase_linkage_compliance.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/cannonball/test/test_two_phase_cannonball_ode_output_linkage.py` & `dymos-1.8.0/dymos/examples/cannonball/test/test_two_phase_cannonball_ode_output_linkage.py`

 * *Files 12% similar despite different names*

```diff
@@ -126,92 +126,24 @@
         p.set_val('traj.descent.states:gam', descent.interp('gam', [0, -45]), units='deg')
 
         dm.run_problem(p)
 
         assert_near_equal(p.get_val('traj.descent.states:r')[-1],
                           3183.25, tolerance=1.0E-2)
 
-        exp_out = traj.simulate()
-
         print('optimal radius: {0:6.4f} m '.format(p.get_val('radius',
                                                              units='m')[0]))
         print('cannonball mass: {0:6.4f} kg '.format(p.get_val('size_comp.mass',
                                                                units='kg')[0]))
         print('launch angle: {0:6.4f} '
               'deg '.format(p.get_val('traj.ascent.timeseries.states:gam',  units='deg')[0, 0]))
         print('maximum range: {0:6.4f} '
               'm '.format(p.get_val('traj.descent.timeseries.states:r')[-1, 0]))
 
-        fig, axes = plt.subplots(nrows=1, ncols=1, figsize=(10, 6))
-
-        time_imp = {'ascent': p.get_val('traj.ascent.timeseries.time'),
-                    'descent': p.get_val('traj.descent.timeseries.time')}
-
-        time_exp = {'ascent': exp_out.get_val('traj.ascent.timeseries.time'),
-                    'descent': exp_out.get_val('traj.descent.timeseries.time')}
-
-        r_imp = {'ascent': p.get_val('traj.ascent.timeseries.states:r'),
-                 'descent': p.get_val('traj.descent.timeseries.states:r')}
-
-        r_exp = {'ascent': exp_out.get_val('traj.ascent.timeseries.states:r'),
-                 'descent': exp_out.get_val('traj.descent.timeseries.states:r')}
-
-        h_imp = {'ascent': p.get_val('traj.ascent.timeseries.states:h'),
-                 'descent': p.get_val('traj.descent.timeseries.states:h')}
-
-        h_exp = {'ascent': exp_out.get_val('traj.ascent.timeseries.states:h'),
-                 'descent': exp_out.get_val('traj.descent.timeseries.states:h')}
-
-        axes.plot(r_imp['ascent'], h_imp['ascent'], 'bo')
-
-        axes.plot(r_imp['descent'], h_imp['descent'], 'ro')
-
-        axes.plot(r_exp['ascent'], h_exp['ascent'], 'b--')
-
-        axes.plot(r_exp['descent'], h_exp['descent'], 'r--')
-
-        axes.set_xlabel('range (m)')
-        axes.set_ylabel('altitude (m)')
-
-        fig, axes = plt.subplots(nrows=4, ncols=1, figsize=(10, 6))
-        states = ['r', 'h', 'v', 'gam']
-        for i, state in enumerate(states):
-            x_imp = {'ascent': p.get_val('traj.ascent.timeseries.states:{0}'.format(state)),
-                     'descent': p.get_val('traj.descent.timeseries.states:{0}'.format(state))}
-
-            x_exp = {'ascent': exp_out.get_val('traj.ascent.timeseries.states:{0}'.format(state)),
-                     'descent': exp_out.get_val('traj.descent.timeseries.states:{0}'.format(state))}
-
-            axes[i].set_ylabel(state)
-
-            axes[i].plot(time_imp['ascent'], x_imp['ascent'], 'bo')
-            axes[i].plot(time_imp['descent'], x_imp['descent'], 'ro')
-            axes[i].plot(time_exp['ascent'], x_exp['ascent'], 'b--')
-            axes[i].plot(time_exp['descent'], x_exp['descent'], 'r--')
-
-        params = ['CD', 'mass', 'S']
-        fig, axes = plt.subplots(nrows=3, ncols=1, figsize=(12, 6))
-        for i, param in enumerate(params):
-            p_imp = {
-                'ascent': p.get_val('traj.ascent.timeseries.parameters:{0}'.format(param)),
-                'descent': p.get_val('traj.descent.timeseries.parameters:{0}'.format(param))}
-
-            p_exp = {'ascent': exp_out.get_val('traj.ascent.timeseries.'
-                                               'parameters:{0}'.format(param)),
-                     'descent': exp_out.get_val('traj.descent.timeseries.'
-                                                'parameters:{0}'.format(param))}
-
-            axes[i].set_ylabel(param)
-
-            axes[i].plot(time_imp['ascent'], p_imp['ascent'], 'bo')
-            axes[i].plot(time_imp['descent'], p_imp['descent'], 'ro')
-            axes[i].plot(time_exp['ascent'], p_exp['ascent'], 'b--')
-            axes[i].plot(time_exp['descent'], p_exp['descent'], 'r--')
-
-        plt.show()
+        assert_near_equal(p.get_val('traj.linkages.ascent:ke_final|descent:ke_initial'), 0.0)
 
     @require_pyoptsparse(optimizer='SLSQP')
     def test_traj_param_target_none(self):
         # Tests a bug where you couldn't specify None as a target for a specific phase.
         import openmdao.api as om
         from openmdao.utils.assert_utils import assert_near_equal
```

### Comparing `dymos-1.7.0/dymos/examples/cart_pole/animate_cartpole.py` & `dymos-1.8.0/dymos/examples/cart_pole/animate_cartpole.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/cart_pole/cartpole_dynamics.py` & `dymos-1.8.0/dymos/examples/cart_pole/cartpole_dynamics.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/double_integrator/doc/test_doc_double_integrator.py` & `dymos-1.8.0/dymos/examples/double_integrator/doc/test_doc_double_integrator.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/double_integrator/double_integrator_ode.py` & `dymos-1.8.0/dymos/examples/double_integrator/double_integrator_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/double_integrator/test/test_double_integrator.py` & `dymos-1.8.0/dymos/examples/double_integrator/test/test_double_integrator.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/double_integrator/test/test_double_integrator_timeseries_units.py` & `dymos-1.8.0/dymos/examples/double_integrator/test/test_double_integrator_timeseries_units.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     phase.add_state('x', fix_initial=True, rate_source='v', units='ft', shape=(1, ))
 
     phase.add_control('u', units='m/s**2', scaler=0.01, continuity=False, rate_continuity=False,
                       rate2_continuity=False, shape=(1, ), lower=-1.0, upper=1.0)
 
     phase.set_simulate_options(rtol=1.0E-9, atol=1.0E-9)
 
+    phase.timeseries_options['include_state_rates'] = True
+
     # Maximize distance travelled in one second.
     phase.add_objective('x', loc='final', scaler=-1)
 
     p.model.linear_solver = om.DirectSolver()
 
     p.setup(check=True)
```

### Comparing `dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/doc/test_doc_finite_burn_orbit_raise.py` & `dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/doc/test_doc_finite_burn_orbit_raise.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/finite_burn_eom.py` & `dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/finite_burn_eom.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/finite_burn_orbit_raise_problem.py` & `dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/finite_burn_orbit_raise_problem.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise.py` & `dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise_bokeh_plots.py` & `dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise_bokeh_plots.py`

 * *Files 9% similar despite different names*

```diff
@@ -201,30 +201,27 @@
     @unittest.skipIf(not bokeh_available, 'bokeh unavailable')
     def test_bokeh_plots(self):
         dm.options['plots'] = 'bokeh'
 
         p = two_burn_orbit_raise_problem(transcription='gauss-lobatto', transcription_order=3,
                                          compressed=False, optimizer='SLSQP', show_output=False)
 
-        plot_dir = pathlib.Path(_get_reports_dir(p)).joinpath('plots')
-        self.assertSetEqual({'plots.html'}, set(os.listdir(plot_dir)))
+        html_file = pathlib.Path(_get_reports_dir(p)) / 'traj_results_report.html'
+        self.assertTrue(html_file.exists(), msg=f'{html_file} does not exist!')
 
     def test_mpl_plots(self):
         dm.options['plots'] = 'matplotlib'
 
         p = two_burn_orbit_raise_problem(transcription='gauss-lobatto', transcription_order=3,
                                          compressed=False, optimizer='SLSQP', show_output=False)
 
-        expected_files = {'control_rates_u1_rate.png', 'state_rates_r.png', 'states_deltav.png',
-                          'states_r.png', 'state_rates_accel.png', 'state_rates_deltav.png',
-                          'states_accel.png', 'controls_u1.png', 'states_vr.png', 'pos_x.png',
-                          'states_vt.png', 'pos_y.png', 'parameters_u1.png', 'states_theta.png',
-                          'control_rates_u1_rate2.png', 'state_rates_vt.png', 'time_phase.png',
-                          'parameters_c.png', 'state_rates_theta.png', 'state_rates_vr.png', 'dt_dstau.png'}
-
-        html_files = {str(pathlib.Path(f).with_suffix('.html')) for f in expected_files}
-        plot_dir = pathlib.Path(_get_reports_dir(p)).joinpath('plots')
-        self.assertSetEqual(expected_files.union(html_files), set(os.listdir(plot_dir)))
+        expected_files = ('states_deltav.png', 'states_r.png', 'states_accel.png',
+                          'controls_u1.png', 'states_vr.png', 'pos_x.png',
+                          'states_vt.png', 'pos_y.png', 'states_theta.png')
+
+        for file in expected_files:
+            plotfile = pathlib.Path(_get_reports_dir(p)).joinpath('plots') / file
+            self.assertTrue(plotfile.exists(), msg=f'{plotfile} does not exist!')
 
 
 if __name__ == '__main__':  # pragma: no cover
     unittest.main()
```

### Comparing `dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise_mpi.py` & `dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_ex_two_burn_orbit_raise_mpi.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_finite_burn_eom.py` & `dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_finite_burn_eom.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_multi_phase_restart.py` & `dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_multi_phase_restart.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/finite_burn_orbit_raise/test/test_two_burn_orbit_raise_linkages.py` & `dymos-1.8.0/dymos/examples/finite_burn_orbit_raise/test/test_two_burn_orbit_raise_linkages.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,20 +117,128 @@
 
         # Finish Problem Setup
         p.model.linear_solver = om.DirectSolver()
 
         with self.assertRaises(ValueError) as e:
             p.setup(check=True, force_alloc_complex=True)
 
-        expected_exception = 'traj: Linkage units were not specified but the units of var_a (DU/TU**2) and var_b ' \
-                             '(km/s**2) are not the same. Units for this linkage constraint must ' \
+        expected_exception = 'traj: Linkage units were not specified but the units of burn1.accel (DU/TU**2) and ' \
+                             'burn2.accel (km/s**2) are not equivalent. Units for this linkage constraint must ' \
                              'be specified explicitly.'
 
         self.assertEqual(expected_exception, str(e.exception))
 
+    def test_two_burn_orbit_raise_gl_radau_gl_equivalent_units_error(self):
+        import openmdao.api as om
+
+        import dymos as dm
+        from dymos.examples.finite_burn_orbit_raise.finite_burn_eom import FiniteBurnODE
+
+        traj = dm.Trajectory()
+        p = om.Problem(model=om.Group())
+        p.model.add_subsystem('traj', traj)
+
+        p.driver = om.pyOptSparseDriver()
+        p.driver.options['optimizer'] = 'IPOPT'
+
+        p.driver.declare_coloring()
+
+        traj.add_parameter('c', opt=False, val=1.5, units='DU/TU',
+                           targets={'burn1': ['c'], 'coast': ['c'], 'burn2': ['c']})
+
+        # First Phase (burn)
+
+        burn1 = dm.Phase(ode_class=FiniteBurnODE,
+                         transcription=dm.GaussLobatto(num_segments=10, order=3, compressed=True))
+
+        burn1 = traj.add_phase('burn1', burn1)
+
+        burn1.set_time_options(fix_initial=True, duration_bounds=(.5, 10), units='TU')
+        burn1.add_state('r', fix_initial=True, fix_final=False, defect_scaler=100.0,
+                        rate_source='r_dot', targets=['r'], units='nmi')
+        burn1.add_state('theta', fix_initial=True, fix_final=False, defect_scaler=100.0,
+                        rate_source='theta_dot', targets=['theta'], units='rad')
+        burn1.add_state('vr', fix_initial=True, fix_final=False, defect_scaler=100.0,
+                        rate_source='vr_dot', targets=['vr'], units='DU/TU')
+        burn1.add_state('vt', fix_initial=True, fix_final=False, defect_scaler=100.0,
+                        rate_source='vt_dot', targets=['vt'], units='DU/TU')
+        burn1.add_state('accel', fix_initial=True, fix_final=False,
+                        rate_source='at_dot', targets=['accel'], units='DU/TU**2')
+        burn1.add_state('deltav', fix_initial=True, fix_final=False,
+                        rate_source='deltav_dot', units='DU/TU')
+        burn1.add_control('u1', rate_continuity=True, rate2_continuity=True, units='deg',
+                          scaler=0.01,
+                          rate_continuity_scaler=0.001, rate2_continuity_scaler=0.001,
+                          lower=-30, upper=30, targets=['u1'])
+
+        # Second Phase (Coast)
+        coast = dm.Phase(ode_class=FiniteBurnODE,
+                         transcription=dm.Radau(num_segments=10, order=3))
+
+        traj.add_phase('coast', coast)
+
+        coast.set_time_options(initial_bounds=(0.5, 20), duration_bounds=(.5, 10), duration_ref=10, units='TU')
+
+        coast.add_state('r', fix_initial=False, fix_final=False, defect_scaler=100.0,
+                        rate_source='r_dot', targets=['r'], units='nmi')
+        coast.add_state('theta', fix_initial=False, fix_final=False, defect_scaler=100.0,
+                        units='rad', rate_source='theta_dot', targets=['theta'])
+        coast.add_state('vr', fix_initial=False, fix_final=False, defect_scaler=100.0,
+                        rate_source='vr_dot', targets=['vr'], units='DU/TU')
+        coast.add_state('vt', fix_initial=False, fix_final=False, defect_scaler=100.0,
+                        rate_source='vt_dot', targets=['vt'], units='DU/TU')
+        coast.add_state('accel', fix_initial=True, fix_final=False, ref=1.0E-12, defect_ref=1.0E-12,
+                        rate_source='at_dot', targets=['accel'], units='DU/TU**2')
+        coast.add_state('deltav', fix_initial=False, fix_final=False,
+                        rate_source='deltav_dot', units='DU/TU')
+        coast.add_parameter('u1', targets=['u1'], opt=False, val=0.0, units='deg')
+
+        # Third Phase (burn)
+
+        burn2 = dm.Phase(ode_class=FiniteBurnODE,
+                         transcription=dm.GaussLobatto(num_segments=10, order=3, compressed=True))
+
+        traj.add_phase('burn2', burn2)
+
+        burn2.set_time_options(initial_bounds=(0.5, 20), duration_bounds=(.5, 10), initial_ref=10, units='TU')
+        burn2.add_state('r', fix_initial=False, fix_final=True,
+                        rate_source='r_dot', targets=['r'], units='NM')
+        burn2.add_state('theta', fix_initial=False, fix_final=False,
+                        rate_source='theta_dot', targets=['theta'], units='rad')
+        burn2.add_state('vr', fix_initial=False, fix_final=True,
+                        rate_source='vr_dot', targets=['vr'], units='DU/TU')
+        burn2.add_state('vt', fix_initial=False, fix_final=True,
+                        rate_source='vt_dot', targets=['vt'], units='DU/TU')
+        burn2.add_state('accel', fix_initial=False, fix_final=False, defect_ref=1.0E-6,
+                        rate_source='at_dot', targets=['accel'], units='DU/TU**2')
+        burn2.add_state('deltav', fix_initial=False, fix_final=False,
+                        rate_source='deltav_dot', units='DU/TU')
+        burn2.add_control('u1', targets=['u1'], rate_continuity=True, rate2_continuity=True,
+                          units='deg', scaler=0.01, lower=-30, upper=30)
+
+        burn2.add_objective('deltav', loc='final', scaler=1.0)
+
+        burn1.add_timeseries_output('pos_x')
+        coast.add_timeseries_output('pos_x')
+        burn2.add_timeseries_output('pos_x')
+
+        burn1.add_timeseries_output('pos_y')
+        coast.add_timeseries_output('pos_y')
+        burn2.add_timeseries_output('pos_y')
+
+        # Link Phases
+        traj.link_phases(phases=['burn1', 'coast', 'burn2'],
+                         vars=['time', 'r', 'vr', 'vt', 'deltav'])
+        traj.link_phases(phases=['burn1', 'burn2'], vars=['accel'])
+
+        # Finish Problem Setup
+        p.model.linear_solver = om.DirectSolver()
+
+        p.setup(check=True, force_alloc_complex=True)
+
     def test_two_burn_orbit_raise_gl_radau_gl_constrained(self):
         import numpy as np
 
         import matplotlib.pyplot as plt
 
         import openmdao.api as om
         from openmdao.utils.assert_utils import assert_near_equal
@@ -513,16 +621,16 @@
         # This tolerance is loosened because we're testing that the control
         # stays continuous across the trajectory phases, which isn't necessarily optimal.
         assert_near_equal(p.get_val('traj.burn2.timeseries.states:deltav')[-1],
                           0.3995,
                           tolerance=0.05)
 
         burn1_u1_final = p.get_val('traj.burn1.timeseries.controls:u1')[-1, ...]
-        coast_u1_initial = p.get_val('traj.coast.timeseries.parameters:u1')[0, ...]
-        coast_u1_final = p.get_val('traj.coast.timeseries.parameters:u1')[-1, ...]
+        coast_u1_initial = p.get_val('traj.coast.parameter_vals:u1')[0, ...]
+        coast_u1_final = p.get_val('traj.coast.parameter_vals:u1')[-1, ...]
         burn2_u1_initial = p.get_val('traj.burn2.timeseries.controls:u1')[0, ...]
 
         assert_near_equal(burn1_u1_final - coast_u1_initial, 0.0, 1e-12)
         assert_near_equal(coast_u1_final - burn2_u1_initial, 0.0, 1e-12)
 
     @use_tempdirs
     def test_two_burn_orbit_raise_gl_list_add_timeseries_output(self):
```

### Comparing `dymos-1.7.0/dymos/examples/flying_robot/flying_robot_ode.py` & `dymos-1.8.0/dymos/examples/flying_robot/flying_robot_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/flying_robot/test/test_flying_robot.py` & `dymos-1.8.0/dymos/examples/flying_robot/test/test_flying_robot.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/hull_problem/hull_ode.py` & `dymos-1.8.0/dymos/examples/hull_problem/hull_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/hull_problem/test/test_hull_problem.py` & `dymos-1.8.0/dymos/examples/hull_problem/test/test_hull_problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,20 @@
         phase0.add_state('xL', fix_initial=True, fix_final=False, rate_source='L')
         phase0.add_control('u', opt=True, targets=['u'])
 
         phase0.add_objective(f'J = {c}*x**2/2 + xL')
 
         p.setup(check=True)
 
-        p.set_val('traj.phase.states:x', phase0.interp('x', [1.5, 1]))
-        p.set_val('traj.phase.states:xL', phase0.interp('xL', [0, 1]))
+        if transcription is ExplicitShooting:
+            p.set_val('traj.phase.initial_states:x', 1.5)
+            p.set_val('traj.phase.initial_states:xL', 0.0)
+        else:
+            p.set_val('traj.phase.states:x', phase0.interp('x', [1.5, 1]))
+            p.set_val('traj.phase.states:xL', phase0.interp('xL', [0, 1]))
         p.set_val('traj.phase.t_initial', 0)
         p.set_val('traj.phase.t_duration', 10)
         p.set_val('traj.phase.controls:u', phase0.interp('u', [-7, -0.14]))
 
         return p
 
     @staticmethod
```

### Comparing `dymos-1.7.0/dymos/examples/hyper_sensitive/doc/test_doc_hyper_sensitive.py` & `dymos-1.8.0/dymos/examples/hyper_sensitive/doc/test_doc_hyper_sensitive.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/hyper_sensitive/hyper_sensitive_ode.py` & `dymos-1.8.0/dymos/examples/hyper_sensitive/hyper_sensitive_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/hyper_sensitive/test/test_hyper_sensitive.py` & `dymos-1.8.0/dymos/examples/hyper_sensitive/test/test_hyper_sensitive.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/length_constrained_brachistochrone/arc_length_comp.py` & `dymos-1.8.0/dymos/examples/length_constrained_brachistochrone/arc_length_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/length_constrained_brachistochrone/doc/test_doc_length_constrained_brachistochrone.py` & `dymos-1.8.0/dymos/examples/length_constrained_brachistochrone/doc/test_doc_length_constrained_brachistochrone.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/aero.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/aero.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/cd0_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/cd0_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/cd_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/cd_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/cl_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/cl_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/cla_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/cla_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/dynamic_pressure_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/dynamic_pressure_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/kappa_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/kappa_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/lift_drag_force_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/lift_drag_force_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/mach_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/mach_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/test/test_aerodynamics.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/test/test_aerodynamics.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/test/test_cd0_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/test/test_cd0_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/test/test_cla_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/test/test_cla_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/aero/test/test_kappa_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/aero/test/test_kappa_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/doc/aero_partial_coloring.py` & `dymos-1.8.0/dymos/examples/min_time_climb/doc/aero_partial_coloring.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/doc/dynamic_pressure_comp_partial_coloring.py` & `dymos-1.8.0/dymos/examples/min_time_climb/doc/dynamic_pressure_comp_partial_coloring.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/doc/min_time_climb_ode_partial_coloring.py` & `dymos-1.8.0/dymos/examples/min_time_climb/doc/min_time_climb_ode_partial_coloring.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/min_time_climb_ode.py` & `dymos-1.8.0/dymos/examples/min_time_climb/min_time_climb_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/prop/max_thrust_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/prop/max_thrust_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/prop/mdot_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/prop/mdot_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/prop/prop.py` & `dymos-1.8.0/dymos/examples/min_time_climb/prop/prop.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/prop/test/test_max_thrust_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/prop/test/test_max_thrust_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/prop/thrust_comp.py` & `dymos-1.8.0/dymos/examples/min_time_climb/prop/thrust_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/test/test_doc_min_time_climb_partial_coloring.py` & `dymos-1.8.0/dymos/examples/min_time_climb/test/test_doc_min_time_climb_partial_coloring.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/test/test_ex_min_time_climb.py` & `dymos-1.8.0/dymos/examples/min_time_climb/test/test_ex_min_time_climb.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/test/test_min_time_climb_simulate_failure.py` & `dymos-1.8.0/dymos/examples/min_time_climb/test/test_min_time_climb_simulate_failure.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/min_time_climb/test/test_refine_with_shaped_parameter.py` & `dymos-1.8.0/dymos/examples/min_time_climb/test/test_refine_with_shaped_parameter.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/oscillator/oscillator_ode.py` & `dymos-1.8.0/dymos/examples/oscillator/oscillator_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/oscillator/test/test_oscillator.py` & `dymos-1.8.0/dymos/examples/oscillator/test/test_oscillator.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/plotting.py` & `dymos-1.8.0/dymos/examples/plotting.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/Track.py` & `dymos-1.8.0/dymos/examples/racecar/Track.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/accelerationODE.py` & `dymos-1.8.0/dymos/examples/racecar/accelerationODE.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/carODE.py` & `dymos-1.8.0/dymos/examples/racecar/carODE.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/combinedODE.py` & `dymos-1.8.0/dymos/examples/racecar/combinedODE.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/curvature.py` & `dymos-1.8.0/dymos/examples/racecar/curvature.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/linewidthhelper.py` & `dymos-1.8.0/dymos/examples/racecar/linewidthhelper.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/normalForceODE.py` & `dymos-1.8.0/dymos/examples/racecar/normalForceODE.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/spline.py` & `dymos-1.8.0/dymos/examples/racecar/spline.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/test/test_racecar.py` & `dymos-1.8.0/dymos/examples/racecar/test/test_racecar.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/timeAdder.py` & `dymos-1.8.0/dymos/examples/racecar/timeAdder.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/timeODE.py` & `dymos-1.8.0/dymos/examples/racecar/timeODE.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/tireConstraintODE.py` & `dymos-1.8.0/dymos/examples/racecar/tireConstraintODE.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/tireODE.py` & `dymos-1.8.0/dymos/examples/racecar/tireODE.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/racecar/tracks.py` & `dymos-1.8.0/dymos/examples/racecar/tracks.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/robertson_problem/doc/robertson_ode.py` & `dymos-1.8.0/dymos/examples/robertson_problem/doc/robertson_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/robertson_problem/doc/test_doc_robertson_problem.py` & `dymos-1.8.0/dymos/examples/robertson_problem/doc/test_doc_robertson_problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import matplotlib
 import matplotlib.pyplot as plt
 
 from openmdao.utils.testing_utils import use_tempdirs
 from dymos.examples.robertson_problem.doc.robertson_ode import RobertsonODE
 
 
-# matplotlib.use('Agg')
+matplotlib.use('Agg')
 plt.style.use('ggplot')
 
 
 @use_tempdirs
 class TestRobertsonProblemForDocs(unittest.TestCase):
 
     def robertson_problem(self, t_final=1.0):
@@ -49,17 +49,17 @@
 
         #
         # Set the initial values
         #
         p['traj.phase0.t_initial'] = 0.0
         p['traj.phase0.t_duration'] = t_final
 
-        p.set_val('traj.phase0.states:x0', phase.interp('x0', ys=[1.0, 0.7]))
-        p.set_val('traj.phase0.states:y0', phase.interp('y0', ys=[0.0, 1e-5]))
-        p.set_val('traj.phase0.states:z0', phase.interp('z0', ys=[0.0, 0.3]))
+        p.set_val('traj.phase0.initial_states:x0', phase.interp('x0', ys=[1.0, 0.7]))
+        p.set_val('traj.phase0.initial_states:y0', phase.interp('y0', ys=[0.0, 1e-5]))
+        p.set_val('traj.phase0.initial_states:z0', phase.interp('z0', ys=[0.0, 0.3]))
 
         return p
 
     def test_robertson_problem_for_docs(self):
 
         import openmdao.api as om
         from dymos.utils.testing_utils import assert_check_partials
```

### Comparing `dymos-1.7.0/dymos/examples/robot_arm/doc/test_doc_robot_arm.py` & `dymos-1.8.0/dymos/examples/robot_arm/doc/test_doc_robot_arm.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/robot_arm/robot_arm_ode.py` & `dymos-1.8.0/dymos/examples/robot_arm/robot_arm_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/robot_arm/test/test_robot_arm.py` & `dymos-1.8.0/dymos/examples/robot_arm/test/test_robot_arm.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/shuttle_reentry/aerodynamics_comp.py` & `dymos-1.8.0/dymos/examples/shuttle_reentry/aerodynamics_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/shuttle_reentry/atmosphere_comp.py` & `dymos-1.8.0/dymos/examples/shuttle_reentry/atmosphere_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/shuttle_reentry/doc/test_doc_reentry.py` & `dymos-1.8.0/dymos/examples/shuttle_reentry/doc/test_doc_reentry.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/shuttle_reentry/flight_dynamics_comp.py` & `dymos-1.8.0/dymos/examples/shuttle_reentry/flight_dynamics_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/shuttle_reentry/heating_comp.py` & `dymos-1.8.0/dymos/examples/shuttle_reentry/heating_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/shuttle_reentry/shuttle_ode.py` & `dymos-1.8.0/dymos/examples/shuttle_reentry/shuttle_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/shuttle_reentry/test/test_reentry.py` & `dymos-1.8.0/dymos/examples/shuttle_reentry/test/test_reentry.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/ssto/doc/test_doc_ssto_earth.py` & `dymos-1.8.0/dymos/examples/ssto/doc/test_doc_ssto_earth.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/ssto/doc/test_doc_ssto_linear_tangent_guidance.py` & `dymos-1.8.0/dymos/examples/ssto/doc/test_doc_ssto_linear_tangent_guidance.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/ssto/doc/test_doc_ssto_polynomial_control.py` & `dymos-1.8.0/dymos/examples/ssto/doc/test_doc_ssto_polynomial_control.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/ssto/launch_vehicle_ode.py` & `dymos-1.8.0/dymos/examples/ssto/launch_vehicle_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/ssto/test/test_simulate_root_trajectory.py` & `dymos-1.8.0/dymos/examples/ssto/test/test_simulate_root_trajectory.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/vanderpol/doc/test_doc_vanderpol.py` & `dymos-1.8.0/dymos/examples/vanderpol/doc/test_doc_vanderpol.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/vanderpol/test/test_vanderpol.py` & `dymos-1.8.0/dymos/examples/vanderpol/test/test_vanderpol.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/vanderpol/vanderpol_dymos.py` & `dymos-1.8.0/dymos/examples/vanderpol/vanderpol_dymos.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/vanderpol/vanderpol_ode.py` & `dymos-1.8.0/dymos/examples/vanderpol/vanderpol_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/water_rocket/phases.py` & `dymos-1.8.0/dymos/examples/water_rocket/phases.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/water_rocket/test/test_water_rocket.py` & `dymos-1.8.0/dymos/examples/water_rocket/test/test_water_rocket.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/water_rocket/water_engine_comp.py` & `dymos-1.8.0/dymos/examples/water_rocket/water_engine_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/examples/water_rocket/water_propulsion_ode.py` & `dymos-1.8.0/dymos/examples/water_rocket/water_propulsion_ode.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/grid_refinement/error_estimation.py` & `dymos-1.8.0/dymos/grid_refinement/error_estimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     # Set the values in the refinement problem using the outputs from the first
     ode = p_refine.model.grid_refinement_system.ode
 
     t_name = phase.time_options['name']
     t_phase_name = f'{t_name}_phase'
 
     t_prev = phase.get_val(f'timeseries.{t_name}', units=phase.time_options['units'])
-    t_phase_prev = phase.get_val(f'timeseries.{t_phase_name}', units=phase.time_options['units'])
+    t_phase_prev = t_prev - t_prev[0]
     t_initial = np.repeat(t_prev[0, 0], repeats=transcription.grid_data.num_nodes, axis=0)
     t_duration = np.repeat(t_prev[-1, 0], repeats=transcription.grid_data.num_nodes, axis=0)
     t = np.dot(L, t_prev)
     t_phase = np.dot(L, t_phase_prev)
     targets = get_targets(ode, 'time', phase.time_options['targets'])
     t_phase_targets = get_targets(ode, 't_phase', phase.time_options['time_phase_targets'])
     t_initial_targets = get_targets(ode, 't_initial', phase.time_options['t_initial_targets'])
@@ -179,22 +179,22 @@
         rate2_targets = get_targets(ode, f'{name}_rate12', options['rate2_targets'])
 
         u_prev = phase.get_val(f'timeseries.controls:{name}', units=options['units'])
         u[name] = np.dot(L, u_prev)
         if targets:
             p_refine.set_val(f'controls:{name}', u[name])
 
-        u_rate_prev = phase.get_val(f'timeseries.control_rates:{name}_rate')
-        u_rate[name] = np.dot(L, u_rate_prev)
         if rate_targets:
+            u_rate_prev = phase.get_val(f'timeseries.control_rates:{name}_rate')
+            u_rate[name] = np.dot(L, u_rate_prev)
             p_refine.set_val(f'control_rates:{name}_rate', u_rate[name])
 
-        u_rate2_prev = phase.get_val(f'timeseries.control_rates:{name}_rate2')
-        u_rate2[name] = np.dot(L, u_rate2_prev)
         if rate2_targets:
+            u_rate2_prev = phase.get_val(f'timeseries.control_rates:{name}_rate2')
+            u_rate2[name] = np.dot(L, u_rate2_prev)
             p_refine.set_val(f'control_rates:{name}_rate2', u_rate2[name])
 
     for name, options in phase.polynomial_control_options.items():
         targets = get_targets(ode, name, options['targets'])
         rate_targets = get_targets(ode, f'{name}_rate', options['rate_targets'])
         rate2_targets = get_targets(ode, f'{name}_rate2', options['rate2_targets'])
 
@@ -213,15 +213,15 @@
         if rate2_targets:
             p_refine.set_val(f'polynomial_control_rates:{name}_rate2', p_rate2[name])
 
     # Configure the parameters
     for name, options in phase.parameter_options.items():
         targets = get_targets(ode, name, options['targets'])
         # The value of the parameter at one node
-        param[name] = phase.get_val(f'timeseries.parameters:{name}', units=options['units'])[0, ...]
+        param[name] = phase.get_val(f'parameter_vals:{name}', units=options['units'])[0, ...]
         if targets:
             p_refine.set_val(f'parameters:{name}', param[name], units=options['units'])
 
     # Execute the model
     p_refine.run_model()
 
     # Assign the state rates on the new grid to f
```

### Comparing `dymos-1.7.0/dymos/grid_refinement/grid_refinement_ode_system.py` & `dymos-1.8.0/dymos/grid_refinement/grid_refinement_ode_system.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/grid_refinement/hp_adaptive/hp_adaptive.py` & `dymos-1.8.0/dymos/grid_refinement/hp_adaptive/hp_adaptive.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/grid_refinement/ph_adaptive/ph_adaptive.py` & `dymos-1.8.0/dymos/grid_refinement/ph_adaptive/ph_adaptive.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/grid_refinement/refinement.py` & `dymos-1.8.0/dymos/grid_refinement/refinement.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/grid_refinement/write_iteration.py` & `dymos-1.8.0/dymos/grid_refinement/write_iteration.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/load_case.py` & `dymos-1.8.0/dymos/load_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,16 @@
             problem.set_val(f'{traj.pathname}.parameters:{param_name}', prev_val[0, ...], units=prev_units)
 
     for phase_abs_path, phase in phase_paths.items():
         phase_name = phase_abs_path.rpartition('.')[-1]
 
         # Get the initial time and duration from the previous result and set them into the new phase.
         try:
-            prev_time_path = [s for s in prev_vars if s.endswith(f'{phase_name}.timeseries.time')][0]
+            integration_name = phase.time_options['name']
+            prev_time_path = [s for s in prev_vars if s.endswith(f'{phase_name}.timeseries.{integration_name}')][0]
         except IndexError as e:
             continue
 
         prev_time_val = prev_vars[prev_time_path]['val']
         prev_time_val, unique_idxs = np.unique(prev_time_val, return_index=True)
         prev_time_units = prev_vars[prev_time_path]['units']
```

### Comparing `dymos-1.7.0/dymos/models/atmosphere/atmos_1976.py` & `dymos-1.8.0/dymos/models/atmosphere/atmos_1976.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/models/atmosphere/test/test_atmos.py` & `dymos-1.8.0/dymos/models/atmosphere/test/test_atmos.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/models/eom/flight_path_eom_2d.py` & `dymos-1.8.0/dymos/models/eom/flight_path_eom_2d.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/models/eom/test/test_flight_path_eom_2d.py` & `dymos-1.8.0/dymos/models/eom/test/test_flight_path_eom_2d.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/options.py` & `dymos-1.8.0/dymos/_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,12 +7,16 @@
 
 _env_check_partials = os.environ.get('DYMOS_CHECK_PARTIALS', '0')
 _icp_default = _env_check_partials.lower() in ('1', 'yes', 'true')
 
 options.declare('include_check_partials', default=_icp_default, types=bool,
                 desc='If True, include dymos components when checking partials.')
 
-options.declare('plots', default='matplotlib', values=['matplotlib', 'bokeh'],
+options.declare('plots', default='bokeh', values=['matplotlib', 'bokeh'],
                 desc='The plot library used to generate output plots for Dymos.')
 
 options.declare('notebook_mode', default=False, types=bool,
                 desc='If True, provide notebook-enhanced plots and outputs.')
+
+options.declare('use_timeseries_prefix', default=True, types=bool,
+                desc='If True, prefix timeseries outputs with the variable type for states, times, controls,'
+                     'and parameters.')
```

### Comparing `dymos-1.7.0/dymos/phase/analytic_phase.py` & `dymos-1.8.0/dymos/phase/analytic_phase.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/options.py` & `dymos-1.8.0/dymos/phase/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
                           'option is invalid if opt=False.')
 
         self.declare(name='ref', types=(Iterable, Number), default=None,
                      allow_none=True,
                      desc='The unit-reference value of the parameter. This '
                           'option is invalid if opt=False.')
 
-        self.declare(name='include_timeseries', types=bool, default=True,
+        self.declare(name='include_timeseries', types=bool, default=False,
                      desc='True if the static parameters should be included in output timeseries, else False')
 
 
 class TrajParameterOptionsDictionary(ParameterOptionsDictionary):
     """
     An OptionsDictionary specific to trajectory design parameters.
 
@@ -735,7 +735,29 @@
                      desc='If True this is a rate.')
 
         self.declare(name='is_expr', default=False, allow_none=False,
                      desc='If true the requested timeseries is a mathematical expression')
 
         self.declare(name='expr_kwargs', default={}, allow_none=False,
                      desc='Options to be passed to the timeseries expression comp when adding the expression.')
+
+
+class PhaseTimeseriesOptionsDictionary(om.OptionsDictionary):
+    """
+    An OptionsDictionary for phase options related to timeseries.
+
+    Parameters
+    ----------
+    read_only : bool
+        If True, setting (via __setitem__ or update) is not permitted.
+    """
+    def __init__(self, read_only=False):
+        super().__init__(read_only)
+
+        self.declare(name='include_state_rates', types=bool, default=True,
+                     desc='If True, include state rates in the timeseries outputs by default.')
+
+        self.declare(name='include_control_rates', types=bool, default=True,
+                     desc='If True, include control rates in the timeseries outputs by default.')
+
+        self.declare(name='include_t_phase', types=bool, default=True,
+                     desc='If True, include the elapsed phase time in the timeseries outputs by default.')
```

### Comparing `dymos-1.7.0/dymos/phase/phase.py` & `dymos-1.8.0/dymos/phase/phase.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from openmdao.utils.mpi import MPI
 from openmdao.core.system import System
 import dymos as dm
 
 from .options import ControlOptionsDictionary, ParameterOptionsDictionary, \
     StateOptionsDictionary, TimeOptionsDictionary, ConstraintOptionsDictionary, \
     PolynomialControlOptionsDictionary, GridRefinementOptionsDictionary, SimulateOptionsDictionary, \
-    TimeseriesOutputOptionsDictionary
+    TimeseriesOutputOptionsDictionary, PhaseTimeseriesOptionsDictionary
 
 from ..transcriptions.transcription_base import TranscriptionBase
 from ..transcriptions.grid_data import GaussLobattoGrid, RadauGrid, UniformGrid
 from ..transcriptions import ExplicitShooting, GaussLobatto, Radau
 from ..utils.indexing import get_constraint_flat_idxs
 from ..utils.introspection import configure_time_introspection, _configure_constraint_introspection, \
     configure_controls_introspection, configure_parameters_introspection, \
@@ -64,14 +64,15 @@
         self.state_options = {}
         self.control_options = {}
         self.polynomial_control_options = {}
         self.parameter_options = {}
         self.refine_options = GridRefinementOptionsDictionary()
         self.simulate_options = SimulateOptionsDictionary()
         self.timeseries_ec_vars = {}
+        self.timeseries_options = PhaseTimeseriesOptionsDictionary()
 
         # Dictionaries of variable options that are set by the user via the API
         # These will be applied over any defaults specified by decorators on the ODE
         if from_phase is None:
             self._initial_boundary_constraints = []
             self._final_boundary_constraints = []
             self._path_constraints = []
@@ -1446,23 +1447,24 @@
         -------
         str or None
            Name of output that was added to the timeseries or None if nothing was added.
         """
         if timeseries not in self._timeseries:
             raise ValueError(f'Timeseries {timeseries} does not exist in phase {self.pathname}')
 
-        if expr:
-            output_name = name.split('=')[0].strip()
-        elif '*' in name:
-            output_name = name
-        elif output_name is None:
-            output_name = name.rpartition('.')[-1]
+        if output_name is None:
+            if expr:
+                output_name = name.split('=')[0].strip()
+            elif '*' in name:
+                output_name = name
+            elif output_name is None:
+                output_name = name.rpartition('.')[-1]
 
-        if rate:
-            output_name = output_name + '_rate'
+            if rate:
+                output_name = output_name + '_rate'
 
         if output_name not in self._timeseries[timeseries]['outputs']:
             ts_output = TimeseriesOutputOptionsDictionary()
             ts_output['name'] = name
             ts_output['output_name'] = output_name
             ts_output['wildcard_units'] = {}
             ts_output['units'] = units
```

### Comparing `dymos-1.7.0/dymos/phase/simulation_phase.py` & `dymos-1.8.0/dymos/phase/simulation_phase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from openmdao.utils.mpi import MPI
 
 from .phase import Phase
+from .._options import options as dymos_options
 from ..transcriptions.grid_data import GaussLobattoGrid, RadauGrid, UniformGrid
 from ..transcriptions import ExplicitShooting, GaussLobatto, Radau
 
 from ..utils.misc import _unspecified
 
 
 class SimulationPhase(Phase):
@@ -106,15 +107,15 @@
         self.set_val('t_initial', t_initial, units=self.time_options['units'])
 
         t_duration = from_phase.get_val('t_duration', units=self.time_options['units'])
         self.set_val('t_duration', t_duration, units=self.time_options['units'])
 
         for name, options in self.state_options.items():
             val = from_phase.get_val(f'states:{name}', units=options['units'])[0, ...]
-            self.set_val(f'states:{name}', val, units=options['units'])
+            self.set_val(f'initial_states:{name}', val, units=options['units'])
 
         for name, options in self.parameter_options.items():
             val = from_phase.get_val(f'parameters:{name}', units=options['units'])
             self.set_val(f'parameters:{name}', val, units=options['units'])
 
         for name, options in self.control_options.items():
             val = from_phase.get_val(f'controls:{name}', units=options['units'])
@@ -157,16 +158,17 @@
         time_name = phs.time_options['name']
         op = op_dict[f'timeseries.timeseries_comp.{time_name}']
         prob.set_val(f'{self_path}t_initial', op['val'][0, ...])
         prob.set_val(f'{self_path}t_duration', op['val'][-1, ...] - op['val'][0, ...])
 
         # Assign initial state values
         for name in phs.state_options:
-            op = op_dict[f'timeseries.timeseries_comp.states:{name}']
-            prob[f'{self_path}states:{name}'][...] = op['val'][0, ...]
+            prefix = 'states:' if dymos_options['use_timeseries_prefix'] else ''
+            op = op_dict[f'timeseries.timeseries_comp.{prefix}{name}']
+            prob[f'{self_path}initial_states:{name}'][...] = op['val'][0, ...]
 
         # Assign control values
         for name, options in phs.control_options.items():
             ip = ip_dict[f'control_group.control_interp_comp.controls:{name}']
             prob[f'{self_path}controls:{name}'][...] = ip['val']
 
         # Assign polynomial control values
```

### Comparing `dymos-1.7.0/dymos/phase/test/test_add_boundary_constraint.py` & `dymos-1.8.0/dymos/phase/test/test_add_boundary_constraint.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/test/test_add_parameter_types.py` & `dymos-1.8.0/dymos/phase/test/test_add_parameter_types.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/test/test_add_path_constraint.py` & `dymos-1.8.0/dymos/phase/test/test_add_path_constraint.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/test/test_analytic_phase.py` & `dymos-1.8.0/dymos/phase/test/test_analytic_phase.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         p.set_val('traj.phase.t_initial', 0.0, units='s')
         p.set_val('traj.phase.t_duration', 2.0, units='s')
         p.set_val('traj.phase.parameters:y0', 0.5, units='unitless')
 
         p.run_model()
 
         y = p.get_val('traj.phase.timeseries.states:y', units='unitless')
-        y0 = p.get_val('traj.phase.timeseries.parameters:y0', units='unitless')
+        y0 = p.get_val('traj.phase.parameter_vals:y0', units='unitless')
 
         expected_z = y0 + y**2
         z = p.get_val('traj.phase.timeseries.z')
 
         assert_near_equal(z, expected_z)
```

### Comparing `dymos-1.7.0/dymos/phase/test/test_input_parameter_connections.py` & `dymos-1.8.0/dymos/phase/test/test_input_parameter_connections.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/test/test_interp.py` & `dymos-1.8.0/dymos/phase/test/test_interp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/test/test_phase.py` & `dymos-1.8.0/dymos/phase/test/test_phase.py`

 * *Files 6% similar despite different names*

```diff
@@ -599,27 +599,32 @@
 
                 p.model.linear_solver = om.DirectSolver()
                 p.setup(check=True)
 
                 p['phase0.t_initial'] = 0.0
                 p['phase0.t_duration'] = 2.0
 
-                p['phase0.states:x'] = phase.interp('x', [0, 10])
-                p['phase0.states:y'] = phase.interp('y', [10, 5])
-                p['phase0.states:v'] = phase.interp('v', [0, 9.9])
+                if txname == 'explicit-shooting':
+                    p['phase0.initial_states:x'] = 0
+                    p['phase0.initial_states:y'] = 10
+                    p['phase0.initial_states:v'] = 0
+                else:
+                    p['phase0.states:x'] = phase.interp('x', [0, 10])
+                    p['phase0.states:y'] = phase.interp('y', [10, 5])
+                    p['phase0.states:v'] = phase.interp('v', [0, 9.9])
                 p['phase0.controls:theta'] = phase.interp('theta', [5, 100])
                 p['phase0.parameters:g'] = 5
 
                 p.run_driver()
 
                 assert_near_equal(p.get_val('phase0.timeseries.time')[-1], 1.8016,
                                   tolerance=1.0E-4)
-                assert_near_equal(p.get_val('phase0.timeseries.parameters:g')[0], 9.80665,
+                assert_near_equal(p.get_val('phase0.parameter_vals:g')[0], 9.80665,
                                   tolerance=1.0E-6)
-                assert_near_equal(p.get_val('phase0.timeseries.parameters:g')[-1], 9.80665,
+                assert_near_equal(p.get_val('phase0.parameter_vals:g')[-1], 9.80665,
                                   tolerance=1.0E-6)
 
     def test_parameter_final_boundary_constraint(self):
 
         transcriptions = {'gauss-lobatto': dm.GaussLobatto,
                           'radau-ps': dm.Radau,
                           'explicit-shooting': dm.ExplicitShooting}
@@ -667,27 +672,32 @@
 
                 p.model.linear_solver = om.DirectSolver()
                 p.setup(check=True)
 
                 p['phase0.t_initial'] = 0.0
                 p['phase0.t_duration'] = 2.0
 
-                p['phase0.states:x'] = phase.interp('x', [0, 10])
-                p['phase0.states:y'] = phase.interp('y', [10, 5])
-                p['phase0.states:v'] = phase.interp('v', [0, 9.9])
+                if txname == 'explicit-shooting':
+                    p['phase0.initial_states:x'] = 0
+                    p['phase0.initial_states:y'] = 10
+                    p['phase0.initial_states:v'] = 0
+                else:
+                    p['phase0.states:x'] = phase.interp('x', [0, 10])
+                    p['phase0.states:y'] = phase.interp('y', [10, 5])
+                    p['phase0.states:v'] = phase.interp('v', [0, 9.9])
                 p['phase0.controls:theta'] = phase.interp('theta', [5, 100])
                 p['phase0.parameters:g'] = 5
 
                 p.run_driver()
 
                 assert_near_equal(p.get_val('phase0.timeseries.time')[-1], 1.8016,
                                   tolerance=1.0E-4)
-                assert_near_equal(p.get_val('phase0.timeseries.parameters:g')[0], 9.80665,
+                assert_near_equal(p.get_val('phase0.parameter_vals:g')[0], 9.80665,
                                   tolerance=1.0E-6)
-                assert_near_equal(p.get_val('phase0.timeseries.parameters:g')[-1], 9.80665,
+                assert_near_equal(p.get_val('phase0.parameter_vals:g')[-1], 9.80665,
                                   tolerance=1.0E-6)
 
     def test_parameter_path_constraint(self):
 
         transcriptions = {'gauss-lobatto': dm.GaussLobatto,
                           'radau-ps': dm.Radau,
                           'explicit-shooting': dm.ExplicitShooting}
@@ -734,25 +744,30 @@
 
                 p.model.linear_solver = om.DirectSolver()
                 p.setup(check=True)
 
                 p['phase0.t_initial'] = 0.0
                 p['phase0.t_duration'] = 2.0
 
-                p['phase0.states:x'] = phase.interp('x', [0, 10])
-                p['phase0.states:y'] = phase.interp('y', [10, 5])
-                p['phase0.states:v'] = phase.interp('v', [0, 9.9])
+                if txname == 'explicit-shooting':
+                    p['phase0.initial_states:x'] = 0
+                    p['phase0.initial_states:y'] = 10
+                    p['phase0.initial_states:v'] = 0
+                else:
+                    p['phase0.states:x'] = phase.interp('x', [0, 10])
+                    p['phase0.states:y'] = phase.interp('y', [10, 5])
+                    p['phase0.states:v'] = phase.interp('v', [0, 9.9])
                 p['phase0.controls:theta'] = phase.interp('theta', [5, 100])
                 p['phase0.parameters:g'] = 5
 
                 p.run_driver()
 
                 assert_near_equal(p.get_val('phase0.timeseries.time')[-1], 1.8016,
                                   tolerance=1.0E-4)
-                assert_near_equal(p.get_val('phase0.timeseries.parameters:g')[0], 9.80665,
+                assert_near_equal(p.get_val('phase0.parameter_vals:g')[0], 9.80665,
                                   tolerance=1.0E-6)
-                assert_near_equal(p.get_val('phase0.timeseries.parameters:g')[-1], 9.80665,
+                assert_near_equal(p.get_val('phase0.parameter_vals:g')[-1], 9.80665,
                                   tolerance=1.0E-6)
 
 
 if __name__ == '__main__':  # pragma: no cover
     unittest.main()
```

### Comparing `dymos-1.7.0/dymos/phase/test/test_set_time_options.py` & `dymos-1.8.0/dymos/phase/test/test_set_time_options.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/test/test_simulate.py` & `dymos-1.8.0/dymos/phase/test/test_simulate.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/test/test_sized_input_parameters.py` & `dymos-1.8.0/dymos/phase/test/test_sized_input_parameters.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/test/test_state_discovery.py` & `dymos-1.8.0/dymos/phase/test/test_state_discovery.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/test/test_time_targets.py` & `dymos-1.8.0/dymos/phase/test/test_time_targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         p.driver = om.ScipyOptimizeDriver()
 
         # Compute sparsity/coloring when run_driver is called
         p.driver.declare_coloring()
 
         t = {'gauss-lobatto': dm.GaussLobatto(num_segments=num_seg, order=transcription_order),
              'radau-ps': dm.Radau(num_segments=num_seg, order=transcription_order),
-             'explicit-shooting': dm.ExplicitShooting(num_segments=num_seg, grid='radau-ps', num_steps_per_segment=10)}
+             'explicit-shooting': dm.ExplicitShooting(num_segments=num_seg, grid='radau-ps')}
 
         phase = dm.Phase(ode_class=_BrachistochroneTestODE, transcription=t[transcription])
 
         p.model.add_subsystem('phase0', phase)
 
         phase.set_time_options(initial_bounds=(1, 1), duration_bounds=(.5, 10), units='s',
                                time_phase_targets=['time_phase'], t_duration_targets=['t_duration'],
@@ -124,30 +124,37 @@
         phase.add_control('theta', units='deg', rate_continuity=True, lower=0.01, upper=179.9, targets=['theta'])
 
         phase.add_parameter('g', units='m/s**2', opt=False, val=9.80665, targets=['g'])
 
         phase.add_boundary_constraint('x', loc='final', equals=10)
         phase.add_boundary_constraint('y', loc='final', equals=5)
 
+        phase.timeseries_options['include_t_phase'] = True
+
         # Minimize time at the end of the phase
         phase.add_objective(time_name, loc='final', scaler=10)
 
         p.model.linear_solver = om.DirectSolver()
 
         if input_duration:
             p.model.add_design_var('phase0.t_duration', lower=0, upper=3, scaler=1.0)
 
         p.setup(check=True)
 
         p['phase0.t_initial'] = 1.0
         p['phase0.t_duration'] = 5.0
 
-        p['phase0.states:x'] = phase.interp('x', [0, 10])
-        p['phase0.states:y'] = phase.interp('y', [10, 5])
-        p['phase0.states:v'] = phase.interp('v', [0, 9.9])
+        if transcription == 'explicit-shooting':
+            p['phase0.initial_states:x'] = 0
+            p['phase0.initial_states:y'] = 10
+            p['phase0.initial_states:v'] = 0
+        else:
+            p['phase0.states:x'] = phase.interp('x', [0, 10])
+            p['phase0.states:y'] = phase.interp('y', [10, 5])
+            p['phase0.states:v'] = phase.interp('v', [0, 9.9])
         p['phase0.controls:theta'] = phase.interp('theta', [5, 100.5])
 
         return p
 
     def test_gauss_lobatto(self):
         num_seg = 20
```

### Comparing `dymos-1.7.0/dymos/phase/test/test_time_units.py` & `dymos-1.8.0/dymos/phase/test/test_time_units.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/phase/test/test_timeseries.py` & `dymos-1.8.0/dymos/phase/test/test_timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 
         phase.add_state('v', fix_initial=True, fix_final=False)
 
         phase.add_control('theta', continuity=True, rate_continuity=True, opt=True,
                           units='deg', lower=0.01, upper=179.9, ref=1, ref0=0)
 
         if test_smaller_timeseries:
-            phase.add_parameter('g', opt=True, units='m/s**2', val=9.80665, include_timeseries=False)
-        else:
             phase.add_parameter('g', opt=True, units='m/s**2', val=9.80665)
+        else:
+            phase.add_parameter('g', opt=True, units='m/s**2', val=9.80665, include_timeseries=True)
 
         # Minimize time at the end of the phase
         phase.add_objective('time_phase', loc='final', scaler=10)
 
         p.model.linear_solver = om.DirectSolver()
         p.setup(check=True)
 
@@ -90,54 +90,57 @@
 
         for dp in ('g',):
             for i in range(gd.subset_num_nodes['all']):
                 if test_smaller_timeseries:
                     with self.assertRaises(KeyError):
                         p.get_val(f'phase0.timeseries.parameters:{dp}')
                 else:
-                    assert_near_equal(p.get_val(f'phase0.parameters:{dp}')[0],
+                    assert_near_equal(p.get_val(f'phase0.parameter_vals:{dp}')[0],
                                       p.get_val(f'phase0.timeseries.parameters:{dp}')[i])
 
         # call simulate to test SolveIVP transcription
         exp_out = phase.simulate()
         if test_smaller_timeseries:
             with self.assertRaises(KeyError):
                 exp_out.get_val(f'phase0.timeseries.parameters:{dp}')
         else:  # no error accessing timseries.parameter
             exp_out.get_val(f'phase0.timeseries.parameters:{dp}')
 
     def test_timeseries_gl_smaller_timeseries(self):
         self.test_timeseries_gl(test_smaller_timeseries=True)
 
     def test_timeseries_radau(self, test_smaller_timeseries=False):
+
         p = om.Problem(model=om.Group())
 
         p.driver = om.ScipyOptimizeDriver()
         p.driver.declare_coloring()
 
         phase = dm.Phase(ode_class=BrachistochroneODE,
                          transcription=dm.Radau(num_segments=8, order=3, compressed=True))
 
+        phase.timeseries_options['include_state_rates'] = True
+
         p.model.add_subsystem('phase0', phase)
 
         phase.set_time_options(fix_initial=True, duration_bounds=(.5, 10))
 
         phase.add_state('x', fix_initial=True, fix_final=True)
 
         phase.add_state('y', fix_initial=True, fix_final=True)
 
         phase.add_state('v', fix_initial=True, fix_final=False)
 
         phase.add_control('theta', continuity=True, rate_continuity=True, opt=True,
                           units='deg', lower=0.01, upper=179.9, ref=1, ref0=0)
 
         if test_smaller_timeseries:
-            phase.add_parameter('g', opt=True, units='m/s**2', val=9.80665, include_timeseries=False)
-        else:
             phase.add_parameter('g', opt=True, units='m/s**2', val=9.80665)
+        else:
+            phase.add_parameter('g', opt=True, units='m/s**2', val=9.80665, include_timeseries=True)
 
         # Minimize time at the end of the phase
         phase.add_objective('time_phase', loc='final', scaler=10)
 
         p.model.options['assembled_jac_type'] = 'csc'
         p.model.linear_solver = om.DirectSolver()
         p.setup(check=True)
@@ -232,28 +235,25 @@
         phase.add_objective('time', loc='final')
 
         p.setup(force_alloc_complex=True)
 
         p['phase0.t_initial'] = 0.0
         p['phase0.t_duration'] = 2.0
 
-        p['phase0.states:x'] = phase.interp('x', [0, 10])
-        p['phase0.states:y'] = phase.interp('y', [10, 5])
-        p['phase0.states:v'] = phase.interp('v', [0, 9.9])
+        p['phase0.initial_states:x'] = 0
+        p['phase0.initial_states:y'] = 10
+        p['phase0.initial_states:v'] = 0
         p['phase0.controls:theta'] = phase.interp('theta', [5, 100])
         p['phase0.parameters:g'] = 9.80665
 
         p.run_driver()
 
         assert_near_equal(np.atleast_2d(p.get_val('phase0.t')).T,
                           p.get_val('phase0.timeseries.time'))
 
-        assert_near_equal(np.atleast_2d(p.get_val('phase0.t_phase')).T,
-                          p.get_val('phase0.timeseries.time_phase'))
-
         for state in ('x', 'y', 'v'):
             assert_near_equal(p.get_val(f'phase0.integrator.states_out:{state}'),
                               p.get_val(f'phase0.timeseries.states:{state}'))
 
         for control in ('theta',):
             assert_near_equal(p.get_val(f'phase0.control_values:{control}'),
                               p.get_val(f'phase0.timeseries.controls:{control}'))
@@ -443,17 +443,23 @@
         p.model.options['assembled_jac_type'] = 'csc'
         p.model.linear_solver = om.DirectSolver()
         p.setup(check=True)
 
         p['phase0.t_initial'] = 0.0
         p['phase0.t_duration'] = 2.0
 
-        p['phase0.states:x'] = phase.interp('x', [0, 10])
-        p['phase0.states:y'] = phase.interp('y', [10, 5])
-        p['phase0.states:v'] = phase.interp('v', [0, 9.9])
+        if isinstance(transcription, dm.ExplicitShooting):
+            p['phase0.initial_states:x'] = 0
+            p['phase0.initial_states:y'] = 10
+            p['phase0.initial_states:v'] = 0
+        else:
+            p['phase0.states:x'] = phase.interp('x', [0, 10])
+            p['phase0.states:y'] = phase.interp('y', [10, 5])
+            p['phase0.states:v'] = phase.interp('v', [0, 9.9])
+
         p[f'phase0.{control_name}'] = phase.interp('theta', [5, 100])
         p['phase0.parameters:g'] = 9.80665
         return p
 
     def test_invalid_expr_var(self):
         p = om.Problem(model=om.Group())
```

### Comparing `dymos-1.7.0/dymos/run_problem.py` & `dymos-1.8.0/dymos/run_problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 
 import openmdao.api as om
 from openmdao.recorders.case import Case
+from ._options import options as dymos_options
 from dymos.trajectory.trajectory import Trajectory
 from dymos.load_case import load_case
 from dymos.visualization.timeseries_plots import timeseries_plots
 
 from .grid_refinement.refinement import _refine_iter
 
 
@@ -14,14 +15,15 @@
                 solution_record_file='dymos_solution.db',
                 simulation_record_file='dymos_simulation.db',
                 make_plots=False,
                 plot_dir="plots",
                 case_prefix=None,
                 reset_iter_counts=True,
                 simulate_kwargs=None,
+                plot_kwargs=None,
                 ):
     """
     A Dymos-specific interface to execute an OpenMDAO problem containing Dymos Trajectories or
     Phases.  This function can iteratively call run_driver to perform grid refinement, and
     automatically call simulate following a run to check the validity of a result.
 
     Parameters
@@ -50,14 +52,16 @@
         Path to case recorder file use to store results from solution.
     simulation_record_file : str
         Path to case recorder file use to store results from simulation.
     plot_dir : str
         Name of the plot directory to be created.
     simulate_kwargs : dict
         A dictionary of argument: value pairs to be passed to simulate. These are ignored when simulate=False.
+    plot_kwargs : dict
+        A dictionary of argument: value pairs that are passed to `timeseries_plots`. Only used when make_plots=True.
     case_prefix : str or None
         Prefix to prepend to coordinates when recording.
     reset_iter_counts : bool
         If True and model has been run previously, reset all iteration counters.
     """
     if restart is not None:
         if isinstance(restart, str):
@@ -105,12 +109,18 @@
             raise ValueError('Key "case_prefix" was found in simulate_kwargs but should instead by provided by the '
                              'argument "case_prefix", not part of the simulate_kwargs dictionary.')
         for subsys in problem.model.system_iter(include_self=True, recurse=True):
             if isinstance(subsys, Trajectory):
                 subsys.simulate(record_file=simulation_record_file, case_prefix=case_prefix, **_simulate_kwargs)
 
     if make_plots:
-        _sim_record_file = None if not simulate else simulation_record_file
-        timeseries_plots(solution_record_file, simulation_record_file=_sim_record_file,
-                         plot_dir=plot_dir, problem=problem)
+        if dymos_options['plots'] == 'bokeh':
+            from dymos.visualization.timeseries.bokeh_timeseries_report import make_timeseries_report
+            make_timeseries_report(prob=problem, solution_record_file=solution_record_file,
+                                   simulation_record_file=simulation_record_file)
+        else:
+            _sim_record_file = None if not simulate else simulation_record_file
+            _plot_kwargs = plot_kwargs if plot_kwargs is not None else {}
+            timeseries_plots(solution_record_file, simulation_record_file=_sim_record_file,
+                             plot_dir=plot_dir, problem=problem, **_plot_kwargs)
 
     return failed
```

### Comparing `dymos-1.7.0/dymos/test/test_check_partials.py` & `dymos-1.8.0/dymos/test/test_check_partials.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 
         phase.add_objective('time', loc='final')
 
         prob.setup(force_alloc_complex=True)
 
         prob.set_val('phase0.t_initial', 0.0)
         prob.set_val('phase0.t_duration', 2)
-        prob.set_val('phase0.states:x', 0.0)
-        prob.set_val('phase0.states:y', 10.0)
-        prob.set_val('phase0.states:v', 1.0E-6)
+        prob.set_val('phase0.initial_states:x', 0.0)
+        prob.set_val('phase0.initial_states:y', 10.0)
+        prob.set_val('phase0.initial_states:v', 1.0E-6)
         prob.set_val('phase0.parameters:g', 1.0, units='m/s**2')
         prob.set_val('phase0.controls:theta', phase.interp('theta', ys=[0.01, 90]),
                      units='deg')
 
         prob.run_model()
 
         cpd = prob.check_partials(compact_print=True, method='fd', out_stream=None)
```

### Comparing `dymos-1.7.0/dymos/test/test_lint_docstrings.py` & `dymos-1.8.0/dymos/test/test_lint_docstrings.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/test/test_load_case.py` & `dymos-1.8.0/dymos/test/test_load_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         # Run the model to ensure we find the same output values as those that we recorded
         p.run_driver()
 
         inputs = dict([(o[0], o[1]) for o in case.list_inputs(units=True, shape=True, out_stream=None)])
 
         assert_near_equal(p['phase0.controls:theta'],
                           inputs['phase0.control_group.control_interp_comp.controls:theta']
-                          ['value'])
+                          ['val'])
 
     def test_load_case_unchanged_grid_polynomial_control(self):
         import openmdao.api as om
         from openmdao.utils.assert_utils import assert_near_equal
         import dymos as dm
 
         p = setup_problem(dm.GaussLobatto(num_segments=10), polynomial_control=True)
@@ -117,15 +117,15 @@
         # Run the model to ensure we find the same output values as those that we recorded
         p.run_driver()
 
         inputs = dict([(o[0], o[1]) for o in case.list_inputs(units=True, shape=True, out_stream=None)])
 
         assert_near_equal(p['phase0.polynomial_controls:theta'],
                           inputs['phase0.polynomial_control_group.interp_comp.polynomial_controls:theta']
-                          ['value'])
+                          ['val'])
 
     def test_load_case_lgl_to_radau(self):
         import openmdao.api as om
         from openmdao.utils.assert_utils import assert_near_equal
         import dymos as dm
 
         p = setup_problem(dm.GaussLobatto(num_segments=10))
```

### Comparing `dymos-1.7.0/dymos/test/test_options.py` & `dymos-1.8.0/dymos/test/test_options.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/test/test_pycodestyle.py` & `dymos-1.8.0/dymos/test/test_pycodestyle.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/test/test_run_problem.py` & `dymos-1.8.0/dymos/test/test_run_problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
         if optimizer == 'SNOPT':
             p.driver.opt_settings['Major iterations limit'] = 200
             p.driver.opt_settings['Major feasibility tolerance'] = 1.0E-6
             p.driver.opt_settings['Major optimality tolerance'] = 1.0E-6
         elif optimizer == 'IPOPT':
             p.driver.opt_settings['hessian_approximation'] = 'limited-memory'
-            # p.driver.opt_settings['nlp_scaling_method'] = 'user-scaling'
             p.driver.opt_settings['print_level'] = 0
             p.driver.opt_settings['max_iter'] = 200
             p.driver.opt_settings['linear_solver'] = 'mumps'
 
         traj = p.model.add_subsystem('traj', dm.Trajectory())
         phase0 = traj.add_phase('phase0', dm.Phase(ode_class=HyperSensitiveODE,
                                                    transcription=dm.Radau(num_segments=10,
@@ -389,15 +388,14 @@
         cr_opt = om.CaseReader('brach_driver_rec.db')
         cases = cr_opt.list_cases(source='driver', out_stream=None)
 
         for case in cases:
             self.assertTrue(case.startswith('hp_') and 'pyOptSparse_SLSQP|' in case, msg=f'Unexpected case: {case}')
 
     @require_pyoptsparse(optimizer='SLSQP')
-    @unittest.skip(reason='Skipped until the OpenMDAO issue of coloring changing the case_prefix is resolved.')
     def test_run_brachistochrone_problem_refine_case_prefix(self):
         p = om.Problem(model=om.Group())
         p.driver = om.pyOptSparseDriver()
         p.driver.declare_coloring()
         p.driver.options['optimizer'] = 'SLSQP'
 
         p.driver.add_recorder(om.SqliteRecorder('brach_driver_rec.db'))
@@ -657,14 +655,17 @@
         phase0.add_boundary_constraint('x', loc='final', equals=10)
         phase0.add_boundary_constraint('y', loc='final', equals=5)
         # Minimize time at the end of the phase
         phase0.add_objective('time_phase', loc='final', scaler=10)
 
         phase0.set_refine_options(refine=True)
 
+        phase0.timeseries_options['include_state_rates'] = True
+        phase0.timeseries_options['include_t_phase'] = True
+
         p.model.linear_solver = om.DirectSolver()
         p.setup(check=True)
 
         p.set_val('traj.phase0.t_initial', 0.0)
         p.set_val('traj.phase0.t_duration', 2.0)
 
         p.set_val('traj.phase0.states:x', phase0.interp('x', [0, 10]))
@@ -672,74 +673,93 @@
         p.set_val('traj.phase0.states:v', phase0.interp('v', [0, 9.9]))
         p.set_val('traj.phase0.controls:theta', phase0.interp('theta', [5, 100]))
         p.set_val('traj.phase0.parameters:g', 9.80665)
 
         self.p = p
 
     def test_run_brachistochrone_problem_make_plots(self):
+        plots_cache = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
         dm.run_problem(self.p, make_plots=True)
         plot_dir = pathlib.Path(_get_reports_dir(self.p)).joinpath('plots')
 
         for varname in ['time_phase', 'states:x', 'state_rates:x', 'states:y',
                         'state_rates:y', 'states:v',
                         'state_rates:v', 'controls:theta', 'control_rates:theta_rate',
-                        'control_rates:theta_rate2', 'parameters:g']:
-            self.assertTrue(plot_dir.joinpath(f'{varname.replace(":","_")}.png').exists())
+                        'control_rates:theta_rate2']:
+            self.assertTrue(plot_dir.joinpath(f'{varname.replace(":","_")}.png').exists(),
+                            msg=str(plot_dir.joinpath(f'{varname.replace(":","_")}.png')) + ' does not exist.')
+        dm.options['plots'] = plots_cache
 
     def test_run_brachistochrone_problem_make_plots_set_plot_dir(self):
+        _cache = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
+
         dm.run_problem(self.p, make_plots=True, plot_dir="test_plot_dir")
 
         plot_dir = pathlib.Path(_get_reports_dir(self.p))
-        for varname in ['time_phase', 'states:x', 'state_rates:x', 'states:y',
-                        'state_rates:y', 'states:v',
-                        'state_rates:v', 'controls:theta', 'control_rates:theta_rate',
-                        'control_rates:theta_rate2', 'parameters:g']:
-            self.assertTrue(plot_dir.joinpath('test_plot_dir', f'{varname.replace(":","_")}.png').exists())
+        for varname in ['states:x', 'states:y', 'states:v', 'controls:theta']:
+            plotfile = plot_dir.joinpath('test_plot_dir', f'{varname.replace(":","_")}.png')
+            self.assertTrue(plotfile.exists(), msg=str(plotfile) + ' does not exist.')
+
+        dm.options['plots'] = _cache
 
     def test_run_brachistochrone_problem_do_not_make_plots(self):
         dm.run_problem(self.p, make_plots=False)
         plot_dir = pathlib.Path(_get_reports_dir(self.p)).joinpath('plots')
 
         for varname in ['time_phase', 'states:x', 'state_rates:x', 'states:y',
                         'state_rates:y', 'states:v',
                         'state_rates:v', 'controls:theta', 'control_rates:theta_rate',
                         'control_rates:theta_rate2', 'parameters:g']:
-            self.assertFalse(plot_dir.joinpath(f'{varname.replace(":","_")}.png').exists())
+            plotfile = plot_dir.joinpath(f'{varname.replace(":","_")}.png')
+            self.assertFalse(plotfile.exists(), msg=f'Unexpectedly found plot file {plotfile}')
 
     def test_run_brachistochrone_problem_set_simulation_record_file(self):
         simulation_record_file = 'simulation_record_file.db'
         dm.run_problem(self.p, simulate=True, simulation_record_file=simulation_record_file)
 
         self.assertTrue(os.path.exists(simulation_record_file))
 
     def test_run_brachistochrone_problem_set_solution_record_file(self):
         solution_record_file = 'solution_record_file.db'
         dm.run_problem(self.p, solution_record_file=solution_record_file)
 
         self.assertTrue(os.path.exists(solution_record_file))
 
     def test_run_brachistochrone_problem_plot_simulation(self):
+        plots_cache = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
+
         dm.run_problem(self.p, make_plots=True, simulate=True)
         plot_dir = pathlib.Path(_get_reports_dir(self.p)).joinpath('plots')
 
         for varname in ['time_phase', 'states:x', 'state_rates:x', 'states:y',
                         'state_rates:y', 'states:v',
                         'state_rates:v', 'controls:theta', 'control_rates:theta_rate',
-                        'control_rates:theta_rate2', 'parameters:g']:
-            self.assertTrue(plot_dir.joinpath(f'{varname.replace(":","_")}.png').exists())
+                        'control_rates:theta_rate2']:
+            plotfile = plot_dir.joinpath(f'{varname.replace(":","_")}.png')
+            self.assertTrue(plotfile.exists(), msg=f'plot file {plotfile} does not exist!')
+        dm.options['plots'] = plots_cache
 
     def test_run_brachistochrone_problem_plot_no_simulation_record_file_given(self):
+        plots_cache = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
+
         dm.run_problem(self.p, make_plots=True, simulate=True)
         plot_dir = pathlib.Path(_get_reports_dir(self.p)).joinpath('plots')
 
         for varname in ['time_phase', 'states:x', 'state_rates:x', 'states:y',
                         'state_rates:y', 'states:v',
                         'state_rates:v', 'controls:theta', 'control_rates:theta_rate',
-                        'control_rates:theta_rate2', 'parameters:g']:
-            self.assertTrue(plot_dir.joinpath(f'{varname.replace(":","_")}.png').exists())
+                        'control_rates:theta_rate2']:
+            plotfile = plot_dir.joinpath(f'{varname.replace(":", "_")}.png')
+            self.assertTrue(plotfile.exists(), msg=f'plot file {plotfile} does not exist!')
+
+        dm.options['plots'] = plots_cache
 
 
 @use_tempdirs
 class TestSimulateArrayParam(unittest.TestCase):
 
     def test_simulate_array_param(self):
         #
@@ -809,16 +829,16 @@
         #
         dm.run_problem(p, simulate=True)
 
         # Test the results
         sol_results = om.CaseReader('dymos_solution.db').get_case('final')
         sim_results = om.CaseReader('dymos_solution.db').get_case('final')
 
-        sol = sol_results.get_val('traj.phase0.timeseries.parameters:array')
-        sim = sim_results.get_val('traj.phase0.timeseries.parameters:array')
+        sol = sol_results.get_val('traj.phase0.parameter_vals:array')
+        sim = sim_results.get_val('traj.phase0.parameter_vals:array')
 
         assert_near_equal(sol - sim, np.zeros_like(sol))
 
         # Test that the parameter is available in the solution and simulation files
         sol = sol_results.get_val('traj.phase0.parameters:array')
         sim = sim_results.get_val('traj.phase0.parameters:array')
```

### Comparing `dymos-1.7.0/dymos/test/test_upgrade_guide.py` & `dymos-1.8.0/dymos/test/test_upgrade_guide.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,17 @@
         #
         assert_near_equal(p.get_val('traj.phase0.timeseries.time')[-1], 143, tolerance=0.05)
         assert_near_equal(p.get_val('traj.phase0.timeseries.states:y')[-1], 1.85E5, 1e-4)
         assert_near_equal(p.get_val('traj.phase0.timeseries.states:vx')[-1], 7796.6961, 1e-4)
         assert_near_equal(p.get_val('traj.phase0.timeseries.states:vy')[-1], 0, 1e-4)
 
         # upgrade_doc: begin parameter_timeseries
-        thrust = p.get_val('traj.phase0.timeseries.parameters:thrust')
+        thrust = p.get_val('traj.phase0.parameter_vals:thrust')
         # upgrade_doc: end parameter_timeseries
-        nn = phase.options['transcription'].grid_data.num_nodes
-        assert_near_equal(thrust, 2.1E6 * np.ones([nn, 1]))
+        assert_near_equal(thrust.ravel(), 2.1E6)
 
     def test_parameter_no_timeseries(self):
         import openmdao.api as om
         import dymos as dm
         from dymos.examples.brachistochrone.brachistochrone_ode import BrachistochroneODE
 
         p = om.Problem(model=om.Group())
@@ -748,15 +747,15 @@
 
             y0 = p.get_val('traj0.phase0.timeseries.states:y')[0]
             yf = p.get_val('traj0.phase0.timeseries.states:y')[-1]
 
             v0 = p.get_val('traj0.phase0.timeseries.states:v')[0]
             vf = p.get_val('traj0.phase0.timeseries.states:v')[-1]
 
-            g = p.get_val('traj0.phase0.timeseries.parameters:g')[0]
+            g = p.get_val('traj0.phase0.parameter_vals:g')[0]
 
             thetaf = p.get_val('traj0.phase0.timeseries.controls:theta')[-1]
 
             assert_near_equal(t_initial, 0.0)
             assert_near_equal(x0, 0.0)
             assert_near_equal(y0, 10.0)
             assert_near_equal(v0, 0.0)
```

### Comparing `dymos-1.7.0/dymos/trajectory/options.py` & `dymos-1.8.0/dymos/trajectory/options.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/trajectory/phase_linkage_comp.py` & `dymos-1.8.0/dymos/trajectory/phase_linkage_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 import openmdao.api as om
 
-from ..options import options as dymos_options
+from .._options import options as dymos_options
 from ..utils.misc import _unspecified
 
 
 class PhaseLinkageComp(om.ExplicitComponent):
     """
     Component that provides a constraint between end values in two connected phases.
```

### Comparing `dymos-1.7.0/dymos/trajectory/test/test_phase_linkage_comp.py` & `dymos-1.8.0/dymos/trajectory/test/test_phase_linkage_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/trajectory/test/test_t_initial_bounds.py` & `dymos-1.8.0/dymos/trajectory/test/test_t_initial_bounds.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/trajectory/test/test_trajectory.py` & `dymos-1.8.0/dymos/trajectory/test/test_trajectory.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,16 +408,16 @@
         p.set_val('burn2.states:accel', value=burn2.interp('accel', [0.1, 0]))
         p.set_val('burn2.states:deltav', value=burn2.interp('deltav', [0.1, 0.2]))
         p.set_val('burn2.controls:u1', value=burn2.interp('u1', [1, 1]))
         p.set_val('burn2.parameters:c', value=1.5)
 
         p.run_model()
 
-        burn1_c_final = p.get_val('burn1.timeseries.parameters:c')[-1, ...]
-        burn2_c_initial = p.get_val('burn2.timeseries.parameters:c')[0, ...]
+        burn1_c_final = p.get_val('burn1.parameter_vals:c')[-1, ...]
+        burn2_c_initial = p.get_val('burn2.parameter_vals:c')[0, ...]
 
         c_linkage_error = p.get_val('linkages.burn1:c_final|burn2:c_initial')
         assert_near_equal(c_linkage_error, burn1_c_final - burn2_c_initial)
 
     def test_linked_control_to_polynomial_control(self):
 
         self.traj = dm.Trajectory()
@@ -623,14 +623,17 @@
 
         # Link Phases
         self.traj.link_phases(phases=['burn1', 'coast', 'burn2'],
                               vars=['time', 'r', 'theta', 'vr', 'vt', 'deltav'])
         self.traj.link_phases(phases=['burn1', 'burn2'], vars=['accel'])
         self.traj.link_phases(phases=['burn1', 'burn2'], vars=['u1_rate'])
 
+        for phs in burn1, coast, burn2:
+            phs.timeseries_options['include_control_rates'] = True
+
         # Finish Problem Setup
         p.model.linear_solver = om.DirectSolver()
 
         p.setup(check=True)
 
         # Set Initial Guesses
```

### Comparing `dymos-1.7.0/dymos/trajectory/test/test_trajectory_parameters.py` & `dymos-1.8.0/dymos/trajectory/test/test_trajectory_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
         traj.link_phases(phases=['burn1', 'burn2'], vars=['accel'])
 
     return traj
 
 
 def two_burn_orbit_raise_problem(transcription='gauss-lobatto', optimizer='SLSQP', r_target=3.0,
-                                 transcription_order=3, compressed=False,
+                                 transcription_order=3, compressed=False, run_driver=True, simulate=True,
                                  show_output=True, connected=False, param_mode='param_sequence'):
 
     p = om.Problem(model=om.Group())
 
     p.driver = om.pyOptSparseDriver()
     p.driver.options['optimizer'] = optimizer
     p.driver.declare_coloring()
@@ -230,15 +230,15 @@
         p.set_val('orbit_transfer.burn2.states:vr', val=burn2.interp('vr', [0, 0]))
         p.set_val('orbit_transfer.burn2.states:vt', val=burn2.interp('vt', [1, np.sqrt(1 / r_target)]))
         p.set_val('orbit_transfer.burn2.states:deltav', val=burn2.interp('deltav', [0.1, 0.2]))
         p.set_val('orbit_transfer.burn2.states:accel', val=burn2.interp('accel', [0.1, 0]))
 
         p.set_val('orbit_transfer.burn2.controls:u1', val=burn2.interp('u1', [0, 0]))
 
-    dm.run_problem(p, simulate=True)
+    dm.run_problem(p, run_driver=run_driver, simulate=simulate)
 
     return p
 
 
 @use_tempdirs
 class TestTrajectoryParameters(unittest.TestCase):
 
@@ -246,50 +246,65 @@
     def test_param_explicit_connections_to_sequence(self):
         """
         Test that, when setting up a trajectory parameter, we can explicitly provide a sequence
         in each phase as targets and a corresponding parameter for the phase will
         automatically be added.
         """
         p = two_burn_orbit_raise_problem(transcription='gauss-lobatto', transcription_order=3,
-                                         compressed=False, optimizer='IPOPT',
-                                         show_output=False, param_mode='param_sequence')
+                                         compressed=False, optimizer='IPOPT', run_driver=False,
+                                         simulate=False, show_output=False, param_mode='param_sequence')
 
-        if p.model.orbit_transfer.phases.burn2 in p.model.orbit_transfer.phases._subsystems_myproc:
-            assert_near_equal(p.get_val('orbit_transfer.burn2.states:deltav')[-1], 0.3995,
-                              tolerance=2.0E-3)
+        traj_c = p.get_val('orbit_transfer.parameter_vals:c')
+        burn1_c = p.get_val('orbit_transfer.burn1.parameter_vals:c')
+        coast_c = p.get_val('orbit_transfer.coast.parameter_vals:c')
+        burn2_c = p.get_val('orbit_transfer.burn2.parameter_vals:c')
+
+        assert_near_equal(burn1_c, traj_c)
+        assert_near_equal(coast_c, traj_c)
+        assert_near_equal(burn2_c, traj_c)
 
     @require_pyoptsparse(optimizer='IPOPT')
     def test_param_explicit_connections_to_sequence_missing_phase(self):
         """
         Test that, when setting up a trajectory parameter with a phase omitted from input,
         that we attempt to connect to an existing input variable in that phase of the same name.
         """
         p = two_burn_orbit_raise_problem(transcription='gauss-lobatto', transcription_order=3,
-                                         compressed=False, optimizer='IPOPT',
+                                         compressed=False, optimizer='IPOPT', run_driver=False, simulate=False,
                                          show_output=False,
                                          param_mode='param_sequence_missing_phase')
 
-        if p.model.orbit_transfer.phases.burn2 in p.model.orbit_transfer.phases._subsystems_myproc:
-            assert_near_equal(p.get_val('orbit_transfer.burn2.states:deltav')[-1], 0.3995,
-                              tolerance=2.0E-3)
+        traj_c = p.get_val('orbit_transfer.parameter_vals:c')
+        burn1_c = p.get_val('orbit_transfer.burn1.parameter_vals:c')
+        coast_c = p.get_val('orbit_transfer.coast.parameter_vals:c')
+        burn2_c = p.get_val('orbit_transfer.burn2.parameter_vals:c')
+
+        assert_near_equal(burn1_c, traj_c)
+        assert_near_equal(coast_c, traj_c)
+        assert_near_equal(burn2_c, traj_c)
 
     @require_pyoptsparse(optimizer='IPOPT')
     def test_param_no_targets(self):
         """
         Test that, when setting up a trajectory parameter with a phase omitted from input,
         that we attempt to connect to an existing input variable in that phase of the same name.
         """
         p = two_burn_orbit_raise_problem(transcription='gauss-lobatto', transcription_order=3,
-                                         compressed=False, optimizer='IPOPT',
-                                         show_output=False,
+                                         compressed=False, optimizer='IPOPT', run_driver=False,
+                                         show_output=False, simulate=False,
                                          param_mode='param_no_targets')
 
-        if p.model.orbit_transfer.phases.burn2 in p.model.orbit_transfer.phases._subsystems_myproc:
-            assert_near_equal(p.get_val('orbit_transfer.burn2.states:deltav')[-1], 0.3995,
-                              tolerance=2.0E-3)
+        traj_c = p.get_val('orbit_transfer.parameter_vals:c')
+        burn1_c = p.get_val('orbit_transfer.burn1.parameter_vals:c')
+        coast_c = p.get_val('orbit_transfer.coast.parameter_vals:c')
+        burn2_c = p.get_val('orbit_transfer.burn2.parameter_vals:c')
+
+        assert_near_equal(burn1_c, traj_c)
+        assert_near_equal(coast_c, traj_c)
+        assert_near_equal(burn2_c, traj_c)
 
 
 @use_tempdirs
 class TestPhaseParameterPromotion(unittest.TestCase):
 
     @require_pyoptsparse(optimizer='SLSQP')
     def test_promotes_parameter(self):
```

### Comparing `dymos-1.7.0/dymos/trajectory/trajectory.py` & `dymos-1.8.0/dymos/trajectory/trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import OrderedDict
 from collections.abc import Sequence
 import itertools
 import sys
 
 from openmdao.utils.om_warnings import warn_deprecation
 from openmdao.utils.graph_utils import get_sccs_topo
+from openmdao.utils.units import unit_conversion
 
 import numpy as np
 import networkx as nx
 
 import openmdao.api as om
 from openmdao.utils.mpi import MPI
 
@@ -17,14 +18,15 @@
 from .options import LinkageOptionsDictionary
 from .phase_linkage_comp import PhaseLinkageComp
 from ..phase.analytic_phase import AnalyticPhase
 from ..phase.options import TrajParameterOptionsDictionary
 from ..transcriptions.common import ParameterComp
 from ..utils.misc import get_rate_units, _unspecified
 from ..utils.introspection import get_promoted_vars, get_source_metadata
+from .._options import options as dymos_options
 
 
 class Trajectory(om.Group):
     """
     Class definition for a Trajectory group.
 
     A Trajectory object serves as a container for one or more Phases, as well as the linkage
@@ -240,15 +242,15 @@
             (meaning they cannot have a unique value at each node).  Otherwise False.
         """
         if name not in self.parameter_options:
             self.parameter_options[name] = TrajParameterOptionsDictionary()
             self.parameter_options[name]['name'] = name
         else:
             raise ValueError(f'Attempted to add parameter "{name}" to trajectory but trajectory already has a parameter'
-                             'of that name.')
+                             ' of that name.')
 
         self.set_parameter_options(name, units=units, val=val, desc=desc, opt=opt, targets=targets, lower=lower,
                                    upper=upper, scaler=scaler, adder=adder, ref0=ref0, ref=ref, shape=shape,
                                    dynamic=dynamic, static_target=static_target)
 
     def _setup_parameters(self):
         """
@@ -539,34 +541,39 @@
                 units[i] = phases[i].time_options['units']
             elif classes[i] == 't_phase':
                 time_name = phases[i].time_options['name']
                 sources[i] = f'timeseries.{time_name}_phase'
                 units[i] = phases[i].time_options['units']
                 shapes[i] = (1,)
             elif classes[i] == 'state':
-                sources[i] = f'timeseries.states:{vars[i]}'
+                prefix = 'states:' if dymos_options['use_timeseries_prefix'] else ''
+                sources[i] = f'timeseries.{prefix}{vars[i]}'
                 units[i] = phases[i].state_options[vars[i]]['units']
                 shapes[i] = phases[i].state_options[vars[i]]['shape']
             elif classes[i] in {'indep_control', 'input_control'}:
-                sources[i] = f'timeseries.controls:{vars[i]}'
+                prefix = 'controls:' if dymos_options['use_timeseries_prefix'] else ''
+                sources[i] = f'timeseries.{prefix}{vars[i]}'
                 units[i] = phases[i].control_options[vars[i]]['units']
                 shapes[i] = phases[i].control_options[vars[i]]['shape']
             elif classes[i] in {'control_rate', 'control_rate2'}:
-                sources[i] = f'timeseries.control_rates:{vars[i]}'
+                prefix = 'control_rates:' if dymos_options['use_timeseries_prefix'] else ''
+                sources[i] = f'timeseries.{prefix}{vars[i]}'
                 control_name = vars[i][:-5] if classes[i] == 'control_rate' else vars[i][:-6]
                 units[i] = phases[i].control_options[control_name]['units']
                 deriv = 1 if classes[i].endswith('rate') else 2
                 units[i] = get_rate_units(units[i], phases[i].time_options['units'], deriv=deriv)
                 shapes[i] = phases[i].control_options[control_name]['shape']
             elif classes[i] in {'indep_polynomial_control', 'input_polynomial_control'}:
-                sources[i] = f'timeseries.polynomial_controls:{vars[i]}'
+                prefix = 'polynomial_controls:' if dymos_options['use_timeseries_prefix'] else ''
+                sources[i] = f'timeseries.{prefix}{vars[i]}'
                 units[i] = phases[i].polynomial_control_options[vars[i]]['units']
                 shapes[i] = phases[i].polynomial_control_options[vars[i]]['shape']
             elif classes[i] in {'polynomial_control_rate', 'polynomial_control_rate2'}:
-                sources[i] = f'timeseries.polynomial_control_rates:{vars[i]}'
+                prefix = 'polynomial_control_rates:' if dymos_options['use_timeseries_prefix'] else ''
+                sources[i] = f'timeseries.{prefix}{vars[i]}'
                 control_name = vars[i][:-5] if classes[i] == 'polynomial_control_rate' else vars[i][:-6]
                 control_units = phases[i].polynomial_control_options[control_name]['units']
                 time_units = phases[i].time_options['units']
                 deriv = 1 if classes[i].endswith('rate') else 2
                 units[i] = get_rate_units(control_units, time_units, deriv=deriv)
                 shapes[i] = phases[i].polynomial_control_options[control_name]['shape']
             elif classes[i] == 'parameter':
@@ -592,18 +599,24 @@
 
         if linkage_options['units_a'] is _unspecified:
             linkage_options['units_a'] = units['a']
 
         if linkage_options['units_b'] is _unspecified:
             linkage_options['units_b'] = units['b']
 
-        if not linkage_options['connected'] and (linkage_options['units_a'] != linkage_options['units_b']) and \
-                linkage_options['units'] is _unspecified:
-            raise ValueError(f'{info_str}Linkage units were not specified but the units of '
-                             f'var_a ({units["a"]}) and var_b ({units["b"]}) are not the same. '
+        if units['a'] is not None and units['b'] is not None:
+            conversion_scaler, conversion_offset = unit_conversion(units['a'], units['b'])
+        else:
+            conversion_scaler, conversion_offset = (1.0, 0.0)
+
+        if not linkage_options['connected'] \
+                and linkage_options['units'] is _unspecified \
+                and (abs(conversion_scaler - 1.0) > 1.0E-15 or abs(conversion_offset) > 1.0E-15):
+            raise ValueError(f'{info_str}Linkage units were not specified but the units of {phase_name_a}.{var_a} '
+                             f'({units["a"]}) and {phase_name_b}.{var_b} ({units["b"]}) are not equivalent. '
                              f'Units for this linkage constraint must be specified explicitly.')
         else:
             linkage_options['units'] = units['a']
 
     def _expand_star_linkage_configure(self):
         """
         Finds the variable pair ('*', '*') and expands it out to time and all states if found.
@@ -716,15 +729,18 @@
                     'indep_polynomial_control': 'polynomial_controls:',
                     'polynomial_control_rate': 'polynomial_control_rates:',
                     'polynomial_control_rate2': 'polynomial_control_rates:',
                     'ode': ''
                     }
 
         def _get_prefixed_var(var, phase):
-            return f'{prefixes[phase.classify_var(var)]}{var}'
+            if dymos_options['use_timeseries_prefix']:
+                return f'{prefixes[phase.classify_var(var)]}{var}'
+            else:
+                return var
 
         # First, if the user requested all states and time be continuous ('*', '*'), then
         # expand it out.
         self._expand_star_linkage_configure()
 
         _print_on_rank(f'--- Linkage Report [{self.pathname}] ---')
```

### Comparing `dymos-1.7.0/dymos/transcriptions/analytic/analytic.py` & `dymos-1.8.0/dymos/transcriptions/analytic/analytic.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/analytic/analytic_timeseries_output_comp.py` & `dymos-1.8.0/dymos/transcriptions/analytic/analytic_timeseries_output_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/common/continuity_comp.py` & `dymos-1.8.0/dymos/transcriptions/common/continuity_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import openmdao.api as om
 
 from ..grid_data import GridData
 from ...utils.misc import get_rate_units
-from ...options import options as dymos_options
+from ..._options import options as dymos_options
 
 
 class ContinuityCompBase(om.ExplicitComponent):
     """
     ContinuityComp defines constraints to ensure continuity between adjacent segments.
 
     Parameters
```

### Comparing `dymos-1.7.0/dymos/transcriptions/common/control_group.py` & `dymos-1.8.0/dymos/transcriptions/common/control_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import openmdao.api as om
 
 from ..grid_data import GridData
 from ...utils.misc import get_rate_units, CoerceDesvar, reshape_val
 from ...utils.lagrange import lagrange_matrices
 from ...utils.indexing import get_desvar_indices
 from ...utils.constants import INF_BOUND
-from ...options import options as dymos_options
+from ..._options import options as dymos_options
 
 
 class ControlInterpComp(om.ExplicitComponent):
     """
     Class definition for the ControlInterpComp.
 
     Compute the approximated control values and rates given the values of a control at all nodes,
```

### Comparing `dymos-1.7.0/dymos/transcriptions/common/parameter_comp.py` & `dymos-1.8.0/dymos/transcriptions/common/parameter_comp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Definition of the Passthru Component."""
 
 
 import numpy as np
 
 from openmdao.core.explicitcomponent import ExplicitComponent
 from ...utils.misc import _unspecified
-from ...options import options as dymos_options
+from ..._options import options as dymos_options
 
 
 class ParameterComp(ExplicitComponent):
     """
     A component which simply passes a parameter input to an equivalent output.
 
     Parameters
@@ -29,15 +29,15 @@
         """
         Instantiate MuxComp and populate private members.
         """
         super().__init__(**kwargs)
 
         self._no_check_partials = not dymos_options['include_check_partials']
 
-    def add_parameter(self, name, val=1.0, shape=None, output_name=None, src_indices=None, flat_src_indices=None,
+    def add_parameter(self, name, val=1.0, shape=None, output_name=None,
                       units=None, desc='', tags=None, input_tags=None, output_tags=None, input_shape_by_conn=False,
                       input_copy_shape=None, output_shape_by_conn=False, output_copy_shape=None,
                       distributed=None, res_units=None, lower=None, upper=None, ref=1.0, ref0=0.0, res_ref=1.0, ):
         """
         Add an input/output pair for a variable to this component.
 
         Parameters
@@ -48,22 +48,14 @@
             The initial value of the variable being added in user-defined units.
             Default is 1.0.
         shape : int or tuple or list or None
             Shape of this variable, only required if src_indices not provided and
             val is not an array. Default is None.
         output_name : str
             Name given to the output variale in this component's namespace.  If None, f'{name}_value' is used.
-        src_indices : int or list or tuple or int ndarray or Iterable or None
-            The global indices of the source variable to transfer data from.
-            A value of None implies this input depends on all entries of the source array.
-            Default is None. The shapes of the target and src_indices must match,
-            and the form of the entries within is determined by the value of 'flat_src_indices'.
-        flat_src_indices : bool
-            If True and the source is non-flat, each entry of src_indices is assumed to be an index
-            into the flattened source.  Ignored if the source is flat.
         units : str or None
             Units in which this input variable will be provided to the component
             during execution. Default is None, which means it is unitless.
         desc : str
             Description of the variable.
         tags : str or list of strs
             User defined tags that can be used to filter what gets listed when calling
@@ -146,15 +138,15 @@
         if np.ndim(val) == 0 or _val.shape == (1,):
             in_val = np.full(_shape, _val)
         else:
             in_val = _val
         out_val = np.expand_dims(in_val, axis=0)
 
         i_meta = self.add_input(name=f'parameters:{name}', val=in_val, shape=_shape, units=units, desc=desc,
-                                src_indices=src_indices, flat_src_indices=flat_src_indices, tags=tags + input_tags,
+                                tags=tags + input_tags,
                                 shape_by_conn=input_shape_by_conn, copy_shape=input_copy_shape, distributed=distributed)
 
         o_meta = self.add_output(name=_out_name, val=out_val, shape=_out_shape, units=units,
                                  desc=desc, tags=tags + output_tags, res_units=res_units, ref=ref, ref0=ref0,
                                  res_ref=res_ref, lower=lower, upper=upper, shape_by_conn=output_shape_by_conn,
                                  copy_shape=output_copy_shape, distributed=distributed)
```

### Comparing `dymos-1.7.0/dymos/transcriptions/common/polynomial_control_group.py` & `dymos-1.8.0/dymos/transcriptions/common/polynomial_control_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..grid_data import GridData
 from ...utils.lgl import lgl
 from ...utils.lagrange import lagrange_matrices
 from ...utils.misc import get_rate_units, reshape_val
 from ...utils.constants import INF_BOUND
 
-from ...options import options as dymos_options
+from ..._options import options as dymos_options
 
 
 class LGLPolynomialControlComp(om.ExplicitComponent):
     """
     Component which interpolates controls as a single polynomial across the entire phase.
 
     Parameters
```

### Comparing `dymos-1.7.0/dymos/transcriptions/common/test/test_continuity_comp.py` & `dymos-1.8.0/dymos/transcriptions/common/test/test_continuity_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/common/test/test_control_interp_comp.py` & `dymos-1.8.0/dymos/transcriptions/common/test/test_control_interp_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/common/test/test_polynomial_control_group.py` & `dymos-1.8.0/dymos/transcriptions/common/test/test_polynomial_control_group.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/common/test/test_time_comp.py` & `dymos-1.8.0/dymos/transcriptions/common/test/test_time_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/common/time_comp.py` & `dymos-1.8.0/dymos/transcriptions/common/time_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 import openmdao.api as om
 
-from ...options import options as dymos_options
+from ..._options import options as dymos_options
 
 
 class TimeComp(om.ExplicitComponent):
     """
     Class definition of the TimeComp.
 
     Parameters
```

### Comparing `dymos-1.7.0/dymos/transcriptions/common/timeseries_group.py` & `dymos-1.8.0/dymos/transcriptions/common/timeseries_group.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/common/timeseries_output_comp.py` & `dymos-1.8.0/dymos/transcriptions/common/timeseries_output_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import openmdao.api as om
 
 from ...transcriptions.grid_data import GridData
-from ...options import options as dymos_options
+from ..._options import options as dymos_options
 
 
 class TimeseriesOutputCompBase(om.ExplicitComponent):
     """
     Class definition of the TimeseriesOutputCompBase.
 
     TimeseriesOutputComp collects variable values from the phase and provides them in chronological
```

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/explicit_shooting.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/explicit_shooting.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from openmdao.utils.om_warnings import warn_deprecation
 
 from ..pseudospectral.components import PseudospectralTimeseriesOutputComp
 from .explicit_shooting_continuity_comp import ExplicitShootingContinuityComp
 from ..transcription_base import TranscriptionBase
 from ..grid_data import GaussLobattoGrid, RadauGrid, UniformGrid
 from .ode_integration_comp import ODEIntegrationComp
+from ..._options import options as dymos_options
 from ...utils.misc import get_rate_units, CoerceDesvar
 from ...utils.indexing import get_src_indices_by_row
 from ...utils.introspection import get_promoted_vars, get_source_metadata, get_targets
 from ...utils.constants import INF_BOUND
 from ..common import TimeComp, TimeseriesOutputGroup, ControlGroup, PolynomialControlGroup
 
 
@@ -135,15 +136,15 @@
 
         # Warn about invalid options
         phase.check_time_options()
 
         for ts_name, ts_options in phase._timeseries.items():
             if t_name not in ts_options['outputs']:
                 phase.add_timeseries_output(t_name, timeseries=ts_name)
-            if t_phase_name not in ts_options['outputs']:
+            if t_phase_name not in ts_options['outputs'] and phase.timeseries_options['include_t_phase']:
                 phase.add_timeseries_output(t_phase_name, timeseries=ts_name)
 
         # if times_per_seg is None:
         # Case 1:  Compute times at 'all' node set.
         num_nodes = self._output_grid_data.num_nodes
         node_ptau = self._output_grid_data.node_ptau
         node_dptau_dstau = self._output_grid_data.node_dptau_dstau
@@ -255,28 +256,30 @@
         ----------
         phase : dymos.Phase
             The phase object to which this transcription instance applies.
         """
         integ = phase._get_subsystem('integrator')
         integ._configure_states()
 
+        state_prefix = 'states:' if dymos_options['use_timeseries_prefix'] else ''
+
         for name, options in phase.state_options.items():
-            phase.promotes('integrator', inputs=[f'states:{name}'])
+            phase.promotes('integrator', inputs=[(f'states:{name}', f'initial_states:{name}')])
             for ts_name, ts_options in phase._timeseries.items():
-                if f'states:{name}' not in ts_options['outputs']:
-                    phase.add_timeseries_output(name, output_name=f'states:{name}',
+                if f'{state_prefix}{name}' not in ts_options['outputs']:
+                    phase.add_timeseries_output(name, output_name=f'{state_prefix}{name}',
                                                 timeseries=ts_name)
 
-        # Add the appropriate design parameters
+        # Add the appropriate design variables
         for state_name, options in phase.state_options.items():
             if options['fix_final']:
                 raise ValueError('fix_final is not a valid option for states when using the '
                                  'ExplicitShooting transcription.')
             if options['opt'] and not options['fix_initial']:
-                phase.add_design_var(name=f'states:{state_name}',
+                phase.add_design_var(name=f'initial_states:{state_name}',
                                      lower=options['lower'],
                                      upper=options['upper'],
                                      scaler=options['scaler'],
                                      adder=options['adder'],
                                      ref0=options['ref0'],
                                      ref=options['ref'])
 
@@ -354,24 +357,30 @@
                                          grid_data=self.options['grid'],
                                          output_grid_data=self._output_grid_data)
 
             phase.add_subsystem('control_group',
                                 subsys=control_group,
                                 promotes=['dt_dstau', 'controls:*', 'control_values:*', 'control_rates:*'])
 
+            control_prefix = 'controls:' if dymos_options['use_timeseries_prefix'] else ''
+            control_rate_prefix = 'control_rates:' if dymos_options['use_timeseries_prefix'] else ''
+
             for name, options in phase.control_options.items():
                 for ts_name, ts_options in phase._timeseries.items():
-                    if f'controls:{name}' not in ts_options['outputs']:
-                        phase.add_timeseries_output(name, output_name=f'controls:{name}',
+
+                    if f'{control_prefix}{name}' not in ts_options['outputs']:
+                        phase.add_timeseries_output(name, output_name=f'{control_prefix}{name}',
                                                     timeseries=ts_name)
-                    if f'control_rates:{name}_rate' not in ts_options['outputs']:
-                        phase.add_timeseries_output(f'{name}_rate', output_name=f'control_rates:{name}_rate',
+                    if f'{control_rate_prefix}{name}_rate' not in ts_options['outputs'] \
+                            and phase.timeseries_options['include_control_rates']:
+                        phase.add_timeseries_output(f'{name}_rate', output_name=f'{control_rate_prefix}{name}_rate',
                                                     timeseries=ts_name)
-                    if f'control_rates:{name}_rate2' not in ts_options['outputs']:
-                        phase.add_timeseries_output(f'{name}_rate2', output_name=f'control_rates:{name}_rate2',
+                    if f'{control_rate_prefix}{name}_rate2' not in ts_options['outputs'] \
+                            and phase.timeseries_options['include_control_rates']:
+                        phase.add_timeseries_output(f'{name}_rate2', output_name=f'{control_rate_prefix}{name}_rate2',
                                                     timeseries=ts_name)
 
     def configure_controls(self, phase):
         """
         Configure the inputs/outputs for the controls.
 
         Parameters
@@ -441,24 +450,30 @@
         if phase.polynomial_control_options:
             sys = PolynomialControlGroup(grid_data=self._output_grid_data,
                                          polynomial_control_options=phase.polynomial_control_options,
                                          time_units=phase.time_options['units'])
             phase.add_subsystem('polynomial_control_group', subsys=sys,
                                 promotes_inputs=['*'], promotes_outputs=['*'])
 
+            control_prefix = 'polynomial_controls:' if dymos_options['use_timeseries_prefix'] else ''
+            control_rate_prefix = 'polynomial_control_rates:' if dymos_options['use_timeseries_prefix'] else ''
+
             for name, options in phase.polynomial_control_options.items():
+
                 for ts_name, ts_options in phase._timeseries.items():
-                    if f'polynomial_controls:{name}' not in ts_options['outputs']:
-                        phase.add_timeseries_output(name, output_name=f'polynomial_controls:{name}',
+                    if f'{control_prefix}{name}' not in ts_options['outputs']:
+                        phase.add_timeseries_output(name, output_name=f'{control_prefix}{name}',
                                                     timeseries=ts_name)
-                    if f'polynomial_control_rates:{name}_rate' not in ts_options['outputs']:
-                        phase.add_timeseries_output(f'{name}_rate', output_name=f'polynomial_control_rates:{name}_rate',
+                    if f'{control_rate_prefix}{name}_rate' not in ts_options['outputs'] \
+                            and phase.timeseries_options['include_control_rates']:
+                        phase.add_timeseries_output(f'{name}_rate', output_name=f'{control_rate_prefix}{name}_rate',
                                                     timeseries=ts_name)
-                    if f'polynomial_control_rates:{name}_rate2' not in ts_options['outputs']:
-                        phase.add_timeseries_output(f'{name}_rate2', output_name=f'polynomial_control_rates:{name}_rate2',
+                    if f'{control_rate_prefix}{name}_rate2' not in ts_options['outputs'] \
+                            and phase.timeseries_options['include_control_rates']:
+                        phase.add_timeseries_output(f'{name}_rate2', output_name=f'{control_rate_prefix}{name}_rate2',
                                                     timeseries=ts_name)
 
     def configure_polynomial_controls(self, phase):
         """
         Configure the inputs/outputs for the polynomial controls.
 
         Parameters
@@ -566,25 +581,25 @@
         control_rates_to_enforce = set()
         control_rates2_to_enforce = set()
 
         for control_name, options in phase.control_options.items():
 
             if options['continuity'] and any_control_cnty:
                 controls_to_enforce.add(control_name)
-                phase.connect(f'timeseries.controls:{control_name}',
+                phase.connect(f'control_values:{control_name}',
                               f'continuity_comp.controls:{control_name}',
                               src_indices=src_idxs)
             if options['rate_continuity'] and any_rate_cnty:
                 control_rates_to_enforce.add(control_name)
-                phase.connect(f'timeseries.control_rates:{control_name}_rate',
+                phase.connect(f'control_rates:{control_name}_rate',
                               f'continuity_comp.control_rates:{control_name}_rate',
                               src_indices=src_idxs)
             if options['rate2_continuity'] and any_rate_cnty:
                 control_rates2_to_enforce.add(control_name)
-                phase.connect(f'timeseries.control_rates:{control_name}_rate2',
+                phase.connect(f'control_rates:{control_name}_rate2',
                               f'continuity_comp.control_rates:{control_name}_rate2',
                               src_indices=src_idxs)
 
         if any((controls_to_enforce, control_rates_to_enforce, control_rates2_to_enforce)):
             phase.continuity_comp.configure_io(controls_to_enforce=controls_to_enforce,
                                                control_rates_to_enforce=control_rates_to_enforce,
                                                control_rates2_to_enforce=control_rates2_to_enforce)
```

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/explicit_shooting_continuity_comp.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/explicit_shooting_continuity_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/explicit_shooting_timeseries_comp.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/explicit_shooting_timeseries_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 from openmdao.utils.units import unit_conversion
-from ...options import options as dymos_options
+from ..._options import options as dymos_options
 
 from ..common.timeseries_output_comp import TimeseriesOutputCompBase
 
 
 class ExplicitShootingTimeseriesComp(TimeseriesOutputCompBase):
 
     """
```

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/ode_evaluation_group.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/ode_evaluation_group.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/ode_integration_comp.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/ode_integration_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import openmdao.api as om
 from scipy.integrate import solve_ivp
 
-from ...options import options as dymos_options
+from ..._options import options as dymos_options
 
 from .ode_evaluation_group import ODEEvaluationGroup
 
 
 class ODEIntegrationComp(om.ExplicitComponent):
     """
     A component to perform explicit integration with a generic ODE integrator/IVP solver.
```

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/state_rate_collector_comp.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/state_rate_collector_comp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 import openmdao.api as om
 
 from dymos.utils.misc import get_rate_units
-from dymos.options import options as dymos_options
+from ..._options import options as dymos_options
 
 
 class StateRateCollectorComp(om.ExplicitComponent):
     """
     Class definition for StateRateCollectorComp.
 
     Collects the state rates and outputs them in the units specified in the state options.
```

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/tau_comp.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/tau_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 import openmdao.api as om
 
-from ...options import options as dymos_options
+from ..._options import options as dymos_options
 
 
 class TauComp(om.ExplicitComponent):
     """
     Component that computes the phase tau, segment tau, and current segment index based on time.
 
     Note that stau is differentiable within a segment but non-differentiable at the segment bounds.
```

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/test_control_interpolation_comp.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/test_control_interpolation_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/test_explicit_shooting.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/test_explicit_shooting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 import warnings
 
 import numpy as np
 
 import openmdao.api as om
 import dymos as dm
-import dymos.options as dymos_options
+from dymos import options as dymos_options
 
 from openmdao.utils.assert_utils import assert_check_partials, assert_near_equal
 from openmdao.utils.testing_utils import use_tempdirs
 
 from dymos.examples.brachistochrone.brachistochrone_ode import BrachistochroneODE
 
 
@@ -102,15 +102,15 @@
 
         prob.model.add_subsystem('phase0', phase)
 
         prob.setup(force_alloc_complex=False)
 
         prob.set_val('phase0.t_initial', 0.0)
         prob.set_val('phase0.t_duration', 1.0)
-        prob.set_val('phase0.states:y', 1.0)
+        prob.set_val('phase0.initial_states:y', 1.0)
 
         prob.run_model()
 
         with np.printoptions(linewidth=1024):
             cpd = prob.check_partials(compact_print=True)
 
         assert_check_partials(cpd, rtol=1.0E-5)
@@ -138,16 +138,16 @@
 
         prob.model.add_subsystem('phase0', phase)
 
         prob.setup(force_alloc_complex=True)
 
         prob.set_val('phase0.t_initial', 0.0)
         prob.set_val('phase0.t_duration', 1.0)
-        prob.set_val('phase0.states:x', 0.5)
-        prob.set_val('phase0.states:y', 1.0)
+        prob.set_val('phase0.initial_states:x', 0.5)
+        prob.set_val('phase0.initial_states:y', 1.0)
         prob.set_val('phase0.parameters:p', 1)
 
         prob.run_model()
 
         t_f = prob.get_val('phase0.integrator.t_final')
         t = prob.get_val('phase0.integrator.time')
         x_f = prob.get_val('phase0.integrator.states_out:x')
@@ -204,17 +204,17 @@
 
                 phase.add_objective('time', loc='final')
 
                 prob.setup(force_alloc_complex=True)
 
                 prob.set_val('traj0.phase0.t_initial', 0.0)
                 prob.set_val('traj0.phase0.t_duration', 2)
-                prob.set_val('traj0.phase0.states:x', 0.0)
-                prob.set_val('traj0.phase0.states:y', 10.0)
-                prob.set_val('traj0.phase0.states:v', 1.0E-6)
+                prob.set_val('traj0.phase0.initial_states:x', 0.0)
+                prob.set_val('traj0.phase0.initial_states:y', 10.0)
+                prob.set_val('traj0.phase0.initial_states:v', 1.0E-6)
                 prob.set_val('traj0.phase0.parameters:g', 9.80665, units='m/s**2')
                 prob.set_val('traj0.phase0.controls:theta', phase.interp('theta', ys=[0.01, 50]), units='deg')
 
                 dm.run_problem(prob)
 
                 x = prob.get_val('traj0.phase0.timeseries.states:x')
                 y = prob.get_val('traj0.phase0.timeseries.states:y')
@@ -273,17 +273,17 @@
 
                 phase.add_objective('time', loc='final')
 
                 prob.setup(force_alloc_complex=True)
 
                 prob.set_val('traj0.phase0.t_initial', 0.0)
                 prob.set_val('traj0.phase0.t_duration', 2)
-                prob.set_val('traj0.phase0.states:x', 0.0)
-                prob.set_val('traj0.phase0.states:y', 10.0)
-                prob.set_val('traj0.phase0.states:v', 1.0E-6)
+                prob.set_val('traj0.phase0.initial_states:x', 0.0)
+                prob.set_val('traj0.phase0.initial_states:y', 10.0)
+                prob.set_val('traj0.phase0.initial_states:v', 1.0E-6)
                 prob.set_val('traj0.phase0.controls:theta', phase.interp('theta', ys=[0.01, 90]), units='deg')
 
                 prob.run_driver()
 
                 x = prob.get_val('traj0.phase0.timeseries.states:x')
                 y = prob.get_val('traj0.phase0.timeseries.states:y')
                 ydot = prob.get_val('traj0.phase0.timeseries.ydot')
@@ -349,17 +349,17 @@
 
                         phase.add_objective('time', loc='final')
 
                         prob.setup(force_alloc_complex=True)
 
                         prob.set_val('traj0.phase0.t_initial', 0.0)
                         prob.set_val('traj0.phase0.t_duration', 2)
-                        prob.set_val('traj0.phase0.states:x', 0.0)
-                        prob.set_val('traj0.phase0.states:y', 10.0)
-                        prob.set_val('traj0.phase0.states:v', 1.0E-6)
+                        prob.set_val('traj0.phase0.initial_states:x', 0.0)
+                        prob.set_val('traj0.phase0.initial_states:y', 10.0)
+                        prob.set_val('traj0.phase0.initial_states:v', 1.0E-6)
                         prob.set_val('traj0.phase0.parameters:g', 9.80665, units='m/s**2')
                         prob.set_val('traj0.phase0.polynomial_controls:theta',
                                      phase.interp('theta', ys=[0.01, 50]), units='deg')
 
                         dm.run_problem(prob)
 
                         x = prob.get_val('traj0.phase0.timeseries.states:x')
@@ -468,17 +468,17 @@
 
             phase.add_objective('time', loc='final')
 
             prob.setup(force_alloc_complex=True)
 
             prob.set_val('phase0.t_initial', 0.0)
             prob.set_val('phase0.t_duration', 2)
-            prob.set_val('phase0.states:x', 0.0)
-            prob.set_val('phase0.states:y', 10.0)
-            prob.set_val('phase0.states:v', 1.0E-6)
+            prob.set_val('phase0.initial_states:x', 0.0)
+            prob.set_val('phase0.initial_states:y', 10.0)
+            prob.set_val('phase0.initial_states:v', 1.0E-6)
             prob.set_val('phase0.parameters:g', 1.0, units='m/s**2')
             prob.set_val('phase0.controls:theta', phase.interp('theta', ys=[0.01, 90]), units='deg')
 
             dm.run_problem(prob, run_driver=True)
 
             x = prob.get_val('phase0.timeseries.states:x')
             y = prob.get_val('phase0.timeseries.states:y')
@@ -628,17 +628,17 @@
             p.set_val('traj.phase0.t_initial', 0.0)
             p.set_val('traj.phase0.t_duration', 2.0)
 
             # Guesses for states are provided at all state_input nodes.
             # We use the phase.interpolate method to linearly interpolate values onto the state input nodes.
             # Since fix_initial=True for all states and fix_final=True for x and y, the initial or final
             # values of the interpolation provided here will not be changed by the optimizer.
-            p.set_val('traj.phase0.states:x', phase.interp('x', [0, 10]))
-            p.set_val('traj.phase0.states:y', phase.interp('y', [10, 5]))
-            p.set_val('traj.phase0.states:v', phase.interp('v', [0, 9.9]))
+            p.set_val('traj.phase0.initial_states:x', phase.interp('x', [0, 10]))
+            p.set_val('traj.phase0.initial_states:y', phase.interp('y', [10, 5]))
+            p.set_val('traj.phase0.initial_states:v', phase.interp('v', [0, 9.9]))
 
             # Guesses for controls are provided at all control_input node.
             # Here phase.interpolate is used to linearly interpolate values onto the control input nodes.
             p.set_val('traj.phase0.controls:theta', phase.interp('theta', [5, 100.5]))
 
             # Set the value for gravitational acceleration.
             p.set_val('traj.phase0.parameters:g', 9.80665)
```

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/test_ode_evaluation_group.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/test_ode_evaluation_group.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/test_ode_integration_comp.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/test_ode_integration_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 import numpy as np
 import openmdao.api as om
 import dymos as dm
-import dymos.options as dymos_options
+from dymos import options as dymos_options
 
 from openmdao.utils.assert_utils import assert_check_partials, assert_near_equal
 from dymos.examples.brachistochrone.brachistochrone_ode import BrachistochroneODE
 from dymos.transcriptions.explicit_shooting.ode_integration_comp import ODEIntegrationComp
 
 from dymos.phase.options import TimeOptionsDictionary, StateOptionsDictionary, ParameterOptionsDictionary
 from dymos.transcriptions.grid_data import GridData
```

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/test/test_tau_comp.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/test/test_tau_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/explicit_shooting/vandermonde_control_interp_comp.py` & `dymos-1.8.0/dymos/transcriptions/explicit_shooting/vandermonde_control_interp_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/grid_data.py` & `dymos-1.8.0/dymos/transcriptions/grid_data.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/collocation_comp.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/collocation_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Define the CollocationComp class."""
 import numpy as np
 
 import openmdao.api as om
 
 from ...grid_data import GridData
 from ....utils.misc import get_rate_units
-from ....options import options as dymos_options
+from ...._options import options as dymos_options
 
 
 class CollocationComp(om.ExplicitComponent):
     """
     Class definiton for the Collocationcomp.
 
     CollocationComp computes the generalized defect of a segment for implicit collocation.
```

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/control_endpoint_defect_comp.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/control_endpoint_defect_comp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import openmdao.api as om
 from ...grid_data import GridData
-from ....options import options as dymos_options
+from ...._options import options as dymos_options
 
 
 class ControlEndpointDefectComp(om.ExplicitComponent):
     r"""
     Compute/enforce the control endpoint defect when using the Radau Pseudospectral method.
 
     For each dynamic control, take the control values at all nodes.  Use a Radau interpolation
```

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/gauss_lobatto_interleave_comp.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/gauss_lobatto_interleave_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import openmdao.api as om
 from openmdao.utils.units import unit_conversion
 
 from ...grid_data import GridData
-from ....options import options as dymos_options
+from ...._options import options as dymos_options
 
 
 class GaussLobattoInterleaveComp(om.ExplicitComponent):
     r"""
     Class definition for the GaussLobattoInterleaveComp.
 
     Provides a contiguous output at all nodes for inputs which are only known at
```

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/pseudospectral_timeseries_output_comp.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/pseudospectral_timeseries_output_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/state_independents.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/state_independents.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Define the StateIndependents class."""
 
 import numpy as np
 
 import openmdao.api as om
 
 from ....transcriptions.grid_data import GridData
-from ....options import options as dymos_options
+from ...._options import options as dymos_options
 
 
 class StateIndependentsComp(om.ImplicitComponent):
     """
     Class definition for the StateIndependentsComp.
 
     A simple component that replaces the state indepvarcomps whenver the solver needs to solve for
```

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/state_interp_comp.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/state_interp_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import scipy.sparse as sp
 import openmdao.api as om
 from ...grid_data import GridData
 from ....utils.misc import get_rate_units
-from ....options import options as dymos_options
+from ...._options import options as dymos_options
 
 
 class StateInterpComp(om.ExplicitComponent):
     r"""
     Provide interpolated state values and/or rates for pseudospectral transcriptions.
 
     When the transcription is *gauss-lobatto* it accepts the state values and derivatives
```

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_opt.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_opt.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_sol_opt.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_sol_opt.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_solver.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_collocation_defect_solver.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_control_endpoint_defect_comp.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_control_endpoint_defect_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         u_coefs = np.polyfit(self.gd.node_ptau[-4:-1], self.p['controls:u'][-4:-1], deg=2)
         u_poly = np.poly1d(u_coefs.ravel())
         u_interp = u_poly(1.0)
         u_given = self.p['controls:u'][-1]
         assert_near_equal(np.ravel(self.p['endpoint_defect_comp.control_endpoint_defects:u']),
                           np.ravel(u_given - u_interp),
-                          tolerance=1.0E-12)
+                          tolerance=1.0E-9)
 
     def test_partials(self):
         cpd = self.p.check_partials(compact_print=False, method='cs')
         assert_check_partials(cpd)
 
 
 if __name__ == '__main__':  # pragma: no cover
```

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_gauss_lobatto_interleave_comp.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_gauss_lobatto_interleave_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/components/test/test_state_interp_comp.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/components/test/test_state_interp_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/gauss_lobatto.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/gauss_lobatto.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/pseudospectral_base.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/pseudospectral_base.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/radau_pseudospectral.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/radau_pseudospectral.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/pseudospectral/test/test_ps_base.py` & `dymos-1.8.0/dymos/transcriptions/pseudospectral/test/test_ps_base.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/__init__.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/__init__.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/ode_integration_interface.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/ode_integration_interface.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/ode_integration_interface_system.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/ode_integration_interface_system.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/odeint_control_interpolation_comp.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/odeint_control_interpolation_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/segment_simulation_comp.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/segment_simulation_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/segment_state_mux_comp.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/segment_state_mux_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/solve_ivp_control_group.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/solve_ivp_control_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,11 +262,12 @@
 
         self.control_interp_comp.configure_io()
 
         for name, options in control_options.items():
             if options['opt']:
                 num_input_nodes = gd.subset_num_nodes['control_input']
 
+                val = np.outer(np.ones(num_input_nodes), options['val'])
                 self.indep_controls.add_output(name=f'controls:{name}',
-                                               val=options['val'],
+                                               val=val,
                                                shape=(num_input_nodes, np.prod(options['shape'])),
                                                units=options['units'])
```

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/solve_ivp_polynomial_control_group.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/solve_ivp_polynomial_control_group.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/solve_ivp_timeseries_comp.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/solve_ivp_timeseries_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/state_rate_collector_comp.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/state_rate_collector_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from ....utils.misc import get_rate_units
-from ....options import options as dymos_options
+from ...._options import options as dymos_options
 import openmdao.api as om
 
 
 class StateRateCollectorComp(om.ExplicitComponent):
     """
     Class definition for StateRateCollectorComp.
```

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/components/test/test_segment_simulation_comp.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/components/test/test_segment_simulation_comp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/solve_ivp/solve_ivp.py` & `dymos-1.8.0/dymos/transcriptions/solve_ivp/solve_ivp.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/transcriptions/transcription_base.py` & `dymos-1.8.0/dymos/transcriptions/transcription_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .common import ControlGroup, PolynomialControlGroup, ParameterComp
 from ..utils.constants import INF_BOUND
 from ..utils.indexing import get_constraint_flat_idxs
 from ..utils.misc import _unspecified
 from ..utils.introspection import configure_states_introspection, get_promoted_vars, get_target_metadata, \
     configure_states_discovery
+from .._options import options as dymos_options
 
 
 class TranscriptionBase(object):
     """
     Base class for all dymos transcriptions.
 
     Parameters
@@ -82,15 +83,16 @@
         if not time_options['input_initial'] or not time_options['input_duration']:
             phase.add_subsystem('time_extents', om.IndepVarComp(),
                                 promotes_outputs=['*'])
 
         for ts_name, ts_options in phase._timeseries.items():
             if t_name not in ts_options['outputs']:
                 phase.add_timeseries_output(t_name, timeseries=ts_name)
-            if t_phase_name not in ts_options['outputs']:
+            if t_phase_name not in ts_options['outputs'] and \
+                    (phase.timeseries_options['include_t_phase'] or time_options['time_phase_targets']):
                 phase.add_timeseries_output(t_phase_name, timeseries=ts_name)
 
     def configure_time(self, phase):
         """
         Configure the inputs/outputs on the time component.
 
         Parameters
@@ -165,24 +167,29 @@
             control_group = ControlGroup(control_options=phase.control_options,
                                          time_units=phase.time_options['units'],
                                          grid_data=self.grid_data)
 
             phase.add_subsystem('control_group',
                                 subsys=control_group)
 
+            control_prefix = 'controls:' if dymos_options['use_timeseries_prefix'] else ''
+            control_rate_prefix = 'control_rates:' if dymos_options['use_timeseries_prefix'] else ''
+
             for name, options in phase.control_options.items():
                 for ts_name, ts_options in phase._timeseries.items():
-                    if f'controls:{name}' not in ts_options['outputs']:
-                        phase.add_timeseries_output(name, output_name=f'controls:{name}',
+                    if f'{control_prefix}{name}' not in ts_options['outputs']:
+                        phase.add_timeseries_output(name, output_name=f'{control_prefix}{name}',
                                                     timeseries=ts_name)
-                    if f'control_rates:{name}_rate' not in ts_options['outputs']:
-                        phase.add_timeseries_output(f'{name}_rate', output_name=f'control_rates:{name}_rate',
+                    if f'{control_rate_prefix}{name}_rate' not in ts_options['outputs'] and \
+                            (phase.timeseries_options['include_control_rates'] or options['rate_targets']):
+                        phase.add_timeseries_output(f'{name}_rate', output_name=f'{control_rate_prefix}{name}_rate',
                                                     timeseries=ts_name)
-                    if f'control_rates:{name}_rate2' not in ts_options['outputs']:
-                        phase.add_timeseries_output(f'{name}_rate2', output_name=f'control_rates:{name}_rate2',
+                    if f'{control_rate_prefix}{name}_rate2' not in ts_options['outputs'] and \
+                            (phase.timeseries_options['include_control_rates'] or options['rate2_targets']):
+                        phase.add_timeseries_output(f'{name}_rate2', output_name=f'{control_rate_prefix}{name}_rate2',
                                                     timeseries=ts_name)
 
     def configure_controls(self, phase):
         """
         Configure the inputs/outputs for the controls.
 
         Parameters
@@ -204,24 +211,29 @@
         if phase.polynomial_control_options:
             sys = PolynomialControlGroup(grid_data=self.grid_data,
                                          polynomial_control_options=phase.polynomial_control_options,
                                          time_units=phase.time_options['units'])
             phase.add_subsystem('polynomial_control_group', subsys=sys,
                                 promotes_inputs=['*'], promotes_outputs=['*'])
 
+            prefix = 'polynomial_controls:' if dymos_options['use_timeseries_prefix'] else ''
+            rate_prefix = 'polynomial_control_rates:' if dymos_options['use_timeseries_prefix'] else ''
+
             for name, options in phase.polynomial_control_options.items():
                 for ts_name, ts_options in phase._timeseries.items():
-                    if f'polynomial_controls:{name}' not in ts_options['outputs']:
-                        phase.add_timeseries_output(name, output_name=f'polynomial_controls:{name}',
+                    if f'{prefix}{name}' not in ts_options['outputs']:
+                        phase.add_timeseries_output(name, output_name=f'{prefix}{name}',
                                                     timeseries=ts_name)
-                    if f'polynomial_control_rates:{name}_rate' not in ts_options['outputs']:
-                        phase.add_timeseries_output(f'{name}_rate', output_name=f'polynomial_control_rates:{name}_rate',
+                    if f'{rate_prefix}{name}_rate' not in ts_options['outputs'] and \
+                            (phase.timeseries_options['include_control_rates'] or options['rate_targets']):
+                        phase.add_timeseries_output(f'{name}_rate', output_name=f'{rate_prefix}{name}_rate',
                                                     timeseries=ts_name)
-                    if f'polynomial_control_rates:{name}_rate2' not in ts_options['outputs']:
-                        phase.add_timeseries_output(f'{name}_rate2', output_name=f'polynomial_control_rates:{name}_rate2',
+                    if f'{rate_prefix}{name}_rate2' not in ts_options['outputs'] and \
+                            (phase.timeseries_options['include_control_rates'] or options['rate2_targets']):
+                        phase.add_timeseries_output(f'{name}_rate2', output_name=f'{rate_prefix}{name}_rate2',
                                                     timeseries=ts_name)
 
     def configure_polynomial_controls(self, phase):
         """
         Configure the inputs/outputs for the polynomial controls.
 
         Parameters
@@ -238,24 +250,25 @@
 
         Parameters
         ----------
         phase : dymos.Phase
             The phase object to which this transcription instance applies.
         """
         phase._check_parameter_options()
+        param_prefix = 'parameters:' if dymos_options['use_timeseries_prefix'] else ''
 
         if phase.parameter_options:
             param_comp = ParameterComp()
             phase.add_subsystem('param_comp', subsys=param_comp, promotes_inputs=['*'], promotes_outputs=['*'])
 
         for name, options in phase.parameter_options.items():
             if options['include_timeseries']:
                 for ts_name, ts_options in phase._timeseries.items():
-                    if f'parameters:{name}' not in ts_options['outputs']:
-                        phase.add_timeseries_output(name, output_name=f'parameters:{name}',
+                    if f'{param_prefix}{name}' not in ts_options['outputs']:
+                        phase.add_timeseries_output(name, output_name=f'{param_prefix}{name}',
                                                     timeseries=ts_name)
 
     def configure_parameters(self, phase):
         """
         Configure parameter promotion.
 
         This method assumes that utils.introspection.configure_parameters_introspection has already populated
@@ -337,21 +350,26 @@
         Configure the states for this transcription.
 
         Parameters
         ----------
         phase : dymos.Phase
             The phase object to which this transcription instance applies.
         """
+        state_prefix = 'states:' if dymos_options['use_timeseries_prefix'] else ''
+        state_rate_prefix = 'state_rates:' if dymos_options['use_timeseries_prefix'] else ''
+
         for name, options in phase.state_options.items():
             for ts_name, ts_options in phase._timeseries.items():
-                if f'states:{name}' not in ts_options['outputs']:
-                    phase.add_timeseries_output(name, output_name=f'states:{name}',
+                if f'{state_prefix}{name}' not in ts_options['outputs']:
+                    phase.add_timeseries_output(name, output_name=f'{state_prefix}{name}',
                                                 timeseries=ts_name)
-                if options['rate_source'] and f'state_rates:{name}' not in ts_options['outputs']:
-                    phase.add_timeseries_output(name=options['rate_source'], output_name=f'state_rates:{name}',
+                if options['rate_source'] and \
+                        f'{state_rate_prefix}{name}' not in ts_options['outputs'] and \
+                        phase.timeseries_options['include_state_rates']:
+                    phase.add_timeseries_output(name=options['rate_source'], output_name=f'{state_rate_prefix}{name}',
                                                 timeseries=ts_name)
 
     def setup_ode(self, phase):
         """
         Setup the ode for this transcription.
 
         Parameters
```

### Comparing `dymos-1.7.0/dymos/utils/hermite.py` & `dymos-1.8.0/dymos/utils/hermite.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/indexing.py` & `dymos-1.8.0/dymos/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/interpolate.py` & `dymos-1.8.0/dymos/utils/interpolate.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/introspection.py` & `dymos-1.8.0/dymos/utils/introspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import fnmatch
 import re
 
 import openmdao.api as om
 import numpy as np
 from openmdao.utils.array_utils import shape_to_len
 from dymos.utils.misc import _unspecified
+from .._options import options as dymos_options
 from ..phase.options import StateOptionsDictionary, TimeseriesOutputOptionsDictionary
 from .misc import get_rate_units
 
 
 def classify_var(var, time_options, state_options, parameter_options, control_options,
                  polynomial_control_options, timeseries_options=None):
     """
@@ -202,92 +203,84 @@
 
             elif var_type == 't_phase':
                 con['shape'] = (1,)
                 con['units'] = time_units if con['units'] is None else con['units']
                 con['constraint_path'] = f'timeseries.{time_name}_phase'
 
             elif var_type == 'state':
+                prefix = 'states:' if dymos_options['use_timeseries_prefix'] else ''
                 state_shape = phase.state_options[var]['shape']
                 state_units = phase.state_options[var]['units']
                 con['shape'] = state_shape
                 con['units'] = state_units if con['units'] is None else con['units']
-                con['constraint_path'] = f'timeseries.states:{var}'
+                con['constraint_path'] = f'timeseries.{prefix}{var}'
 
             elif var_type == 'parameter':
                 param_shape = phase.parameter_options[var]['shape']
                 param_units = phase.parameter_options[var]['units']
                 con['shape'] = param_shape
                 con['units'] = param_units if con['units'] is None else con['units']
                 con['constraint_path'] = f'parameter_vals:{var}'
 
-            elif var_type == 'indep_control':
+            elif var_type in ['indep_control', 'input_control']:
+                prefix = 'controls:' if dymos_options['use_timeseries_prefix'] else ''
                 control_shape = phase.control_options[var]['shape']
                 control_units = phase.control_options[var]['units']
 
                 con['shape'] = control_shape
                 con['units'] = control_units if con['units'] is None else con['units']
-                con['constraint_path'] = f'timeseries.controls:{var}'
+                con['constraint_path'] = f'timeseries.{prefix}{var}'
 
-            elif var_type == 'input_control':
-                control_shape = phase.control_options[var]['shape']
-                control_units = phase.control_options[var]['units']
-
-                con['shape'] = control_shape
-                con['units'] = control_units if con['units'] is None else con['units']
-                con['constraint_path'] = f'timeseries.controls:{var}'
-
-            elif var_type == 'indep_polynomial_control':
-                control_shape = phase.polynomial_control_options[var]['shape']
-                control_units = phase.polynomial_control_options[var]['units']
-                con['shape'] = control_shape
-                con['units'] = control_units if con['units'] is None else con['units']
-                con['constraint_path'] = f'timeseries.polynomial_controls:{var}'
-
-            elif var_type == 'input_polynomial_control':
+            elif var_type in ['indep_polynomial_control', 'input_polynomial_control']:
+                prefix = 'polynomial_controls:' if dymos_options['use_timeseries_prefix'] else ''
                 control_shape = phase.polynomial_control_options[var]['shape']
                 control_units = phase.polynomial_control_options[var]['units']
                 con['shape'] = control_shape
                 con['units'] = control_units if con['units'] is None else con['units']
-                con['constraint_path'] = f'timeseries.polynomial_controls:{var}'
+                con['constraint_path'] = f'timeseries.{prefix}{var}'
 
             elif var_type == 'control_rate':
+                prefix = 'control_rates:' if dymos_options['use_timeseries_prefix'] else ''
                 control_name = var[:-5]
                 control_shape = phase.control_options[control_name]['shape']
                 control_units = phase.control_options[control_name]['units']
                 con['shape'] = control_shape
                 con['units'] = get_rate_units(control_units, time_units, deriv=1) \
                     if con['units'] is None else con['units']
-                con['constraint_path'] = f'timeseries.control_rates:{var}'
+                con['constraint_path'] = f'timeseries.{prefix}{var}'
 
             elif var_type == 'control_rate2':
+                prefix = 'control_rates:' if dymos_options['use_timeseries_prefix'] else ''
                 control_name = var[:-6]
                 control_shape = phase.control_options[control_name]['shape']
                 control_units = phase.control_options[control_name]['units']
                 con['shape'] = control_shape
                 con['units'] = get_rate_units(control_units, time_units, deriv=2) \
                     if con['units'] is None else con['units']
-                con['constraint_path'] = f'timeseries.control_rates:{var}'
+                con['constraint_path'] = f'timeseries.{prefix}{var}'
 
             elif var_type == 'polynomial_control_rate':
+                prefix = 'polynomial_control_rates:' if dymos_options['use_timeseries_prefix'] else ''
                 control_name = var[:-5]
                 control_shape = phase.polynomial_control_options[control_name]['shape']
                 control_units = phase.polynomial_control_options[control_name]['units']
                 con['shape'] = control_shape
                 con['units'] = get_rate_units(control_units, time_units, deriv=1) \
                     if con['units'] is None else con['units']
-                con['constraint_path'] = f'timeseries.polynomial_control_rates:{var}'
+                con['constraint_path'] = f'timeseries.{prefix}{var}'
 
             elif var_type == 'polynomial_control_rate2':
+                prefix = 'polynomial_control_rates:' if dymos_options['use_timeseries_prefix'] else ''
                 control_name = var[:-6]
                 control_shape = phase.polynomial_control_options[control_name]['shape']
                 control_units = phase.polynomial_control_options[control_name]['units']
                 con['shape'] = control_shape
                 con['units'] = get_rate_units(control_units, time_units, deriv=2) \
                     if con['units'] is None else con['units']
-                con['constraint_path'] = f'timeseries.polynomial_control_rates:{var}'
+                con['constraint_path'] = f'timeseries.{prefix}{var}'
 
             elif var_type == 'timeseries_exec_comp_output':
                 con['shape'] = (1,)
                 con['units'] = None
                 con['constraint_path'] = f'timeseries.timeseries_exec_comp.{var}'
 
             else:
@@ -765,14 +758,15 @@
     transcription = phase.options['transcription']
 
     for ts_name, ts_opts in phase._timeseries.items():
 
         not_found = set()
 
         for output_name, output_options in ts_opts['outputs'].items():
+            name = output_options['name']
             if output_options['is_expr']:
                 output_meta = phase.timeseries_ec_vars[ts_name][output_name]['meta_data']
             else:
                 try:
                     output_meta = transcription._get_timeseries_var_source(output_options['name'],
                                                                            output_options['output_name'],
                                                                            phase=phase)
@@ -786,15 +780,15 @@
             if output_options['shape'] in (None, _unspecified):
                 output_options['shape'] = output_meta['shape']
 
             if output_options['units'] in (None, _unspecified):
                 output_options['units'] = output_meta['units']
 
         if not_found:
-            sorted_list = ', '.join(sorted(not_found))
+            sorted_list = ', '.join(sorted([ts_opts['outputs'][output_name]['name'] for output_name in not_found]))
             om.issue_warning(f'{phase.pathname}: The following timeseries outputs were requested but not found in the '
                              f'ODE: {sorted_list}')
 
         for s in not_found:
             ts_opts['outputs'].pop(s)
```

### Comparing `dymos-1.7.0/dymos/utils/lagrange.py` & `dymos-1.8.0/dymos/utils/lagrange.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/lg.py` & `dymos-1.8.0/dymos/utils/lg.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/lgl.py` & `dymos-1.8.0/dymos/utils/lgl.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/lgr.py` & `dymos-1.8.0/dymos/utils/lgr.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/misc.py` & `dymos-1.8.0/dymos/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/test/test_hermite.py` & `dymos-1.8.0/dymos/utils/test/test_hermite.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/test/test_indexing.py` & `dymos-1.8.0/dymos/utils/test/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/test/test_introspection.py` & `dymos-1.8.0/dymos/utils/test/test_introspection.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/test/test_lg.py` & `dymos-1.8.0/dymos/utils/test/test_lg.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/test/test_lgl.py` & `dymos-1.8.0/dymos/utils/test/test_lgl.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/test/test_lgr.py` & `dymos-1.8.0/dymos/utils/test/test_lgr.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/test/test_misc.py` & `dymos-1.8.0/dymos/utils/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/test/test_testing_utils.py` & `dymos-1.8.0/dymos/utils/test/test_testing_utils.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/utils/testing_utils.py` & `dymos-1.8.0/dymos/utils/testing_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import builtins
 import io
 import os
 
 from packaging.version import Version
 
 import numpy as np
```

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageCellRenderer.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageCellRenderer.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageDiagram.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageDiagram.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageLegend.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageLegend.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageMatrix.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageMatrix.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageMatrixCell.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageMatrixCell.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageModelData.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageModelData.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageStyle.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageStyle.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageSymbolType.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageSymbolType.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageTreeNode.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageTreeNode.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkageUserInterface.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkageUserInterface.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/js/DmLinkage_main.js` & `dymos-1.8.0/dymos/visualization/linkage/js/DmLinkage_main.js`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/report.py` & `dymos-1.8.0/dymos/visualization/linkage/report.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/report_template.html` & `dymos-1.8.0/dymos/visualization/linkage/report_template.html`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/style/linkage_report.css` & `dymos-1.8.0/dymos/visualization/linkage/style/linkage_report.css`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/linkage/test/linkage_report_ui_test.py` & `dymos-1.8.0/dymos/visualization/linkage/test/linkage_report_ui_test.py`

 * *Files identical despite different names*

### Comparing `dymos-1.7.0/dymos/visualization/test/test_timeseries_plots.py` & `dymos-1.8.0/dymos/visualization/test/test_timeseries_plots.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,65 +76,96 @@
         p['traj0.phase0.parameters:g'] = 9.80665
 
         p.setup()
 
         self.p = p
 
     def test_brachistochrone_timeseries_plots(self):
+        temp = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
+
         dm.run_problem(self.p, make_plots=False)
 
         timeseries_plots('dymos_solution.db', problem=self.p)
         plot_dir = pathlib.Path(_get_reports_dir(self.p)).joinpath('plots')
 
         self.assertTrue(plot_dir.joinpath('states_x.png').exists())
         self.assertTrue(plot_dir.joinpath('states_y.png').exists())
         self.assertTrue(plot_dir.joinpath('states_v.png').exists())
         self.assertTrue(plot_dir.joinpath('controls_theta.png').exists())
         self.assertTrue(plot_dir.joinpath('control_rates_theta_rate.png').exists())
         self.assertTrue(plot_dir.joinpath('control_rates_theta_rate2.png').exists())
 
+        dm.options['plots'] = temp
+
     def test_brachistochrone_timeseries_plots_solution_only_set_solution_record_file(self):
+        temp = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
+
         # records to the default file 'dymos_simulation.db'
         dm.run_problem(self.p, make_plots=False, solution_record_file='solution_record_file.db')
 
         timeseries_plots('solution_record_file.db', problem=self.p)
         plot_dir = pathlib.Path(_get_reports_dir(self.p)).joinpath('plots')
 
         self.assertTrue(plot_dir.joinpath('states_x.png').exists())
         self.assertTrue(plot_dir.joinpath('states_y.png').exists())
         self.assertTrue(plot_dir.joinpath('states_v.png').exists())
         self.assertTrue(plot_dir.joinpath('controls_theta.png').exists())
         self.assertTrue(plot_dir.joinpath('control_rates_theta_rate.png').exists())
         self.assertTrue(plot_dir.joinpath('control_rates_theta_rate2.png').exists())
 
+        dm.options['plots'] = temp
+
     def test_brachistochrone_timeseries_plots_solution_and_simulation(self):
+        temp = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
+
         dm.run_problem(self.p, simulate=True, make_plots=False,
                        simulation_record_file='simulation_record_file.db')
 
         timeseries_plots('dymos_solution.db', simulation_record_file='simulation_record_file.db', problem=self.p)
 
+        plot_dir = pathlib.Path(_get_reports_dir(self.p)).joinpath("plots").resolve()
+        self.assertTrue(plot_dir.joinpath('states_x.png').exists())
+        self.assertTrue(plot_dir.joinpath('states_y.png').exists())
+        self.assertTrue(plot_dir.joinpath('states_v.png').exists())
+        self.assertTrue(plot_dir.joinpath('controls_theta.png').exists())
+        self.assertTrue(plot_dir.joinpath('control_rates_theta_rate.png').exists())
+        self.assertTrue(plot_dir.joinpath('control_rates_theta_rate2.png').exists())
+
+        dm.options['plots'] = temp
+
     def test_brachistochrone_timeseries_plots_set_plot_dir(self):
+
+        temp = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
+
         dm.run_problem(self.p, make_plots=False)
 
         plot_dir = pathlib.Path(_get_reports_dir(self.p)).joinpath("test_plot_dir").resolve()
         timeseries_plots('dymos_solution.db', plot_dir=plot_dir, problem=self.p)
 
         self.assertTrue(plot_dir.joinpath('states_x.png').exists())
         self.assertTrue(plot_dir.joinpath('states_y.png').exists())
         self.assertTrue(plot_dir.joinpath('states_v.png').exists())
         self.assertTrue(plot_dir.joinpath('controls_theta.png').exists())
         self.assertTrue(plot_dir.joinpath('control_rates_theta_rate.png').exists())
         self.assertTrue(plot_dir.joinpath('control_rates_theta_rate2.png').exists())
 
+        dm.options['plots'] = temp
+
 
 @use_tempdirs
 class TestTimeSeriesPlotsMultiPhase(unittest.TestCase):
 
     @require_pyoptsparse(optimizer='IPOPT')
     def test_trajectory_linked_phases_make_plot(self):
+        temp = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
 
         self.traj = dm.Trajectory()
         p = self.p = om.Problem(model=self.traj)
 
         p.driver = om.pyOptSparseDriver()
         p.driver.options['optimizer'] = 'IPOPT'
         p.driver.declare_coloring()
@@ -217,14 +248,18 @@
         self.traj.link_phases(phases=['burn1', 'coast', 'burn2'],
                               vars=['time', 'r', 'theta', 'vr', 'vt', 'deltav'])
         self.traj.link_phases(phases=['burn1', 'burn2'], vars=['accel'])
 
         # Finish Problem Setup
         p.model.linear_solver = om.DirectSolver()
 
+        for phase_name, phase in self.traj._phases.items():
+            phase.timeseries_options['include_state_rates'] = True
+            phase.timeseries_options['include_t_phase'] = True
+
         p.setup(check=True)
 
         # Set Initial Guesses
 
         p.set_val('burn1.t_initial', value=0.0)
         p.set_val('burn1.t_duration', value=2.25)
 
@@ -267,20 +302,25 @@
                          problem=p)
         plot_dir = pathlib.Path(_get_reports_dir(p)).joinpath("plots")
 
         for varname in ['time_phase', 'states:r', 'state_rates:r', 'states:theta',
                         'state_rates:theta', 'states:vr', 'state_rates:vr', 'states:vt',
                         'state_rates:vt', 'states:accel',
                         'state_rates:accel', 'states:deltav', 'state_rates:deltav',
-                        'controls:u1', 'control_rates:u1_rate', 'control_rates:u1_rate2',
-                        'parameters:c']:
-            self.assertTrue(plot_dir.joinpath(varname.replace(":", "_") + '.png').exists())
+                        'controls:u1', 'control_rates:u1_rate', 'control_rates:u1_rate2']:
+            plotfile = plot_dir.joinpath(varname.replace(":", "_") + '.png')
+            self.assertTrue(plotfile.exists(), msg=f'{plotfile} does not exist!')
+
+        dm.options['plots'] = temp
 
     def test_overlapping_phases_make_plot(self):
 
+        _temp = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
+
         prob = om.Problem()
 
         opt = prob.driver = om.ScipyOptimizeDriver()
         opt.declare_coloring()
         opt.options['optimizer'] = 'SLSQP'
 
         num_seg = 5
@@ -331,14 +371,18 @@
         traj.link_phases(phases=['phase0', 'phase1'], vars=['state_of_charge', 'time'])
         traj.link_phases(phases=['phase0', 'phase1_bfail'], vars=['state_of_charge', 'time'])
         traj.link_phases(phases=['phase0', 'phase1_mfail'], vars=['state_of_charge', 'time'])
 
         prob.model.options['assembled_jac_type'] = 'csc'
         prob.model.linear_solver = om.DirectSolver(assemble_jac=True)
 
+        for phase_name, phase in traj._phases.items():
+            phase.timeseries_options['include_t_phase'] = True
+            phase.timeseries_options['include_state_rates'] = True
+
         prob.setup()
 
         prob['traj.phase0.t_initial'] = 0
         prob['traj.phase0.t_duration'] = 1.0*3600
 
         prob['traj.phase1.t_initial'] = 1.0*3600
         prob['traj.phase1.t_duration'] = 1.0*3600
@@ -357,20 +401,24 @@
                          problem=prob)
         plot_dir = pathlib.Path(_get_reports_dir(prob)).joinpath("plots")
 
         self.assertTrue(plot_dir.joinpath('time_phase.png').exists())
         self.assertTrue(plot_dir.joinpath('states_state_of_charge.png').exists())
         self.assertTrue(plot_dir.joinpath('state_rates_state_of_charge.png').exists())
 
+        dm.options['plots'] = _temp
+
     @require_pyoptsparse(optimizer='IPOPT')
     def test_trajectory_linked_phases_make_plot_missing_data(self):
         """
         Test that plots are still generated even if the phases don't share the exact same
         variables in the timeseries.
         """
+        temp = dm.options['plots']
+        dm.options['plots'] = 'matplotlib'
 
         self.traj = dm.Trajectory()
         p = self.p = om.Problem(model=self.traj)
 
         p.driver = om.pyOptSparseDriver()
         p.driver.options['optimizer'] = 'IPOPT'
         p.driver.declare_coloring()
@@ -392,15 +440,15 @@
                         rate_source='vt_dot', targets=['vt'], units='DU/TU')
         burn1.add_state('accel', fix_initial=True, fix_final=False,
                         rate_source='at_dot', targets=['accel'], units='DU/TU**2')
         burn1.add_state('deltav', fix_initial=True, fix_final=False,
                         rate_source='deltav_dot', units='DU/TU')
         burn1.add_control('u1', targets=['u1'], rate_continuity=True, rate2_continuity=True,
                           units='deg', scaler=0.01, lower=-30, upper=30)
-        burn1.add_parameter('c', opt=False, val=1.5, targets=['c'], units='DU/TU')
+        burn1.add_parameter('c', opt=False, val=1.5, targets=['c'], units='DU/TU', include_timeseries=True)
 
         # Second Phase (Coast)
 
         coast = dm.Phase(ode_class=FiniteBurnODE, transcription=dm.GaussLobatto(num_segments=10,
                                                                                 order=3))
 
         self.traj.add_phase('coast', coast)
@@ -415,16 +463,16 @@
                         rate_source='vr_dot', targets=['vr'], units='DU/TU')
         coast.add_state('vt', fix_initial=False, fix_final=False, defect_scaler=100.0,
                         rate_source='vt_dot', targets=['vt'], units='DU/TU')
         coast.add_state('accel', fix_initial=True, fix_final=True, ref=1.0E-12, defect_ref=1.0E-12,
                         rate_source='at_dot', targets=['accel'], units='DU/TU**2')
         coast.add_state('deltav', fix_initial=False, fix_final=False,
                         rate_source='deltav_dot', units='DU/TU')
-        coast.add_parameter('u1', targets=['u1'], opt=False, val=0.0, units='deg')
-        coast.add_parameter('c', opt=False, val=1.5, targets=['c'], units='DU/TU')
+        coast.add_parameter('u1', targets=['u1'], opt=False, val=0.0, units='deg', include_timeseries=True)
+        coast.add_parameter('c', opt=False, val=1.5, targets=['c'], units='DU/TU', include_timeseries=True)
 
         # Third Phase (burn)
 
         burn2 = dm.Phase(ode_class=FiniteBurnODE, transcription=dm.GaussLobatto(num_segments=3,
                                                                                 order=3))
 
         self.traj.add_phase('burn2', burn2)
@@ -441,26 +489,31 @@
                         rate_source='vt_dot', targets=['vt'], units='DU/TU')
         burn2.add_state('accel', fix_initial=False, fix_final=False, defect_ref=1.0E-6,
                         rate_source='at_dot', targets=['accel'], units='DU/TU**2')
         burn2.add_state('deltav', fix_initial=False, fix_final=False,
                         rate_source='deltav_dot', units='DU/TU')
         burn2.add_control('u1', targets=['u1'], rate_continuity=True, rate2_continuity=True,
                           units='deg', scaler=0.01, lower=-30, upper=30)
-        burn2.add_parameter('c', opt=False, val=1.5, targets=['c'], units='DU/TU')
+        burn2.add_parameter('c', opt=False, val=1.5, targets=['c'], units='DU/TU', include_timeseries=True)
 
         burn2.add_objective('deltav', loc='final')
 
         # Link Phases
         self.traj.link_phases(phases=['burn1', 'coast', 'burn2'],
                               vars=['time', 'r', 'theta', 'vr', 'vt', 'deltav'])
         self.traj.link_phases(phases=['burn1', 'burn2'], vars=['accel'])
 
         # Finish Problem Setup
         p.model.linear_solver = om.DirectSolver()
 
+        for phase_name, phase in self.traj._phases.items():
+            phase.timeseries_options['include_t_phase'] = True
+            phase.timeseries_options['include_state_rates'] = True
+            phase.timeseries_options['include_control_rates'] = True
+
         p.setup(check=True)
 
         # Set Initial Guesses
         p.set_val('burn1.t_initial', value=0.0)
         p.set_val('burn1.t_duration', value=2.25)
 
         p.set_val('burn1.states:r', value=burn1.interp('r', [1, 1.5]))
@@ -503,12 +556,15 @@
 
         for varname in ['time_phase', 'states:r', 'state_rates:r', 'states:theta',
                         'state_rates:theta', 'states:vr', 'state_rates:vr', 'states:vt',
                         'state_rates:vt', 'states:accel',
                         'state_rates:accel', 'states:deltav', 'state_rates:deltav',
                         'controls:u1', 'control_rates:u1_rate', 'control_rates:u1_rate2',
                         'parameters:c', 'parameters:u1']:
-            self.assertTrue(plot_dir.joinpath(varname.replace(":", "_") + '.png').exists())
+            self.assertTrue(plot_dir.joinpath(varname.replace(":", "_") + '.png').exists(),
+                            msg=plot_dir.joinpath(varname.replace(":", "_") + '.png does not exist!'))
+
+        dm.options['plots'] = temp
 
 
 if __name__ == '__main__':  # pragma: no cover
     unittest.main()
```

### Comparing `dymos-1.7.0/dymos/visualization/timeseries_plots.py` & `dymos-1.8.0/dymos/visualization/timeseries_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import matplotlib
 import matplotlib.pyplot as plt
 import matplotlib.lines as mlines
 import matplotlib.patches as mpatches
 
 import openmdao.api as om
-from dymos.options import options as dymos_options
+from .._options import options as dymos_options
 
 
 def _get_phases_node_in_problem_metadata(node, path=""):
     """
     Find the phases node in the Problem metadata hierarchy.
 
     There is one node in the hierarchy that has the name 'phases'. Finding this
@@ -49,23 +49,27 @@
                                                                                     new_path)
                 if phases_node:
                     return phases_node, phase_node_path
     return None, None
 
 
 def _mpl_timeseries_plots(time_units, var_units, phase_names, phases_node_path,
-                          last_solution_case, last_simulation_case, plot_dir_path):
+                          last_solution_case, last_simulation_case, plot_dir_path,
+                          dpi, include_parameters):
     # get ready to plot
     backend_save = plt.get_backend()
     plt.switch_backend('Agg')
     # use a colormap with 20 values
     cm = matplotlib.cm.get_cmap('tab20')
     plotfiles = []
 
     for var_name, var_unit in var_units.items():
+        if (not include_parameters) and ("parameters:" in var_name):
+            continue
+
         # start a new plot
         fig, ax = plt.subplots()
 
         # Get the labels
         time_label = f'time ({time_units[var_name]})'
         var_label = f'{var_name} ({var_unit})'
         title = f'timeseries.{var_name}'
@@ -129,15 +133,15 @@
         plt.legend(handles=handles, loc='upper right', ncol=len(phase_names), shadow=True,
                    bbox_to_anchor=(1.15, -0.12), title='Phases')
 
         plt.subplots_adjust(bottom=0.23, top=0.9, left=0.2)
 
         # save to file
         plot_file_path = plot_dir_path.joinpath(f'{var_name.replace(":","_")}.png')
-        plt.savefig(plot_file_path)
+        plt.savefig(plot_file_path, dpi=dpi)
         plt.close(fig)
         plotfiles.append(plot_file_path)
 
     plt.switch_backend(backend_save)
 
     return plotfiles
 
@@ -321,15 +325,15 @@
 
     </body>
     </html>
     """
 
 
 def timeseries_plots(solution_recorder_filename, simulation_record_file=None, plot_dir="plots",
-                     problem=None):
+                     problem=None, dpi=150, make_html=True, include_parameters=True):
     """
     Create plots of the timeseries.
 
     Given timeseries data from case recorder files, make separate plots of each variable
     and store the plot files in the directory indicated by the variable plot_dir
 
     Parameters
@@ -340,14 +344,22 @@
         The path to the case recorder file containing simulation data. If not None,
         this implies that the data from it should be plotted.
     plot_dir : str
         The path to the directory to which the plot files will be written.
     problem : Problem or None
         If not None, this is the owning Problem, and the plot_dir will be relative to the reports
         directory for this Problem.
+    dpi : float
+        The dpi (pixels per inch) for the matplotlib images to be saved. A larger dpi number
+        results in higher resolution images.
+    make_html : bool
+        If true, make .html files that wrap the generated images.
+    include_parameters : bool
+        If true, include parameters in the timeseries plots. It can be helpful to set this to false
+        for models with only static parameters that are uninteresting to plot.
     """
     # get ready to generate plot files
 
     if not pathlib.Path(plot_dir).is_absolute():
         if problem is None:
             plot_dir_path = pathlib.Path.cwd().joinpath(plot_dir)
         else:
@@ -417,16 +429,17 @@
         return
 
     if dymos_options['plots'] == 'bokeh':
         _bokeh_timeseries_plots(time_units, var_units, phase_names, phases_node_path,
                                 last_solution_case, last_simulation_case, plot_dir_path)
     elif dymos_options['plots'] == 'matplotlib':
         fnames = _mpl_timeseries_plots(time_units, var_units, phase_names, phases_node_path,
-                                       last_solution_case, last_simulation_case, plot_dir_path)
-        if problem is not None:
+                                       last_solution_case, last_simulation_case, plot_dir_path,
+                                       dpi, include_parameters)
+        if (problem is not None) and make_html:
             for name in fnames:
                 # create html files that wrap the image files
                 fpath = pathlib.Path(name).resolve()
                 htmlpath = str(fpath.parent.joinpath(fpath.stem + '.html'))
                 with open(htmlpath, 'w', encoding='utf-8') as f:
                     f.write(image2html(fpath.name))
     else:
```

### Comparing `dymos-1.7.0/dymos.egg-info/PKG-INFO` & `dymos-1.8.0/dymos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dymos
-Version: 1.7.0
+Version: 1.8.0
 Summary: Open-Source Optimization of Dynamic Multidisciplinary Systems
 Home-page: https://github.com/OpenMDAO/dymos
 License: Apache License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `dymos-1.7.0/dymos.egg-info/SOURCES.txt` & `dymos-1.8.0/dymos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 setup.py
 dymos/__init__.py
+dymos/_options.py
 dymos/load_case.py
-dymos/options.py
 dymos/run_problem.py
 dymos.egg-info/PKG-INFO
 dymos.egg-info/SOURCES.txt
 dymos.egg-info/dependency_links.txt
 dymos.egg-info/entry_points.txt
 dymos.egg-info/not-zip-safe
 dymos.egg-info/requires.txt
@@ -412,8 +412,10 @@
 dymos/visualization/linkage/js/DmLinkageUserInterface.js
 dymos/visualization/linkage/js/DmLinkage_main.js
 dymos/visualization/linkage/style/linkage_report.css
 dymos/visualization/linkage/test/__init__.py
 dymos/visualization/linkage/test/linkage_report_ui_test.py
 dymos/visualization/linkage/test/test_gui.py
 dymos/visualization/test/__init__.py
-dymos/visualization/test/test_timeseries_plots.py
+dymos/visualization/test/test_timeseries_plots.py
+dymos/visualization/timeseries/__init__.py
+dymos/visualization/timeseries/bokeh_timeseries_report.py
```

### Comparing `dymos-1.7.0/setup.py` & `dymos-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import find_packages, setup
 
 # Setup optional dependencies
 optional_dependencies = {
     'docs': [
         'matplotlib',
+        'bokeh',
         'jupyter',
-        'jupyter-book',
+        'jupyter-book==0.14',
         'nbconvert',
         'notebook',
         'ipython',
         'numpydoc>=1.1',
         'redbaron',
         'tabulate',
         'jaxlib',
@@ -17,14 +18,15 @@
     ],
     'notebooks': [
         'notebook',
         'tabulate',
         'ipython'
     ],
     'test': [
+        'packaging',
         'pycodestyle',
         'testflo>=1.3.6',
         'matplotlib',
         'numpydoc>=1.1',
         'playwright>=1.20',
         'aiounittest'
     ]
@@ -35,15 +37,15 @@
     dependency
     for dependencies in optional_dependencies.values()
     for dependency in dependencies
 ])
 
 
 setup(name='dymos',
-    version='1.7.0',
+    version='1.8.0',
     description='Open-Source Optimization of Dynamic Multidisciplinary Systems',
     long_description='''
 Dymos is a framework for the simulation and optimization of dynamical systems within the OpenMDAO Multidisciplinary Analysis and Optimization environment.
 Dymos leverages implicit and explicit simulation techniques to simulate generic dynamic systems of arbitary complexity.
 
 The software has two primary objectives:
 -   Provide a generic ODE integration interface that allows for the analysis of dynamical systems.
```

