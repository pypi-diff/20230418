# Comparing `tmp/pyiron_contrib-0.1.8.tar.gz` & `tmp/pyiron_contrib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_contrib-0.1.8.tar", last modified: Tue Mar 21 08:23:33 2023, max compression
+gzip compressed data, was "pyiron_contrib-0.1.9.tar", last modified: Tue Apr 18 20:31:07 2023, max compression
```

## Comparing `pyiron_contrib-0.1.8.tar` & `pyiron_contrib-0.1.9.tar`

### file list

```diff
@@ -1,132 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.580240 pyiron_contrib-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-21 08:23:33.580240 pyiron_contrib-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.580240 pyiron_contrib-0.1.8/pyiron_contrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.568240 pyiron_contrib-0.1.8/pyiron_contrib/RDM/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/RDM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/RDM/storagejob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-21 08:23:33.580240 pyiron_contrib-0.1.8/pyiron_contrib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.568240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.568240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/atomicrex_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/fit_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    52872 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/function_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    22489 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/general_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    45580 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/potential_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    33933 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/structure_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.568240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.568240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomistics/job/structurelistmasterinteractive.py
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomistics/job/trainingcontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.572240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/cp2k/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/cp2k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/cp2k/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.572240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/dft/parametermaster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.572240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/fitsnap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/fitsnap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.572240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/interactive/langevin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/interactive/mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/interactive/montecarlo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.572240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/ml/potentialfit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.572240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/cfgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/masters.py
--rw-r--r--   0 runner    (1001) docker     (123)    30653 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/mlip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/mlipjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/mlipselect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/potential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.572240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/pacemaker/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.572240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/randspg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/randspg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/randspg/randspg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.572240 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22659 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/runner/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/runner/storageclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/atomistics/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.572240 pyiron_contrib-0.1.8/pyiron_contrib/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20156 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/generic/s3io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.576240 pyiron_contrib-0.1.8/pyiron_contrib/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/image/custom_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/image/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/image/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/image/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.576240 pyiron_contrib-0.1.8/pyiron_contrib/nofiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/nofiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/nofiles/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/nofiles/lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18228 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/nofiles/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/nofiles/murn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/nofiles/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/nofiles/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.576240 pyiron_contrib-0.1.8/pyiron_contrib/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.576240 pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38061 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/finite_temperature_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22843 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/molecular_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/nudged_elastic_band.py
--rw-r--r--   0 runner    (1001) docker     (123)    28964 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/qmmm.py
--rw-r--r--   0 runner    (1001) docker     (123)   102721 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/thermodynamic_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    43034 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.576240 pyiron_contrib-0.1.8/pyiron_contrib/protocol/primitive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/primitive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/primitive/fts_vertices.py
--rw-r--r--   0 runner    (1001) docker     (123)    68762 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/primitive/one_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/primitive/two_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.580240 pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/comparers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/pptree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.580240 pyiron_contrib-0.1.8/pyiron_contrib/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/workflow/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/workflow/has_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/workflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/workflow/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/workflow/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/workflow/type_hinting.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/workflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/pyiron_contrib/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 08:23:33.568240 pyiron_contrib-0.1.8/pyiron_contrib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-21 08:23:33.000000 pyiron_contrib-0.1.8/pyiron_contrib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-03-21 08:23:33.000000 pyiron_contrib-0.1.8/pyiron_contrib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 08:23:33.000000 pyiron_contrib-0.1.8/pyiron_contrib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-21 08:23:33.000000 pyiron_contrib-0.1.8/pyiron_contrib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-21 08:23:33.000000 pyiron_contrib-0.1.8/pyiron_contrib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-21 08:23:33.580240 pyiron_contrib-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-21 08:23:33.000000 pyiron_contrib-0.1.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68610 2023-03-21 08:23:30.000000 pyiron_contrib-0.1.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.798342 pyiron_contrib-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-18 20:31:07.798342 pyiron_contrib-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.798342 pyiron_contrib-0.1.9/pyiron_contrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.782341 pyiron_contrib-0.1.9/pyiron_contrib/RDM/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/RDM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/RDM/storagejob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-18 20:31:07.798342 pyiron_contrib-0.1.9/pyiron_contrib/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.782341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.786341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/atomicrex_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/fit_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52872 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/function_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22489 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/general_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/parameter_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45580 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/potential_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33933 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/structure_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.786341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.786341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomistics/job/structurelistmasterinteractive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomistics/job/trainingcontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.786341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/cp2k/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/cp2k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/cp2k/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.786341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/dft/parametermaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.786341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/fitsnap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/fitsnap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.786341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/interactive/langevin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/interactive/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/interactive/montecarlo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.786341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/ml/potentialfit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.790341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/cfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/masters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30653 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/mlip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/mlipjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/mlipselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/potential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.790341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/pacemaker/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.790341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/randspg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/randspg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/randspg/randspg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.790341 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22659 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/runner/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/runner/storageclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/atomistics/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.790341 pyiron_contrib-0.1.9/pyiron_contrib/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/generic/coscineIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/generic/filedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22063 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/generic/s3io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/generic/storage_interface_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.790341 pyiron_contrib-0.1.9/pyiron_contrib/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/image/custom_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/image/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/image/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.790341 pyiron_contrib-0.1.9/pyiron_contrib/nofiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/nofiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/nofiles/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/nofiles/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/nofiles/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/nofiles/murn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/nofiles/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/nofiles/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.794342 pyiron_contrib-0.1.9/pyiron_contrib/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.794342 pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38061 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/finite_temperature_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22843 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/molecular_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/nudged_elastic_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28964 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/qmmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102721 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/thermodynamic_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43034 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.794342 pyiron_contrib-0.1.9/pyiron_contrib/protocol/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/primitive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/primitive/fts_vertices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68762 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/primitive/one_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/primitive/two_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.794342 pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/comparers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/pptree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.798342 pyiron_contrib-0.1.9/pyiron_contrib/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/workflow/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/workflow/has_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/workflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16104 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/workflow/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/workflow/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/workflow/type_hinting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/workflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/pyiron_contrib/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:07.782341 pyiron_contrib-0.1.9/pyiron_contrib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-18 20:31:07.000000 pyiron_contrib-0.1.9/pyiron_contrib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-04-18 20:31:07.000000 pyiron_contrib-0.1.9/pyiron_contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:31:07.000000 pyiron_contrib-0.1.9/pyiron_contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-18 20:31:07.000000 pyiron_contrib-0.1.9/pyiron_contrib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 20:31:07.000000 pyiron_contrib-0.1.9/pyiron_contrib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-18 20:31:07.798342 pyiron_contrib-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-18 20:31:07.000000 pyiron_contrib-0.1.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68610 2023-04-18 20:31:04.000000 pyiron_contrib-0.1.9/versioneer.py
```

### Comparing `pyiron_contrib-0.1.8/LICENSE` & `pyiron_contrib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/PKG-INFO` & `pyiron_contrib-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_contrib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_contrib
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/RDM/storagejob.py` & `pyiron_contrib-0.1.9/pyiron_contrib/RDM/storagejob.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     Attributes:
        storage_type(str): type of the storage, one of _available_storage_types
        local(bool): storage_type == 'local'
        s3(bool): storage_type == 's3'
        read_only (bool): read only StorageType cannot be changed
 
     """
-    _available_storage_types = ['local', 's3']
+
+    _available_storage_types = ["local", "s3"]
 
     def __init__(self, storage_type=None):
         """What type of storage is used
 
         Parameters:
             storage_type(str): one of ['local', 's3']
         """
@@ -43,46 +44,51 @@
         if self._read_only and not val:
             self._read_only_error()
         else:
             self._read_only = bool(val)
 
     @classmethod
     def _read_only_error(cls):
-        raise RuntimeError("The storage type cannot be changed when it is already in use.")
+        raise RuntimeError(
+            "The storage type cannot be changed when it is already in use."
+        )
 
     @property
     def local(self):
-        return self.storage_type == 'local'
+        return self.storage_type == "local"
 
     @property
     def s3(self):
-        return self.storage_type == 's3'
+        return self.storage_type == "s3"
 
     @property
     def storage_type(self):
         return self._storage_type
 
     @storage_type.setter
     def storage_type(self, storage_type):
         if self.read_only:
             self._read_only_error()
         if storage_type not in self._available_storage_types:
-            raise ValueError(f"Expected 'storage_type' to be one of {self._available_storage_types} "
-                             f"but got {storage_type}.")
+            raise ValueError(
+                f"Expected 'storage_type' to be one of {self._available_storage_types} "
+                f"but got {storage_type}."
+            )
         self._storage_type = storage_type
 
 
 class StorageJob(GenericJob):
     """Job to store files associated with meta data either locally, or at a remote data service like s3."""
+
     def __init__(self, project, job_name):
 
         super().__init__(project, job_name)
         self.server.run_mode.interactive = True
-        self._stored_files = DataContainer(table_name='stored_files')
-        self._storage_type = StorageType(storage_type='local')
+        self._stored_files = DataContainer(table_name="stored_files")
+        self._storage_type = StorageType(storage_type="local")
         self._storage_type_store = DataContainer(table_name="storage_type")
         self._external_storage = None
 
     def _before_generic_remove_child(self):
         if self._storage_type.s3 and self._external_storage.is_dir(self.path):
             self._external_storage.remove_group(path=self.path)
 
@@ -97,43 +103,49 @@
         TODO:
         - overwrite run_if_scheduler to not trigger a job to be run on the queing system.
         - make some file_handler class to allow for 'store/receive/delete file' with a uniform interface for
             - local
             - s3
             - ssh
         """
-        raise NotImplementedError("Storing files remotely via ssh is not yet supported.")
+        raise NotImplementedError(
+            "Storing files remotely via ssh is not yet supported."
+        )
 
     @property
     def storage_type(self):
         return self._storage_type.storage_type
 
     def use_s3_storage(self, config=None, bucket_name=None, _only_warn=False):
-        external_storage = FileS3IO(config=config, path=self.path, bucket_name=bucket_name)
+        external_storage = FileS3IO(
+            config=config, path=self.path, bucket_name=bucket_name
+        )
         if len(external_storage.list_nodes() + external_storage.list_groups()) > 0:
             if not _only_warn:
                 raise ValueError("Storage location not empty.")
             else:
                 self._logger.warning("Storage NOT empty - Danger of data loss!")
         self._external_storage = external_storage
-        self._storage_type.storage_type = 's3'
+        self._storage_type.storage_type = "s3"
         self._storage_type_store.create_group("s3_config")
         self._storage_type_store.s3_config.config = config
-        self._storage_type_store.s3_config.bucket_info = self._external_storage.bucket_info
+        self._storage_type_store.s3_config.bucket_info = (
+            self._external_storage.connection_info
+        )
         self._storage_type_store.s3_config.bucket_name = bucket_name
 
     def _list_groups(self):
         return []
 
     def _list_nodes(self):
         return self.files_stored
 
     def use_local_storage(self):
-        self._storage_type.storage_type = 'local'
-        if 's3_config' in self._storage_type_store.keys():
+        self._storage_type.storage_type = "local"
+        if "s3_config" in self._storage_type_store.keys():
             del self._storage_type_store.s3_config
         self._external_storage = None
 
     @property
     def files_stored(self):
         return [key for key in self._stored_files.keys()]
 
@@ -159,36 +171,40 @@
             overwrite(bool): if true to overwrite already present files
         """
         if self.status.initialized:
             self.run()
         if isinstance(filenames, str):
             filenames = [filenames]
         if isinstance(metadata, list) and len(metadata) != len(filenames):
-            raise ValueError(f"Length of filenames and metadata have to match, "
-                             f"but got len(filenames)={len(filenames)} and len(metadata)={len(metadata)}.")
+            raise ValueError(
+                f"Length of filenames and metadata have to match, "
+                f"but got len(filenames)={len(filenames)} and len(metadata)={len(metadata)}."
+            )
 
         files = [os.path.basename(file) for file in filenames]
         if len(set(files)) != len(files):
             raise ValueError(f"Resulting filenames {files} have duplicates.")
 
         for i, file in enumerate(filenames):
             if not overwrite and os.path.basename(file) in self._stored_files.keys():
-                self._logger.warning(f"{file} not copied, since already present and 'overwrite'=False.")
+                self._logger.warning(
+                    f"{file} not copied, since already present and 'overwrite'=False."
+                )
                 continue
             _metadata = metadata[i] if isinstance(metadata, list) else metadata
             self._store_file(file, _metadata)
 
         self.run()
 
     def _store_file(self, file, metadata):
         try:
             if self._storage_type.local:
                 shutil.copy(file, self.working_directory)
             elif self._storage_type.s3:
-                self._external_storage.upload(file, metadata)
+                self._external_storage.upload_file(file, metadata)
         except Exception as e:
             raise IOError(f"Storing {file} failed") from e
         else:
             self._stored_files[os.path.basename(file)] = metadata
 
     def _remove_file(self, file):
         try:
@@ -212,31 +228,33 @@
             silent(bool):                   If true, do not print the status message.
         """
         if isinstance(filenames, str):
             filenames = [filenames]
 
         files_not_found = [file for file in filenames if file not in self._stored_files]
         if len(files_not_found) > 0 and raise_error:
-            raise FileNotFoundError(f"Files {files_not_found} not found, abort removing files. You may specify "
-                                    f"raise_error=False to suppress this error.")
+            raise FileNotFoundError(
+                f"Files {files_not_found} not found, abort removing files. You may specify "
+                f"raise_error=False to suppress this error."
+            )
 
         files_to_remove = [file for file in filenames if file in self._stored_files]
         if dryrun and not silent:
             print(f"dryrun: to remove {files_to_remove} specify dryrun=False")
             return
 
         for file in files_to_remove:
             self._remove_file(file)
 
         if not silent:
             print(f"removed {files_to_remove}")
         self.run()
 
     def run_static(self):
-        raise NotImplementedError('There is no static run mode for a Storage job.')
+        raise NotImplementedError("There is no static run mode for a Storage job.")
 
     def collect_output(self):
         pass
 
     def run_if_interactive(self):
         self.status.running = True
         self.to_hdf()
@@ -260,39 +278,42 @@
         pass
 
     def reconnect_s3_storage(self, config=None, bucket_name=None):
         config = config or self._storage_type_store.s3_config.config
         bucket_name = bucket_name or self._storage_type_store.s3_config.bucket_name
         try:
             external_storage = FileS3IO(
-                config=config,
-                path=self.path,
-                bucket_name=bucket_name
+                config=config, path=self.path, bucket_name=bucket_name
             )
         except Exception as e:
             raise RuntimeError("Could not restore connection to the S3 storage.") from e
-        if self._storage_type_store.s3_config.bucket_info == external_storage.bucket_info:
+        if (
+            self._storage_type_store.s3_config.bucket_info
+            == external_storage.connection_info
+        ):
             self._external_storage = external_storage
         else:
-            raise RuntimeError(f"New and saved s3 storage do not match! Got {external_storage.bucket_info}"
-                               f" but expected {self._storage_type_store.s3_config.bucket_info}.")
+            raise RuntimeError(
+                f"New and saved s3 storage do not match! Got {external_storage.connection_info}"
+                f" but expected {self._storage_type_store.s3_config.connection_info}."
+            )
 
     def from_hdf(self, hdf=None, group_name=None):
         super().from_hdf(hdf, group_name)
         self._stored_files.from_hdf(hdf=self._hdf5)
         self._storage_type_store.from_hdf(hdf=self._hdf5)
         self._storage_type = StorageType(self._storage_type_store.storage_type)
         self._storage_type.read_only = self._storage_type_store.fixed_storage_type
         if self._storage_type.s3 and self.status != "initialized":
             self.reconnect_s3_storage()
 
     def to_hdf(self, hdf=None, group_name=None):
         super().to_hdf(hdf, group_name)
         if self._storage_type.s3:
-            self._hdf5['REQUIRE_FULL_OBJ_FOR_RM'] = True
+            self._hdf5["REQUIRE_FULL_OBJ_FOR_RM"] = True
         self._stored_files.to_hdf(hdf=self._hdf5)
         self._storage_type_store.storage_type = self.storage_type
         self._storage_type_store.fixed_storage_type = self._storage_type.read_only
         self._storage_type_store.to_hdf(hdf=self._hdf5)
 
     def __getitem__(self, item):
         # copied from super().__getitem__ changing the output of returning a file
@@ -319,13 +340,15 @@
 
         name_lst = item.split("/")
         item_obj = name_lst[0]
 
         # Here this function is changed to return a FileData object.
         if self._storage_type.local:
             if name_lst[0] in self.list_files():
-                file_name = posixpath.join(self.working_directory, "{}".format(item_obj))
+                file_name = posixpath.join(
+                    self.working_directory, "{}".format(item_obj)
+                )
                 return FileData(file=file_name, metadata=self._stored_files[item])
         elif self._storage_type.s3:
             if name_lst[0] in self._external_storage.list_nodes():
                 return self._external_storage[name_lst[0]]
         return None
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/__init__.py` & `pyiron_contrib-0.1.9/pyiron_contrib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 try:
 	from pyiron import Project
 except:
 	warnings.warn("pyiron module not found, importing Project from pyiron_base")
 	from pyiron_base import Project
 
 from pyiron_base import JOB_CLASS_DICT
+from pyiron_contrib.generic.storage_interface_toolkit import StorageInterfaceFactory
+
+Project.register_tools('storage_interface', StorageInterfaceFactory)
 
 # Make classes available for new pyiron version
 JOB_CLASS_DICT['ProtoMinimGradDes'] = 'pyiron_contrib.protocol.compound.minimize'
 JOB_CLASS_DICT['ProtoMD'] = 'pyiron_contrib.protocol.compound.molecular_dynamics'
 JOB_CLASS_DICT['ProtoConfinedMD'] = 'pyiron_contrib.protocol.compound.molecular_dynamics'
 JOB_CLASS_DICT['ProtoHarmMD'] = 'pyiron_contrib.protocol.compound.molecular_dynamics'
 JOB_CLASS_DICT['ProtoNEBSer'] = 'pyiron_contrib.protocol.compound.nudged_elastic_band'
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/base.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/base.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/fit_properties.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/fit_properties.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/function_factory.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/function_factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/general_input.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/general_input.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/interactive.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/parameter_constraints.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/potential_factory.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/potential_factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/structure_list.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/structure_list.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomicrex/utility_functions.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomicrex/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomistics/job/structurelistmasterinteractive.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomistics/job/structurelistmasterinteractive.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/atomistics/job/trainingcontainer.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/atomistics/job/trainingcontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/cp2k/job.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/cp2k/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/dft/parametermaster.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/dft/parametermaster.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/interactive/langevin.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/interactive/langevin.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/interactive/mixer.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/interactive/mixer.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/interactive/montecarlo.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/interactive/montecarlo.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/ml/potentialfit.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/ml/potentialfit.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,22 +142,22 @@
         de = abs(energy_train - energy_pred)
         rmse = np.sqrt((de**2).mean())
         mae  = de.mean()
         high = de.max()
         low  = de.min()
 
         ax = plt.gca()
-        trafo = ax.get_xaxis_transform(),
+        trafo = ax.get_xaxis_transform()
         def annotated_vline(x, text, linestyle='--'):
             plt.axvline(x, color='k', linestyle=linestyle)
             plt.text(
                     x=x, y=0.5, s=text,
                     transform=trafo,
                     rotation='vertical',
-                    horizontal_alignment='center',
+                    horizontalalignment='center',
                     path_effects=[withStroke(linewidth=4, foreground='w')],
             )
 
         plt.hist(
                 de,
                 bins=np.logspace(np.log10(low), np.log10(high), bins),
                 log=logy
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/cfgs.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/cfgs.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/lammps.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/lammps.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/masters.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/masters.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/mlip.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/mlip.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/mlipjob.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/mlipjob.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/mlipselect.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/mlipselect.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/parser.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/mlip/potential.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/mlip/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/pacemaker/job.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/pacemaker/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/randspg/randspg.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/randspg/randspg.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/runner/job.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/runner/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/runner/storageclasses.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/runner/storageclasses.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/atomistics/runner/utils.py` & `pyiron_contrib-0.1.9/pyiron_contrib/atomistics/runner/utils.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/generic/s3io.py` & `pyiron_contrib-0.1.9/pyiron_contrib/generic/s3io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
+# coding: utf-8
+# Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
+# Distributed under the terms of "New BSD License", see the LICENSE file.
+
 import fnmatch
 import io
 import json
 import os
 import posixpath
 from functools import lru_cache
 
 import boto3
 from botocore.client import Config
 
-from pyiron_base import HasGroups
-from pyiron_base import load_file, FileDataTemplate
+from pyiron_contrib.generic.filedata import StorageInterface
+from pyiron_contrib.generic.filedata import load_file, FileDataTemplate
 
 
 class S3FileData(FileDataTemplate):
     """FileData stores an instance of a data file from an S3 system, e.g. a single Image from a measurement."""
+
     def __init__(self, s3obj, filename=None, filetype=None):
         """FileData class to store data and associated metadata.
 
         Args:
             s3obj (s3object): s3object containing a file with data
             filename (str): filename associated with the data.
             filetype (str): File extension associated with the type data,
                             If provided this overwrites the assumption based on the extension of the filename.
         """
         self._s3obj = s3obj
         if filename is None:
-            self.filename = s3obj.key.split('/')[-1]
+            self.filename = s3obj.key.split("/")[-1]
         else:
             self.filename = filename
         if filetype is None:
-            filetype = os.path.splitext(self.filename)[1]
-            if filetype == '' or filetype == '.':
-                self.filetype = None
-            else:
-                self.filetype = filetype[1:]
+            self.filetype = self._get_filetype_from_filename(self.filename)
         else:
             self.filetype = filetype
         self._data = None
         self._metadata = self._s3obj.metadata
 
     @property
     @lru_cache()
@@ -63,56 +64,56 @@
         print(result)
 
 
 class S3ioConnect:
     def __init__(self, credentials=None, bucket_name=None):
         """Establishes connection to a specific 'bucket' of a S3 type object store.
 
-            Args:
-                credentials (str/dict/boto3.resource/None):
-                        if str: path to a json configuration file with login credentials for the bucket.
-                        if dict: dictionary containing the login credentials.
-                        if boto3.resource: This resource is used as is, requires bucket_name to be specified.
-                        if None: use Credentials as obtained by boto3, requires bucket_name to be specified.
-                bucket_name(str/None): Name of the bucket, overwrites name given in the config.
-
-            The credentials needs to provide the following information:
-                access_key or aws_access_key_id (str)
-                secret_key or aws_secret_access_key (str)
-            And may contain these additional fields:
-                endpoint or endpoint_url (str)
-                bucket (str)
-            Each additional keyword is passed on to boto3 as is.
+        Args:
+            credentials (str/dict/boto3.resource/None):
+                    if str: path to a json configuration file with login credentials for the bucket.
+                    if dict: dictionary containing the login credentials.
+                    if boto3.resource: This resource is used as is, requires bucket_name to be specified.
+                    if None: use Credentials as obtained by boto3, requires bucket_name to be specified.
+            bucket_name(str/None): Name of the bucket, overwrites name given in the config.
+
+        The credentials needs to provide the following information:
+            access_key or aws_access_key_id (str)
+            secret_key or aws_secret_access_key (str)
+        And may contain these additional fields:
+            endpoint or endpoint_url (str)
+            bucket (str)
+        Each additional keyword is passed on to boto3 as is.
         """
         self.bucket_name = None
         self.s3resource = self._init_s3resource(credentials)
 
         self.bucket_name = bucket_name or self.bucket_name
         self._check_for_bucket_name()
         self.bucket = self.s3resource.Bucket(self.bucket_name)
 
     def _init_s3resource(self, credentials):
         if isinstance(credentials, boto3.resources.base.ServiceResource):
             return credentials
         elif credentials is None:
             # boto3 looks for the (missing) credentials at  ~/.aws/credentials or at environment variables:
             # AWS_ACCESS_KEY_ID  AWS_SECRET_ACCESS_KEY  etc.
-            return boto3.resource('s3')
+            return boto3.resource("s3")
         else:
             credentials = self._get_credentials_dict(credentials)
 
-            config = credentials.pop('config', Config(s3={'addressing_style': 'path'}))
+            config = credentials.pop("config", Config(s3={"addressing_style": "path"}))
 
-            self._normalize_key(credentials, 'aws_access_key_id', 'access_key')
-            self._normalize_key(credentials, 'aws_secret_access_key', 'secret_key')
-            self._normalize_key(credentials, 'endpoint_url', 'endpoint')
+            self._normalize_key(credentials, "aws_access_key_id", "access_key")
+            self._normalize_key(credentials, "aws_secret_access_key", "secret_key")
+            self._normalize_key(credentials, "endpoint_url", "endpoint")
 
             self.bucket_name = credentials.pop("bucket", None)
 
-            return boto3.resource('s3', config=config, **credentials)
+            return boto3.resource("s3", config=config, **credentials)
 
     def _check_for_bucket_name(self):
         if self.bucket_name is None:
             raise ValueError("Bucket name needs to be provided.")
 
     @staticmethod
     def _normalize_key(credentials, key, alias_key):
@@ -122,23 +123,25 @@
 
     @staticmethod
     def _get_credentials_dict(credentials):
         if isinstance(credentials, str):
             with open(credentials) as json_file:
                 credentials = json.load(json_file)
         if not isinstance(credentials, dict):
-            raise TypeError(f"credentials is not one of the supported types but {type(credentials)}.")
+            raise TypeError(
+                f"credentials is not one of the supported types but {type(credentials)}."
+            )
         return credentials.copy()
 
     @property
     def endpoint_url(self):
         return self.s3resource.meta.client.meta.endpoint_url
 
 
-class FileS3IO(HasGroups):
+class FileS3IO(StorageInterface):
     """Provides access to a specific bucket of a S3 object store similar to a regular storage system.
 
     Implements :class:`.HasGroups`. Groups are 'Folders' in the S3 storage, nodes are file like objects.
 
     Files may be uploaded to the bucket using
         upload: upload a (list of) filenames to the current group of the bucket.
         put: upload a file like object to the specified path in the bucket.
@@ -147,17 +150,26 @@
         download: download (list of) files to the specified folder.
         get: receive a S3FileData from the storage
         get_s3_object: receive a native s3.Object from the store
         get_metadata: receive only the meta data from the specified file
 
     Attributes:
         s3_path: absolute path (starting with '/') inside the bucket, interpreting '/' as the directory separator.
-        bucket_info: dict with name and endpoint of the bucket.
+        connection_info: dict with name and endpoint of the bucket.
     """
-    def __init__(self, config=None, path='/', *, bucket_name=None):
+
+    @property
+    def _path(self):
+        return self.s3_path
+
+    @_path.setter
+    def _path(self, new_path):
+        self.s3_path = new_path
+
+    def __init__(self, config=None, path="/", *, bucket_name=None):
         """
         Establishes connection to a specific 'bucket' of a S3 type object store.
 
         Args:
             config (str/dict/:class:`S3IO_connect`/boto3.ressource/None):
                 Provides access information for the S3 type object store:
                     str: path to a json configuration file with login credentials for the bucket.
@@ -172,14 +184,16 @@
             {
             access_key : ""
             secret_key : ""
             endpoint : ""
             bucket : ""
             }
         """
+        super().__init__()
+        self._path = path
         self.history = [path]
         if isinstance(config, S3ioConnect):
             self._s3io = config
         else:
             self._s3io = S3ioConnect(credentials=config, bucket_name=bucket_name)
 
         self._bucket = self._s3io.bucket
@@ -205,58 +219,70 @@
             path (str): S3 path
         """
         if (path is None) or (path == ""):
             path = "/"
         self._s3_path = posixpath.normpath(path)
         if not posixpath.isabs(self._s3_path):
             self._s3_path = "/" + self._s3_path
-        if not self._s3_path[-1] == '/':
-            self._s3_path = self._s3_path + '/'
+        if not self._s3_path[-1] == "/":
+            self._s3_path = self._s3_path + "/"
 
     @property
     def _bucket_path(self):
         """
         The bucket object internally does not use a '/' to indicate the root group.
 
         Return:
             str: Internal path in the bucket.
         """
         return self._s3_path[1:]
 
     @property
-    def bucket_info(self):
-        return {'bucket_name': self._bucket.name,
-                'endpoint_url': self._s3io.endpoint_url}
+    def connection_info(self):
+        return {
+            "s3_path": self.s3_path,
+            "bucket_name": self._bucket.name,
+            "endpoint_url": self._s3io.endpoint_url,
+        }
+
+    @classmethod
+    def from_dict(cls, connection_dict: dict):
+        path = connection_dict.get('s3_path', '/')
+        config = {
+            'bucket': connection_dict.get('bucket_name', None),
+            'endpoint':  connection_dict.get('endpoint_url', None)
+        }
+        cls(config, path)
 
     def _list_groups(self):
         """
         List directories/groups in the current group.
 
         Returns:
             list: list of directory names.
         """
         groups = []
-        group_path_len = len(self._bucket_path.split('/')) - 1
+        group_path_len = len(self._bucket_path.split("/")) - 1
         for obj in self._list_objects():
-            rel_obj_path_spl = obj.key.split('/')[group_path_len:]
+            rel_obj_path_spl = obj.key.split("/")[group_path_len:]
             if len(rel_obj_path_spl) > 1:
                 if rel_obj_path_spl[0] not in groups:
                     groups.append(rel_obj_path_spl[0])
         return groups
 
     def _list_nodes(self):
         """
         List of 'files' ( string not followed by '/' ) in the current group.
 
         Returns:
             list: list of file names.
         """
         nodes = []
-        for obj in self._bucket.objects.filter(Prefix=self._bucket_path, Delimiter='/'):
-            nodes.append(obj.key.split('/')[-1])
+        for obj in self._bucket.objects.filter(Prefix=self._bucket_path, Delimiter="/"):
+            nodes.append(obj.key.split("/")[-1])
         return nodes
 
     def _to_abs_bucketpath(self, path):
         """Helper function to convert a given path to an absolute path inside the S3 bucket."""
         if path is None or "":
             path = self._bucket_path
         if posixpath.isabs(path):
@@ -272,16 +298,16 @@
         Args:
             path (str): path to check.
 
         Returns:
             bool: True if path is a directory.
         """
         path = self._to_abs_bucketpath(path)
-        if len(path) > 1 and path[-1] != '/':
-            path = path + '/'
+        if len(path) > 1 and path[-1] != "/":
+            path = path + "/"
         objs = list(self._bucket.objects.filter(Prefix=path))
         return len(objs) > 0
 
     def is_file(self, path):
         """
         Check if given path is a file.
 
@@ -324,38 +350,62 @@
         """Close current group and open previous group."""
         if len(self.history) > 1:
             del self.history[-1]
         elif len(self.history) == 1:
             self.history[0] = "/"
         self._s3_path = self.history[-1]
 
-    def upload(self, files, metadata=None):
+    def validate_metadata(self, metadata, raise_error=True):
+        if metadata is None:
+            return {}
+        elif not isinstance(metadata, dict) and raise_error:
+            raise ValueError(
+                f"Meta data needs to be a dict containing only strings but got type {type(metadata)}."
+            )
+        elif not isinstance(metadata, dict):
+            return None
+        elif not all([isinstance(i, str) for i in metadata]):
+            raise ValueError(f"Meta data only allows keywords of type 'str'.")
+
+    def upload_file(self, files, metadata=None, filenames=None):
         """
         Uploads files into the current group of the S3 object store.
 
         Arguments:
-            files (list/str) : List of filenames/ filename to upload
+            files (list/str) : file / List of files to upload
             metadata (dictionary): metadata of the files (Not nested, only "str" type)
+            filenames (list/str/None): Names the files should get
         """
-        if metadata is None:
-            metadata = {}
 
         if isinstance(files, str):
             files = [files]
 
-        for file in files:
-            [_, filename] = os.path.split(file)
+        if filenames is None:
+            filenames = [os.path.basename(file) for file in files]
+        elif isinstance(filenames, str):
+            filenames = [filenames]
+
+        if isinstance(metadata, list) and len(metadata) != len(files):
+            raise ValueError("length of files and meta data have to match!")
+        elif isinstance(metadata, list):
+            metadata = [self.validate_metadata(data) for data in metadata]
+        else:
+            tmp_metadata = self.validate_metadata(metadata)
+            metadata = [tmp_metadata for _ in filenames]
+
+        if len(filenames) != len(files):
+            raise ValueError("length of files and of filenames have to match!")
+
+        for file, filename, _metadata in zip(files, filenames, metadata):
 
             self._bucket.upload_file(
-                file,
-                self._bucket_path + filename,
-                {"Metadata": metadata}
+                file, self._bucket_path + filename, {"Metadata": _metadata}
             )
 
-    def download(self, files, targetpath="."):
+    def download_file(self, files, targetpath="."):
         """
         Download files from current group to local file system (current directory is default)
 
         Arguments:
             files (list/str): List of filenames in the S3 object store.
             targetpath (str): Path in the local data system, to which the files should be downloaded.
         """
@@ -416,20 +466,20 @@
             metadata(dict/None): metadata to be used (has to be a dictionary of type {"string": "string", }).
                   Provided metadata overwrites the one possibly present in the data object.
         """
         if self.is_dir(path):
             path = self._to_abs_bucketpath(path)
         else:
             raise ValueError("No valid path specified!")
-        if len(path) > 0 and path[-1] != '/':
-            path = path + '/'
+        if len(path) > 0 and path[-1] != "/":
+            path = path + "/"
 
         if filename is not None:
             filename_ = filename
-        elif hasattr(data_obj, 'name'):
+        elif hasattr(data_obj, "name"):
             filename_ = os.path.basename(data_obj.name)
         else:
             raise ValueError("No filename given.")
         path = path + filename_
 
         if metadata is None:
             metadata = {}
@@ -440,15 +490,15 @@
 
     def print_fileinfos(self):
         """
         Prints the filename, last modified date and size for all files in the current group,
         recursively including sub groups.
         """
         for obj in self._bucket.objects.filter(Prefix=self._bucket_path):
-            print(f'/{obj.key} {obj.last_modified} {obj.size} bytes')
+            print(f"/{obj.key} {obj.last_modified} {obj.size} bytes")
 
     def _list_all_files_of_bucket(self):
         return list(self._bucket.objects.all())
 
     def glob(self, path):
         """
         Return a list of paths matching a pathname pattern.
@@ -472,28 +522,28 @@
         """
         Prints filename, last_modified, and size of each file in the provided list of file objects.
 
         Args:
             filelist (list): List containing objects from a bucket.
         """
         for obj in filelist:
-            print(f'/{obj.key} {obj.last_modified} {obj.size} bytes')
+            print(f"/{obj.key} {obj.last_modified} {obj.size} bytes")
 
     def remove_file(self, file):
         """
         Deletes the object associated with a file.
 
         Args:
             file (str/None): path like string to the file to be removed.
         """
         if not self.is_file(file):
             raise ValueError(f"{file} is not a file.")
         file = self._to_abs_bucketpath(file)
         self._bucket.Object(file).delete()
-        #self._remove_object(prefix=file, debug=debug)
+        # self._remove_object(prefix=file, debug=debug)
 
     def remove_group(self, path=None, debug=False):
         """
         Deletes the current group with all it's content recursively.
 
         Args:
             path (str/None): group to be removed recursively.
@@ -511,27 +561,29 @@
         Deletes all objects matching the provided prefix.
 
         Args:
             prefix(str): All objects with this prefix will be removed.
             debug(bool): If True, additional information is printed.
         """
         if debug:
-            print(f'\nDeleting all objects with sample prefix {self._bucket.name}/{prefix}.')
+            print(
+                f"\nDeleting all objects with sample prefix {self._bucket.name}/{prefix}."
+            )
         delete_responses = self._bucket.objects.filter(Prefix=prefix).delete()
         if debug:
             for delete_response in delete_responses:
-                for deleted in delete_response['Deleted']:
+                for deleted in delete_response["Deleted"]:
                     print(f'\t Deleted: {deleted["Key"]}')
 
     def __enter__(self):
         """Compatibility function for the with statement."""
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        """ Compatibility function for the with statement."""
+        """Compatibility function for the with statement."""
         self.close()
 
     def __repr__(self):
         """
         Human readable string representation.
 
         Return:
@@ -560,14 +612,13 @@
                     return self.get(item)
                 if item in self.list_groups():
                     return self.open(item)
                 raise ValueError(f"Unknown item: {item}")
             else:
                 item_abs_lst = (
                     os.path.normpath(os.path.join(self.s3_path, item))
-                        .replace("\\", "/")
-                        .split("/")
+                    .replace("\\", "/")
+                    .split("/")
                 )
                 s3_object = self.copy()
                 s3_object.s3_path = "/".join(item_abs_lst[:-1])
                 return s3_object[item_abs_lst[-1]]
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/image/custom_filters.py` & `pyiron_contrib-0.1.9/pyiron_contrib/image/custom_filters.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/image/image.py` & `pyiron_contrib-0.1.9/pyiron_contrib/image/image.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/image/job.py` & `pyiron_contrib-0.1.9/pyiron_contrib/image/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/image/utils.py` & `pyiron_contrib-0.1.9/pyiron_contrib/image/utils.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/nofiles/elastic.py` & `pyiron_contrib-0.1.9/pyiron_contrib/nofiles/elastic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-from pyiron_base import GenericMaster
+from pyiron_base import GenericMaster, state
 from pyiron_gpl.elastic.elastic import ElasticMatrixJob
 
 
 class ElasticMatrixJobWithoutFiles(ElasticMatrixJob):
     def __init__(self, project, job_name):
+        if not state.database.database_is_disabled:
+            raise RuntimeError(
+                "To run a `Without` job, the database must first be disabled. Please "
+                "`from pyiron_base import state; "
+                "state.update({'disable_database': True})`, and try again."
+            )
         super(ElasticMatrixJobWithoutFiles, self).__init__(project, job_name)
-        self._interactive_disable_log_file = False
+        self._interactive_disable_log_file = True
 
     @property
     def child_project(self):
         """
         :class:`.Project`: project which holds the created child jobs
         """
         if not self._interactive_disable_log_file:
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/nofiles/lammps.py` & `pyiron_contrib-0.1.9/pyiron_contrib/nofiles/lammps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import os
 import importlib
 from pyiron_atomistics.lammps.interactive import LammpsInteractive
+from pyiron_base import state
 
 try:  # mpi4py is only supported on Linux and Mac Os X
     from pylammpsmpi import LammpsLibrary
 except ImportError:
     pass
 
 
 class LammpsInteractiveWithoutOutput(LammpsInteractive):
     def __init__(self, project, job_name):
-        super(LammpsInteractiveWithoutOutput, self).__init__(project, job_name)
-        self._interactive_disable_log_file = False
+        if not state.database.database_is_disabled:
+            raise RuntimeError(
+                "To run a `Without` job, the database must first be disabled. Please "
+                "`from pyiron_base import state; "
+                "state.update({'disable_database': True})`, and try again."
+            )
+        super().__init__(project, job_name)
+        self._interactive_disable_log_file = True
 
     def to_hdf(self, hdf=None, group_name=None):
         """
 
         Args:
             hdf:
             group_name:
@@ -60,12 +67,12 @@
                 ["p" if coord else "f" for coord in self.structure.pbc]
             )
         self._reset_interactive_run_command()
         self.interactive_structure_setter(self.structure)
 
     def interactive_close(self):
         if not self._interactive_disable_log_file:
-            super(LammpsInteractiveWithoutOutput).interactive_close()
+            super().interactive_close()
 
     def refresh_job_status(self):
         if not self._interactive_disable_log_file:
-            super(LammpsInteractiveWithoutOutput).refresh_job_status()
+            super().refresh_job_status()
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/nofiles/master.py` & `pyiron_contrib-0.1.9/pyiron_contrib/nofiles/master.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import pandas
 from pympipool import Pool
-from pyiron_base import DataContainer, GenericJob
+from pyiron_base import DataContainer, GenericJob, state
 from pyiron_atomistics.project import Project
 from pyiron_atomistics.atomistics.structure.atoms import (
     Atoms,
     pyiron_to_ase,
     ase_to_pyiron,
 )
 from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob
 
 
 class GenericJobNoFiles(GenericJob):
     def __init__(self, project, job_name):
+        if not state.database.database_is_disabled:
+            raise RuntimeError(
+                "To run a `Without` job, the database must first be disabled. Please "
+                "`from pyiron_base import state; "
+                "state.update({'disable_database': True})`, and try again."
+            )
         super(GenericJobNoFiles, self).__init__(project, job_name)
 
         # internal variables
         self._python_only_job = True
-        self._interactive_disable_log_file = False
+        self._interactive_disable_log_file = True
 
     def refresh_job_status(self):
         if not self._interactive_disable_log_file:
             super(GenericJobNoFiles, self).refresh_job_status()
 
     def to_hdf(self, hdf=None, group_name=None):
         """
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/nofiles/murn.py` & `pyiron_contrib-0.1.9/pyiron_contrib/nofiles/murn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import pandas
 import numpy as np
-from pyiron_base import GenericMaster
+from pyiron_base import GenericMaster, state
 from pyiron_atomistics.atomistics.master.murnaghan import Murnaghan
 
 
 class MurnaghanWithoutFiles(Murnaghan):
     def __init__(self, project, job_name):
+        if not state.database.database_is_disabled:
+            raise RuntimeError(
+                "To run a `Without` job, the database must first be disabled. Please "
+                "`from pyiron_base import state; "
+                "state.update({'disable_database': True})`, and try again."
+            )
         super(MurnaghanWithoutFiles, self).__init__(project, job_name)
-        self._interactive_disable_log_file = False
+        self._interactive_disable_log_file = True
 
     @property
     def child_project(self):
         """
         :class:`.Project`: project which holds the created child jobs
         """
         if not self._interactive_disable_log_file:
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/nofiles/phonopy.py` & `pyiron_contrib-0.1.9/pyiron_contrib/nofiles/phonopy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-from pyiron_base import GenericMaster
+from pyiron_base import GenericMaster, state
 from pyiron_atomistics.atomistics.master.phonopy import PhonopyJob
 
 
 class PhonopyJobWithoutFiles(PhonopyJob):
     def __init__(self, project, job_name):
+        if not state.database.database_is_disabled:
+            raise RuntimeError(
+                "To run a `Without` job, the database must first be disabled. Please "
+                "`from pyiron_base import state; "
+                "state.update({'disable_database': True})`, and try again."
+            )
         super(PhonopyJobWithoutFiles, self).__init__(project, job_name)
-        self._interactive_disable_log_file = False
+        self._interactive_disable_log_file = True
 
     @property
     def child_project(self):
         """
         :class:`.Project`: project which holds the created child jobs
         """
         if not self._interactive_disable_log_file:
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/nofiles/sqs.py` & `pyiron_contrib-0.1.9/pyiron_contrib/nofiles/sqs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from pyiron_atomistics.atomistics.job.sqs import SQSJob, get_sqs_structures
+from pyiron_base import state
 
 
 class SQSJobWithoutOutput(SQSJob):
     def __init__(self, project, job_name):
+        if not state.database.database_is_disabled:
+            raise RuntimeError(
+                "To run a `Without` job, the database must first be disabled. Please "
+                "`from pyiron_base import state; "
+                "state.update({'disable_database': True})`, and try again."
+            )
         super(SQSJobWithoutOutput, self).__init__(project, job_name)
-        self._interactive_disable_log_file = False
+        self._interactive_disable_log_file = True
 
     def to_hdf(self, hdf=None, group_name=None):
         """
 
         Args:
             hdf:
             group_name:
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/finite_temperature_string.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/finite_temperature_string.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/minimize.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/minimize.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/molecular_dynamics.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/molecular_dynamics.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/nudged_elastic_band.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/nudged_elastic_band.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/qmmm.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/qmmm.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/compound/thermodynamic_integration.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/compound/thermodynamic_integration.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/generic.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/list.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/list.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/math.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/math.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/primitive/fts_vertices.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/primitive/fts_vertices.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/primitive/one_state.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/primitive/one_state.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/primitive/two_state.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/primitive/two_state.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/comparers.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/comparers.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/dictionaries.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/event.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/event.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/misc.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/pointer.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/pointer.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/pptree.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/pptree.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/protocol/utils/types.py` & `pyiron_contrib-0.1.9/pyiron_contrib/protocol/utils/types.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/workflow/channels.py` & `pyiron_contrib-0.1.9/pyiron_contrib/workflow/channels.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/workflow/io.py` & `pyiron_contrib-0.1.9/pyiron_contrib/workflow/io.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/workflow/node.py` & `pyiron_contrib-0.1.9/pyiron_contrib/workflow/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import inspect
+from functools import partialmethod
 from typing import get_args, get_type_hints, Optional, TYPE_CHECKING
 
 from pyiron_contrib.workflow.channels import InputChannel, OutputChannel
 from pyiron_contrib.workflow.has_to_dict import HasToDict
 from pyiron_contrib.workflow.io import Inputs, Outputs
 
 if TYPE_CHECKING:
@@ -75,15 +76,15 @@
         At the most basic level, to use nodes all we need to do is provide the `Node`
         class with a function and labels for its output, like so:
         >>> from pyiron_contrib.workflow.node import Node
         >>>
         >>> def mwe(x, y):
         ...     return x+1, y-1
         >>>
-        >>> plus_minus_1 = Node(node_function=mwe, output_labels=("p1", "m1"))
+        >>> plus_minus_1 = Node(mwe, "p1", "m1")
         >>>
         >>> print(plus_minus_1.outputs.p1)
         None
 
         There is no output because we haven't given our function any input, and it has
         no defaults!
         However, we'll run into a hiccup if we try to update one of the inputs...
@@ -104,15 +105,15 @@
 
         We can provide initial values for our node function at instantiation using our
         kwargs.
         The node update is deferred until _all_ of these initial values are processed.
         Thus, the second solution is to ensure that _all_ the arguments of our function
         are receiving good enough initial values to facilitate an execution of the node
         function at the end of instantiation:
-        >>> plus_minus_1 = Node(mwe, ("p1", "m1"), x=1, y=2)
+        >>> plus_minus_1 = Node(mwe, "p1", "m1", x=1, y=2)
         >>>
         >>> print(plus_minus_1.outputs.to_value_dict())
         {'p1': 2, 'm1': 1}
 
         Second, we could add type hints/defaults to our function so that it knows better
         than to try to evaluate itself with bad data.
         Let's make a new node following the second path.
@@ -126,15 +127,15 @@
         >>>
         >>> def hinted_example(
         ...     x: Union[int, float],
         ...     y: int | float = 1
         ... ) -> tuple[int, int | float]:
         ...     return x+1, y-1
         >>>
-        >>> plus_minus_1 = Node(hinted_example, ("p1", "m1"))
+        >>> plus_minus_1 = Node(hinted_example, "p1", "m1")
         >>>
         >>> plus_minus_1.inputs.x = 1
         >>> print(plus_minus_1.outputs.to_value_dict())
         {'p1': 2, 'm1': 0}
 
         In this case, we're able to use the default value for `y`, but you can
         experiment with updating `y` first (when `x` still has the invalid value of
@@ -160,16 +161,16 @@
         ...         input_storage_priority: Optional[dict[str, int]] = None,
         ...         output_storage_priority: Optional[dict[str, int]] = None,
         ...         run_automatically: bool = True,
         ...         update_on_instantiation: bool = False,
         ...         **kwargs
         ...     ):
         ...         super().__init__(
-        ...             node_function=self.alphabet_mod_three,
-        ...             output_labels="letter",
+        ...             self.alphabet_mod_three,
+        ...             "letter",
         ...             labe=label,
         ...             input_storage_priority=input_storage_priority,
         ...             output_storage_priority=output_storage_priority,
         ...             run_automatically=run_automatically,
         ...             update_on_instantiation=update_on_instantiation,
         ...             **kwargs
         ...         )
@@ -214,15 +215,15 @@
         "a"
 
         To see how to use many nodes together, look at the `Workflow` class.
     """
     def __init__(
             self,
             node_function: callable,
-            output_labels: tuple[str, ...] | str,
+            *output_labels: str,
             label: Optional[str] = None,
             input_storage_priority: Optional[dict[str, int]] = None,
             output_storage_priority: Optional[dict[str, int]] = None,
             run_automatically: bool = True,
             update_on_instantiation: bool = True,
             workflow: Optional[Workflow] = None,
             **kwargs
@@ -234,15 +235,15 @@
         if workflow is not None:
             workflow.add(self)
 
         input_channels = self._build_input_channels(input_storage_priority)
         self.inputs = Inputs(*input_channels)
 
         output_channels = self._build_output_channels(
-            output_labels, output_storage_priority
+            *output_labels, storage_priority=output_storage_priority
         )
         self.outputs = Outputs(*output_channels)
 
         self.run_automatically = False
         for k, v in kwargs.items():
             if k in self.inputs.labels:
                 if isinstance(v, OutputChannel):
@@ -280,52 +281,55 @@
                 node=self,
                 default=default,
                 type_hint=type_hint,
                 storage_priority=priority,
             ))
         return channels
 
-    def _build_output_channels(self, return_labels, storage_priority: dict[str:int]):
-        channels = []
+    def _build_output_channels(
+            self, *return_labels: str, storage_priority: dict[str:int] = None
+    ):
         try:
             type_hints = get_type_hints(self.node_function)["return"]
+            if len(return_labels) > 1:
+                type_hints = get_args(type_hints)
+                if not isinstance(type_hints, tuple):
+                    raise TypeError(
+                        f"With multiple return labels expected to get a tuple of type "
+                        f"hints, but got type {type(type_hints)}"
+                    )
+                if len(type_hints) != len(return_labels):
+                    raise ValueError(
+                        f"Expected type hints and return labels to have matching "
+                        f"lengths, but got {len(type_hints)} hints and "
+                        f"{len(return_labels)} labels: {type_hints}, {return_labels}"
+                    )
+            else:
+                # If there's only one hint, wrap it in a tuple so we can zip it with
+                # *return_labels and iterate over both at once
+                type_hints = (type_hints,)
         except KeyError:
-            type_hints = None
+            type_hints = [None] * len(return_labels)
 
-        if isinstance(return_labels, str):
+        channels = []
+        for label, hint in zip(return_labels, type_hints):
             try:
-                priority = storage_priority[return_labels]
+                priority = storage_priority[label]
             except (KeyError, TypeError):
                 priority = None
 
             channels.append(
                 OutputChannel(
-                    label=return_labels,
+                    label=label,
                     node=self,
-                    type_hint=type_hints,
+                    type_hint=hint,
                     storage_priority=priority,
                 )
             )
-        else:
-            hints = get_args(type_hints) if type_hints is not None else [None] * len(
-                return_labels)
-            for label, hint in zip(return_labels, hints):
-                try:
-                    priority = storage_priority[label]
-                except (KeyError, TypeError):
-                    priority = None
-
-                channels.append(
-                    OutputChannel(
-                        label=label,
-                        node=self,
-                        type_hint=hint,
-                        storage_priority=priority,
-                    )
-                )
+
         return channels
 
     def update(self) -> None:
         if self.run_automatically and self.ready:
             self.run()
 
     def run(self) -> None:
@@ -365,7 +369,28 @@
             "label": self.label,
             "ready": self.ready,
             "connected": self.connected,
             "fully_connected": self.fully_connected,
             "inputs": self.inputs.to_dict(),
             "outputs": self.outputs.to_dict(),
         }
+
+
+def node(*output_labels: str):
+    """
+    A decorator for dynamically creating node classes from functions.
+
+    Decorates a function.
+    Takes an output label for each returned value of the function.
+    Returns a `Node` subclass whose name is the camel-case version of the function node,
+    and whose signature is modified to exclude the node function and output labels
+    (which are explicitly defined in the process of using the decorator).
+    """
+
+    def as_node(node_function: callable):
+        return type(
+            node_function.__name__.title().replace("_", ""),  # fnc_name to CamelCase
+            (Node,),  # Define parentage
+            {'__init__': partialmethod(Node.__init__, node_function, *output_labels)}
+        )
+
+    return as_node
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/workflow/type_hinting.py` & `pyiron_contrib-0.1.9/pyiron_contrib/workflow/type_hinting.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 type hints relative to each other.
 """
 
 import types
 import typing
 from collections.abc import Callable
 
-from typeguard import check_type
+from typeguard import check_type, TypeCheckError
 
 
 def valid_value(value, type_hint) -> bool:
     try:
         return isinstance(value, type_hint)
     except TypeError:
         # Subscripted generics cannot be used with class and instance checks
         try:
             # typeguard handles this case
-            check_type("", value, type_hint)
+            check_type(value, type_hint)
             return True
-        except TypeError:
+        except TypeCheckError:
             # typeguard raises an error on a failed check
             return False
 
 
 def type_hint_to_tuple(type_hint) -> tuple:
     if isinstance(type_hint, (types.UnionType, typing._UnionGenericAlias)):
         return typing.get_args(type_hint)
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib/workflow/workflow.py` & `pyiron_contrib-0.1.9/pyiron_contrib/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib.egg-info/PKG-INFO` & `pyiron_contrib-0.1.9/pyiron_contrib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-contrib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_contrib
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyiron_contrib-0.1.8/pyiron_contrib.egg-info/SOURCES.txt` & `pyiron_contrib-0.1.9/pyiron_contrib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,18 @@
 pyiron_contrib/atomistics/randspg/__init__.py
 pyiron_contrib/atomistics/randspg/randspg.py
 pyiron_contrib/atomistics/runner/__init__.py
 pyiron_contrib/atomistics/runner/job.py
 pyiron_contrib/atomistics/runner/storageclasses.py
 pyiron_contrib/atomistics/runner/utils.py
 pyiron_contrib/generic/__init__.py
+pyiron_contrib/generic/coscineIo.py
+pyiron_contrib/generic/filedata.py
 pyiron_contrib/generic/s3io.py
+pyiron_contrib/generic/storage_interface_toolkit.py
 pyiron_contrib/image/__init__.py
 pyiron_contrib/image/custom_filters.py
 pyiron_contrib/image/image.py
 pyiron_contrib/image/job.py
 pyiron_contrib/image/utils.py
 pyiron_contrib/nofiles/__init__.py
 pyiron_contrib/nofiles/elastic.py
```

### Comparing `pyiron_contrib-0.1.8/setup.py` & `pyiron_contrib-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,35 +29,35 @@
     ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[        
         'matplotlib>=3.7.1',
         'numpy>=1.24.2',
-        'pyiron_base>=0.5.33',
+        'pyiron_base>=0.5.36',
         'scipy>=1.10.1',
         'seaborn>=0.12.2',
         'pyparsing>=3.0.9'
     ],
     extras_require={
         'atomistic': [
             'ase>=3.22.1',
-            'pyiron_atomistics>=0.2.64',
+            'pyiron_atomistics>=0.2.66',
             'pycp2k>=0.2.2',
         ],
         'fenics': [
             'fenics>=2019.1.0',
             'mshr>=2019.1.0',
         ],
-        'image': ['scikit-image>=0.19.3'],
+        'image': ['scikit-image>=0.20.0'],
         'generic': [
-            'boto3>=1.26.89', 
-            'moto>=4.1.5'
+            'boto3>=1.26.114', 
+            'moto>=4.1.7'
         ],
         'workflow': [
             'python>=3.10',
-            'typeguard>=2.13.3'
+            'typeguard>=3.0.2'
         ]
     },
     cmdclass=versioneer.get_cmdclass(),
     
 )
```

### Comparing `pyiron_contrib-0.1.8/versioneer.py` & `pyiron_contrib-0.1.9/versioneer.py`

 * *Files identical despite different names*

