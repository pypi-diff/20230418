# Comparing `tmp/atomman-1.4.8.tar.gz` & `tmp/atomman-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomman-1.4.8.tar", last modified: Fri Jan 27 19:35:16 2023, max compression
+gzip compressed data, was "atomman-1.4.9.tar", last modified: Tue Apr 18 20:26:29 2023, max compression
```

## Comparing `atomman-1.4.8.tar` & `atomman-1.4.9.tar`

### file list

```diff
@@ -1,239 +1,242 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.643073 atomman-1.4.8/
--rw-rw-rw-   0        0        0     2776 2019-07-10 17:30:09.000000 atomman-1.4.8/LICENSE.TXT
--rw-rw-rw-   0        0        0      205 2022-06-01 17:14:04.000000 atomman-1.4.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5054 2023-01-27 19:35:16.639073 atomman-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     4311 2021-08-10 14:38:34.000000 atomman-1.4.8/README.rst
--rw-rw-rw-   0        0        0    20892 2023-01-27 19:17:50.000000 atomman-1.4.8/UPDATES.rst
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:14.926065 atomman-1.4.8/atomman/
--rw-rw-rw-   0        0        0        5 2023-01-27 15:21:53.000000 atomman-1.4.8/atomman/VERSION
--rw-rw-rw-   0        0        0     1096 2022-11-03 19:12:57.000000 atomman-1.4.8/atomman/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.104064 atomman-1.4.8/atomman/cluster/
--rw-rw-rw-   0        0        0    31257 2022-06-01 13:44:35.000000 atomman-1.4.8/atomman/cluster/BondAngleMap.py
--rw-rw-rw-   0        0        0       68 2021-03-22 15:19:43.000000 atomman-1.4.8/atomman/cluster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.202079 atomman-1.4.8/atomman/core/
--rw-rw-rw-   0        0        0    22112 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/core/Atoms.py
--rw-rw-rw-   0        0        0    37743 2022-12-27 18:38:02.000000 atomman-1.4.8/atomman/core/Box.py
--rw-rw-rw-   0        0        0    40488 2023-01-09 17:56:29.000000 atomman-1.4.8/atomman/core/ElasticConstants.py
--rw-rw-rw-   0        0        0     5459 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/core/NeighborList.py
--rw-rw-rw-   0        0        0    48986 2022-10-11 21:10:57.000000 atomman-1.4.8/atomman/core/System.py
--rw-rw-rw-   0        0        0      427 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/core/__init__.py
--rw-rw-rw-   0        0        0     1650 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/core/displacement.py
--rw-rw-rw-   0        0        0   829102 2023-01-27 17:17:00.000000 atomman-1.4.8/atomman/core/dmag.c
--rw-rw-rw-   0        0        0      150 2019-07-10 17:30:09.000000 atomman-1.4.8/atomman/core/dmag.pxd
--rw-rw-rw-   0        0        0     4798 2019-10-21 17:17:03.000000 atomman-1.4.8/atomman/core/dmag.pyx
--rw-rw-rw-   0        0        0   832724 2023-01-27 17:17:00.000000 atomman-1.4.8/atomman/core/dvect.c
--rw-rw-rw-   0        0        0      150 2019-07-10 17:30:09.000000 atomman-1.4.8/atomman/core/dvect.pxd
--rw-rw-rw-   0        0        0     4939 2019-07-10 17:30:09.000000 atomman-1.4.8/atomman/core/dvect.pyx
--rw-rw-rw-   0        0        0  1029364 2023-01-27 17:17:01.000000 atomman-1.4.8/atomman/core/nlist.c
--rw-rw-rw-   0        0        0    13108 2019-10-21 17:19:29.000000 atomman-1.4.8/atomman/core/nlist.pyx
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.601069 atomman-1.4.8/atomman/defect/
--rw-rw-rw-   0        0        0    35597 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/DifferentialDisplacement.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.640067 atomman-1.4.8/atomman/defect/Dislocation/
--rw-rw-rw-   0        0        0    16151 2023-01-09 18:14:48.000000 atomman-1.4.8/atomman/defect/Dislocation/__init__.py
--rw-rw-rw-   0        0        0    12114 2023-01-03 19:16:43.000000 atomman-1.4.8/atomman/defect/Dislocation/_dipole.py
--rw-rw-rw-   0        0        0    13171 2022-12-16 15:52:56.000000 atomman-1.4.8/atomman/defect/Dislocation/_monopole.py
--rw-rw-rw-   0        0        0    18771 2022-12-19 15:44:51.000000 atomman-1.4.8/atomman/defect/Dislocation/_periodicarray.py
--rw-rw-rw-   0        0        0    17233 2022-06-01 13:44:35.000000 atomman-1.4.8/atomman/defect/FreeSurface.py
--rw-rw-rw-   0        0        0    55874 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/GammaSurface.py
--rw-rw-rw-   0        0        0    11293 2022-12-14 20:52:28.000000 atomman-1.4.8/atomman/defect/IsotropicVolterraDislocation.py
--rw-rw-rw-   0        0        0    49666 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/SDVPN.py
--rw-rw-rw-   0        0        0    22452 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/StackingFault.py
--rw-rw-rw-   0        0        0  1229759 2023-01-27 19:35:13.000000 atomman-1.4.8/atomman/defect/Strain.c
--rw-rw-rw-   0        0        0   210944 2023-01-27 17:32:48.000000 atomman-1.4.8/atomman/defect/Strain.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0   208896 2023-01-27 17:33:22.000000 atomman-1.4.8/atomman/defect/Strain.cp311-win_amd64.pyd
--rw-rw-rw-   0        0        0   245248 2023-01-27 17:17:18.000000 atomman-1.4.8/atomman/defect/Strain.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   246272 2023-01-27 19:33:00.000000 atomman-1.4.8/atomman/defect/Strain.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0   246784 2023-01-27 19:34:39.000000 atomman-1.4.8/atomman/defect/Strain.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0    23229 2023-01-26 21:37:47.000000 atomman-1.4.8/atomman/defect/Strain.pyx
--rw-rw-rw-   0        0        0    12083 2022-12-14 20:51:00.000000 atomman-1.4.8/atomman/defect/Stroh.py
--rw-rw-rw-   0        0        0    15484 2023-01-03 20:56:30.000000 atomman-1.4.8/atomman/defect/VolterraDislocation.py
--rw-rw-rw-   0        0        0     1643 2022-12-27 18:33:45.000000 atomman-1.4.8/atomman/defect/__init__.py
--rw-rw-rw-   0        0        0    15133 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/differential_displacement.py
--rw-rw-rw-   0        0        0    10116 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/dislocation_array.py
--rw-rw-rw-   0        0        0     5531 2022-11-22 20:19:35.000000 atomman-1.4.8/atomman/defect/dislocation_dipole_displacement.py
--rw-rw-rw-   0        0        0     8690 2022-12-08 13:35:46.000000 atomman-1.4.8/atomman/defect/dislocation_system_basis.py
--rw-rw-rw-   0        0        0     3146 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/dislocation_system_transform.py
--rw-rw-rw-   0        0        0     4612 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/disregistry.py
--rw-rw-rw-   0        0        0    10974 2022-12-08 13:35:40.000000 atomman-1.4.8/atomman/defect/free_surface_basis.py
--rw-rw-rw-   0        0        0     7070 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/nye_tensor.py
--rw-rw-rw-   0        0        0     1937 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/nye_tensor_p.py
--rw-rw-rw-   0        0        0     4457 2022-06-01 13:44:35.000000 atomman-1.4.8/atomman/defect/pn_arctan_disldensity.py
--rw-rw-rw-   0        0        0     4280 2022-06-01 13:44:35.000000 atomman-1.4.8/atomman/defect/pn_arctan_disregistry.py
--rw-rw-rw-   0        0        0    16811 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/defect/point.py
--rw-rw-rw-   0        0        0   821806 2023-01-27 17:17:02.000000 atomman-1.4.8/atomman/defect/slip_vector.c
--rw-rw-rw-   0        0        0   124416 2023-01-27 17:32:49.000000 atomman-1.4.8/atomman/defect/slip_vector.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0   123904 2023-01-27 17:33:23.000000 atomman-1.4.8/atomman/defect/slip_vector.cp311-win_amd64.pyd
--rw-rw-rw-   0        0        0   153600 2023-01-27 17:17:19.000000 atomman-1.4.8/atomman/defect/slip_vector.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0   152576 2023-01-27 17:31:40.000000 atomman-1.4.8/atomman/defect/slip_vector.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0   153088 2023-01-27 17:32:21.000000 atomman-1.4.8/atomman/defect/slip_vector.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0     3708 2019-10-21 19:44:39.000000 atomman-1.4.8/atomman/defect/slip_vector.pyx
--rw-rw-rw-   0        0        0     4377 2022-12-14 20:52:55.000000 atomman-1.4.8/atomman/defect/solve_volterra_dislocation.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.648067 atomman-1.4.8/atomman/dump/
--rw-rw-rw-   0        0        0     1627 2022-12-09 20:33:59.000000 atomman-1.4.8/atomman/dump/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.662068 atomman-1.4.8/atomman/dump/ase_Atoms/
--rw-rw-rw-   0        0        0       39 2019-10-21 19:46:16.000000 atomman-1.4.8/atomman/dump/ase_Atoms/__init__.py
--rw-rw-rw-   0        0        0     1987 2022-10-11 20:55:15.000000 atomman-1.4.8/atomman/dump/ase_Atoms/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.700067 atomman-1.4.8/atomman/dump/atom_data/
--rw-rw-rw-   0        0        0      141 2019-10-21 19:46:30.000000 atomman-1.4.8/atomman/dump/atom_data/__init__.py
--rw-rw-rw-   0        0        0    14738 2022-03-15 14:18:11.000000 atomman-1.4.8/atomman/dump/atom_data/atoms_prop_info.py
--rw-rw-rw-   0        0        0     9290 2022-07-13 15:17:50.000000 atomman-1.4.8/atomman/dump/atom_data/dump.py
--rw-rw-rw-   0        0        0     3289 2022-03-15 14:18:35.000000 atomman-1.4.8/atomman/dump/atom_data/velocities_prop_info.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.727069 atomman-1.4.8/atomman/dump/atom_dump/
--rw-rw-rw-   0        0        0       89 2019-10-21 19:49:17.000000 atomman-1.4.8/atomman/dump/atom_dump/__init__.py
--rw-rw-rw-   0        0        0    10902 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/dump/atom_dump/dump.py
--rw-rw-rw-   0        0        0     9697 2022-03-15 14:44:48.000000 atomman-1.4.8/atomman/dump/atom_dump/process_prop_info.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.747069 atomman-1.4.8/atomman/dump/conventional_to_primitive/
--rw-rw-rw-   0        0        0       39 2022-12-09 19:26:10.000000 atomman-1.4.8/atomman/dump/conventional_to_primitive/__init__.py
--rw-rw-rw-   0        0        0    11506 2022-12-09 20:45:01.000000 atomman-1.4.8/atomman/dump/conventional_to_primitive/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.763104 atomman-1.4.8/atomman/dump/lammps_commands/
--rw-rw-rw-   0        0        0       22 2020-10-29 19:01:14.000000 atomman-1.4.8/atomman/dump/lammps_commands/__init__.py
--rw-rw-rw-   0        0        0     8107 2022-07-11 18:28:20.000000 atomman-1.4.8/atomman/dump/lammps_commands/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.778068 atomman-1.4.8/atomman/dump/phonopy_Atoms/
--rw-rw-rw-   0        0        0       39 2019-10-21 19:50:07.000000 atomman-1.4.8/atomman/dump/phonopy_Atoms/__init__.py
--rw-rw-rw-   0        0        0     2175 2022-10-11 20:55:16.000000 atomman-1.4.8/atomman/dump/phonopy_Atoms/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.793068 atomman-1.4.8/atomman/dump/poscar/
--rw-rw-rw-   0        0        0       39 2019-10-21 19:50:20.000000 atomman-1.4.8/atomman/dump/poscar/__init__.py
--rw-rw-rw-   0        0        0     3807 2022-03-15 14:56:04.000000 atomman-1.4.8/atomman/dump/poscar/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.808104 atomman-1.4.8/atomman/dump/primitive_cell/
--rw-rw-rw-   0        0        0       22 2022-06-01 13:44:35.000000 atomman-1.4.8/atomman/dump/primitive_cell/__init__.py
--rw-rw-rw-   0        0        0     1692 2022-10-11 20:54:59.000000 atomman-1.4.8/atomman/dump/primitive_cell/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.822069 atomman-1.4.8/atomman/dump/primitive_to_conventional/
--rw-rw-rw-   0        0        0       39 2022-12-09 19:26:15.000000 atomman-1.4.8/atomman/dump/primitive_to_conventional/__init__.py
--rw-rw-rw-   0        0        0     2308 2022-12-09 20:40:08.000000 atomman-1.4.8/atomman/dump/primitive_to_conventional/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.837104 atomman-1.4.8/atomman/dump/pymatgen_Structure/
--rw-rw-rw-   0        0        0       39 2019-10-21 19:50:45.000000 atomman-1.4.8/atomman/dump/pymatgen_Structure/__init__.py
--rw-rw-rw-   0        0        0     1705 2022-10-11 20:55:31.000000 atomman-1.4.8/atomman/dump/pymatgen_Structure/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.851071 atomman-1.4.8/atomman/dump/spglib_cell/
--rw-rw-rw-   0        0        0       39 2019-10-21 19:51:00.000000 atomman-1.4.8/atomman/dump/spglib_cell/__init__.py
--rw-rw-rw-   0        0        0      683 2022-03-15 15:05:03.000000 atomman-1.4.8/atomman/dump/spglib_cell/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.866094 atomman-1.4.8/atomman/dump/system_model/
--rw-rw-rw-   0        0        0       39 2019-10-21 19:51:10.000000 atomman-1.4.8/atomman/dump/system_model/__init__.py
--rw-rw-rw-   0        0        0     3836 2022-03-15 15:14:26.000000 atomman-1.4.8/atomman/dump/system_model/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.893102 atomman-1.4.8/atomman/dump/table/
--rw-rw-rw-   0        0        0       89 2019-10-21 19:52:52.000000 atomman-1.4.8/atomman/dump/table/__init__.py
--rw-rw-rw-   0        0        0     5852 2022-10-11 21:05:43.000000 atomman-1.4.8/atomman/dump/table/dump.py
--rw-rw-rw-   0        0        0     5355 2022-03-15 15:23:56.000000 atomman-1.4.8/atomman/dump/table/process_prop_info.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.965069 atomman-1.4.8/atomman/lammps/
--rw-rw-rw-   0        0        0    13503 2022-10-04 19:31:09.000000 atomman-1.4.8/atomman/lammps/Log.py
--rw-rw-rw-   0        0        0     6766 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/lammps/NEBLog.py
--rw-rw-rw-   0        0        0     3143 2022-06-01 13:44:35.000000 atomman-1.4.8/atomman/lammps/Potential.py
--rw-rw-rw-   0        0        0      703 2020-07-28 21:06:14.000000 atomman-1.4.8/atomman/lammps/__init__.py
--rw-rw-rw-   0        0        0     1020 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/lammps/checkversion.py
--rw-rw-rw-   0        0        0     2647 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/lammps/normalize.py
--rw-rw-rw-   0        0        0     5497 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/lammps/run.py
--rw-rw-rw-   0        0        0     7239 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/lammps/style.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:15.981070 atomman-1.4.8/atomman/library/
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.024120 atomman-1.4.8/atomman/library/Database/
--rw-rw-rw-   0        0        0     2750 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/library/Database/__init__.py
--rw-rw-rw-   0        0        0    17695 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/library/Database/_crystal_prototype.py
--rw-rw-rw-   0        0        0    26267 2022-10-11 21:02:27.000000 atomman-1.4.8/atomman/library/Database/_reference_crystal.py
--rw-rw-rw-   0        0        0    20741 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/library/Database/_relaxed_crystal.py
--rw-rw-rw-   0        0        0      251 2021-08-03 11:18:29.000000 atomman-1.4.8/atomman/library/__init__.py
--rw-rw-rw-   0        0        0     6638 2022-06-01 13:44:35.000000 atomman-1.4.8/atomman/library/load_lammps_potential.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.112069 atomman-1.4.8/atomman/library/record/
--rw-rw-rw-   0        0        0    16648 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/library/record/CrystalPrototype.py
--rw-rw-rw-   0        0        0    11791 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/library/record/Dislocation.py
--rw-rw-rw-   0        0        0    10373 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/library/record/FreeSurface.py
--rw-rw-rw-   0        0        0     9427 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/library/record/PointDefect.py
--rw-rw-rw-   0        0        0    19661 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/library/record/ReferenceCrystal.py
--rw-rw-rw-   0        0        0    24577 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/library/record/RelaxedCrystal.py
--rw-rw-rw-   0        0        0    10169 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/library/record/StackingFault.py
--rw-rw-rw-   0        0        0      711 2022-03-03 22:56:52.000000 atomman-1.4.8/atomman/library/record/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.118073 atomman-1.4.8/atomman/library/xsd/
--rw-rw-rw-   0        0        0        0 2021-08-03 11:18:29.000000 atomman-1.4.8/atomman/library/xsd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.126072 atomman-1.4.8/atomman/library/xsl/
--rw-rw-rw-   0        0        0        0 2021-08-03 11:18:29.000000 atomman-1.4.8/atomman/library/xsl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.132070 atomman-1.4.8/atomman/load/
--rw-rw-rw-   0        0        0     1726 2022-10-11 20:58:20.000000 atomman-1.4.8/atomman/load/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.144069 atomman-1.4.8/atomman/load/ase_Atoms/
--rw-rw-rw-   0        0        0       39 2019-10-21 20:07:58.000000 atomman-1.4.8/atomman/load/ase_Atoms/__init__.py
--rw-rw-rw-   0        0        0     1585 2022-10-11 20:58:19.000000 atomman-1.4.8/atomman/load/ase_Atoms/load.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.183072 atomman-1.4.8/atomman/load/atom_data/
--rw-rw-rw-   0        0        0      141 2019-10-21 20:07:40.000000 atomman-1.4.8/atomman/load/atom_data/__init__.py
--rw-rw-rw-   0        0        0    14733 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/atom_data/atoms_prop_info.py
--rw-rw-rw-   0        0        0    13973 2022-10-11 20:58:18.000000 atomman-1.4.8/atomman/load/atom_data/load.py
--rw-rw-rw-   0        0        0     3284 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/atom_data/velocities_prop_info.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.209074 atomman-1.4.8/atomman/load/atom_dump/
--rw-rw-rw-   0        0        0       89 2019-10-21 20:16:44.000000 atomman-1.4.8/atomman/load/atom_dump/__init__.py
--rw-rw-rw-   0        0        0    10365 2022-10-11 20:58:17.000000 atomman-1.4.8/atomman/load/atom_dump/load.py
--rw-rw-rw-   0        0        0     9630 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/atom_dump/process_prop_info.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.226072 atomman-1.4.8/atomman/load/cif/
--rw-rw-rw-   0        0        0       39 2019-10-21 20:03:55.000000 atomman-1.4.8/atomman/load/cif/__init__.py
--rw-rw-rw-   0        0        0     1956 2022-10-11 20:58:16.000000 atomman-1.4.8/atomman/load/cif/load.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.245070 atomman-1.4.8/atomman/load/crystal/
--rw-rw-rw-   0        0        0       22 2020-07-23 19:09:45.000000 atomman-1.4.8/atomman/load/crystal/__init__.py
--rw-rw-rw-   0        0        0     6396 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/crystal/load.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.261071 atomman-1.4.8/atomman/load/dft_reference/
--rw-rw-rw-   0        0        0       22 2021-08-04 15:10:28.000000 atomman-1.4.8/atomman/load/dft_reference/__init__.py
--rw-rw-rw-   0        0        0     2983 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/dft_reference/load.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.281072 atomman-1.4.8/atomman/load/phonopy_Atoms/
--rw-rw-rw-   0        0        0       39 2019-10-21 20:03:35.000000 atomman-1.4.8/atomman/load/phonopy_Atoms/__init__.py
--rw-rw-rw-   0        0        0     1699 2022-10-11 20:58:15.000000 atomman-1.4.8/atomman/load/phonopy_Atoms/load.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.295107 atomman-1.4.8/atomman/load/poscar/
--rw-rw-rw-   0        0        0       39 2019-10-21 20:03:19.000000 atomman-1.4.8/atomman/load/poscar/__init__.py
--rw-rw-rw-   0        0        0     3124 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/poscar/load.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.309070 atomman-1.4.8/atomman/load/prototype/
--rw-rw-rw-   0        0        0       22 2020-07-23 19:09:45.000000 atomman-1.4.8/atomman/load/prototype/__init__.py
--rw-rw-rw-   0        0        0     9720 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/prototype/load.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.326071 atomman-1.4.8/atomman/load/pymatgen_Structure/
--rw-rw-rw-   0        0        0       39 2019-10-21 20:02:57.000000 atomman-1.4.8/atomman/load/pymatgen_Structure/__init__.py
--rw-rw-rw-   0        0        0     1590 2022-10-11 20:58:14.000000 atomman-1.4.8/atomman/load/pymatgen_Structure/load.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.341071 atomman-1.4.8/atomman/load/spglib_cell/
--rw-rw-rw-   0        0        0       39 2019-10-21 20:02:34.000000 atomman-1.4.8/atomman/load/spglib_cell/__init__.py
--rw-rw-rw-   0        0        0     1030 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/spglib_cell/load.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.356072 atomman-1.4.8/atomman/load/system_model/
--rw-rw-rw-   0        0        0       39 2019-10-21 20:02:23.000000 atomman-1.4.8/atomman/load/system_model/__init__.py
--rw-rw-rw-   0        0        0     6303 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/system_model/load.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.380072 atomman-1.4.8/atomman/load/table/
--rw-rw-rw-   0        0        0       89 2019-10-21 20:01:33.000000 atomman-1.4.8/atomman/load/table/__init__.py
--rw-rw-rw-   0        0        0     5246 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/table/load.py
--rw-rw-rw-   0        0        0     5527 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/load/table/process_prop_info.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.413078 atomman-1.4.8/atomman/mep/
--rw-rw-rw-   0        0        0    12671 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/mep/BasePath.py
--rw-rw-rw-   0        0        0    10414 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/mep/ISMPath.py
--rw-rw-rw-   0        0        0     2165 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/mep/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.428088 atomman-1.4.8/atomman/mep/gradient/
--rw-rw-rw-   0        0        0      103 2021-02-22 17:04:15.000000 atomman-1.4.8/atomman/mep/gradient/__init__.py
--rw-rw-rw-   0        0        0     1714 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/mep/gradient/central_difference.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.450070 atomman-1.4.8/atomman/mep/integrator/
--rw-rw-rw-   0        0        0      114 2021-02-22 17:04:37.000000 atomman-1.4.8/atomman/mep/integrator/__init__.py
--rw-rw-rw-   0        0        0      892 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/mep/integrator/euler.py
--rw-rw-rw-   0        0        0     1133 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/mep/integrator/rungekutta.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.466070 atomman-1.4.8/atomman/plot/
--rw-rw-rw-   0        0        0      106 2019-10-21 18:43:36.000000 atomman-1.4.8/atomman/plot/__init__.py
--rw-rw-rw-   0        0        0    18778 2023-01-26 22:32:59.000000 atomman-1.4.8/atomman/plot/interpolate_contour.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.516074 atomman-1.4.8/atomman/region/
--rw-rw-rw-   0        0        0     4210 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/region/Cylinder.py
--rw-rw-rw-   0        0        0     5557 2022-06-01 13:44:35.000000 atomman-1.4.8/atomman/region/Plane.py
--rw-rw-rw-   0        0        0     2196 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/region/PlaneSet.py
--rw-rw-rw-   0        0        0     1740 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/region/Shape.py
--rw-rw-rw-   0        0        0     2301 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/region/Sphere.py
--rw-rw-rw-   0        0        0      229 2020-08-24 20:38:08.000000 atomman-1.4.8/atomman/region/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.557077 atomman-1.4.8/atomman/thermo/
--rw-rw-rw-   0        0        0     3809 2022-11-03 19:11:23.000000 atomman-1.4.8/atomman/thermo/EinsteinSolid.py
--rw-rw-rw-   0        0        0     2105 2022-11-03 19:09:25.000000 atomman-1.4.8/atomman/thermo/IdealGas.py
--rw-rw-rw-   0        0        0     3159 2022-11-03 19:12:56.000000 atomman-1.4.8/atomman/thermo/RDF.py
--rw-rw-rw-   0        0        0    76536 2022-11-03 19:12:50.000000 atomman-1.4.8/atomman/thermo/UhlenbeckFordModel.py
--rw-rw-rw-   0        0        0      146 2022-11-03 19:13:01.000000 atomman-1.4.8/atomman/thermo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:16.634078 atomman-1.4.8/atomman/tools/
--rw-rw-rw-   0        0        0      937 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/tools/__init__.py
--rw-rw-rw-   0        0        0     1278 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/tools/axes_check.py
--rw-rw-rw-   0        0        0      955 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/tools/boolean.py
--rw-rw-rw-   0        0        0     1075 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/tools/compositionstr.py
--rw-rw-rw-   0        0        0     9197 2022-03-25 15:50:03.000000 atomman-1.4.8/atomman/tools/crystalsystem.py
--rw-rw-rw-   0        0        0     6290 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/tools/duplicates_allclose.py
--rw-rw-rw-   0        0        0     2627 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/tools/filltemplate.py
--rw-rw-rw-   0        0        0     1158 2022-03-15 16:07:49.000000 atomman-1.4.8/atomman/tools/indexstr.py
--rw-rw-rw-   0        0        0    15048 2022-12-09 16:03:02.000000 atomman-1.4.8/atomman/tools/miller.py
--rw-rw-rw-   0        0        0     1552 2022-12-15 20:45:30.000000 atomman-1.4.8/atomman/tools/vect_angle.py
--rw-rw-rw-   0        0        0    12639 2022-03-15 16:07:50.000000 atomman-1.4.8/atomman/unitconvert.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:35:14.965064 atomman-1.4.8/atomman.egg-info/
--rw-rw-rw-   0        0        0     5054 2023-01-27 19:35:14.000000 atomman-1.4.8/atomman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6311 2023-01-27 19:35:14.000000 atomman-1.4.8/atomman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 19:35:14.000000 atomman-1.4.8/atomman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-07-10 18:43:04.000000 atomman-1.4.8/atomman.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      115 2023-01-27 19:35:14.000000 atomman-1.4.8/atomman.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-27 19:35:14.000000 atomman-1.4.8/atomman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      154 2022-04-01 16:42:36.000000 atomman-1.4.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-27 19:35:16.643073 atomman-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0     2075 2023-01-27 17:30:15.000000 atomman-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:29.020681 atomman-1.4.9/
+-rw-rw-rw-   0        0        0     2776 2019-07-10 17:30:09.000000 atomman-1.4.9/LICENSE.TXT
+-rw-rw-rw-   0        0        0      205 2022-06-01 17:14:04.000000 atomman-1.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5054 2023-04-18 20:26:29.020681 atomman-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4311 2021-08-10 14:38:34.000000 atomman-1.4.9/README.rst
+-rw-rw-rw-   0        0        0    21069 2023-04-06 14:41:33.000000 atomman-1.4.9/UPDATES.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.748666 atomman-1.4.9/atomman/
+-rw-rw-rw-   0        0        0        5 2023-04-06 14:26:55.000000 atomman-1.4.9/atomman/VERSION
+-rw-rw-rw-   0        0        0     1096 2022-11-03 19:12:57.000000 atomman-1.4.9/atomman/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.776667 atomman-1.4.9/atomman/cluster/
+-rw-rw-rw-   0        0        0    31257 2022-06-01 13:44:35.000000 atomman-1.4.9/atomman/cluster/BondAngleMap.py
+-rw-rw-rw-   0        0        0       68 2021-03-22 15:19:43.000000 atomman-1.4.9/atomman/cluster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.794680 atomman-1.4.9/atomman/core/
+-rw-rw-rw-   0        0        0    22112 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/core/Atoms.py
+-rw-rw-rw-   0        0        0    37743 2022-12-27 18:38:02.000000 atomman-1.4.9/atomman/core/Box.py
+-rw-rw-rw-   0        0        0    40488 2023-01-09 17:56:29.000000 atomman-1.4.9/atomman/core/ElasticConstants.py
+-rw-rw-rw-   0        0        0     5459 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/core/NeighborList.py
+-rw-rw-rw-   0        0        0    48986 2022-10-11 21:10:57.000000 atomman-1.4.9/atomman/core/System.py
+-rw-rw-rw-   0        0        0      427 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/core/__init__.py
+-rw-rw-rw-   0        0        0     1650 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/core/displacement.py
+-rw-rw-rw-   0        0        0   829102 2023-01-27 17:17:00.000000 atomman-1.4.9/atomman/core/dmag.c
+-rw-rw-rw-   0        0        0      150 2019-07-10 17:30:09.000000 atomman-1.4.9/atomman/core/dmag.pxd
+-rw-rw-rw-   0        0        0     4798 2019-10-21 17:17:03.000000 atomman-1.4.9/atomman/core/dmag.pyx
+-rw-rw-rw-   0        0        0   832724 2023-01-27 17:17:00.000000 atomman-1.4.9/atomman/core/dvect.c
+-rw-rw-rw-   0        0        0      150 2019-07-10 17:30:09.000000 atomman-1.4.9/atomman/core/dvect.pxd
+-rw-rw-rw-   0        0        0     4939 2019-07-10 17:30:09.000000 atomman-1.4.9/atomman/core/dvect.pyx
+-rw-rw-rw-   0        0        0  1029364 2023-01-27 17:17:01.000000 atomman-1.4.9/atomman/core/nlist.c
+-rw-rw-rw-   0        0        0    13108 2019-10-21 17:19:29.000000 atomman-1.4.9/atomman/core/nlist.pyx
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.859679 atomman-1.4.9/atomman/defect/
+-rw-rw-rw-   0        0        0    35597 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/DifferentialDisplacement.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.864642 atomman-1.4.9/atomman/defect/Dislocation/
+-rw-rw-rw-   0        0        0    16151 2023-01-09 18:14:48.000000 atomman-1.4.9/atomman/defect/Dislocation/__init__.py
+-rw-rw-rw-   0        0        0    12114 2023-01-03 19:16:43.000000 atomman-1.4.9/atomman/defect/Dislocation/_dipole.py
+-rw-rw-rw-   0        0        0    13171 2022-12-16 15:52:56.000000 atomman-1.4.9/atomman/defect/Dislocation/_monopole.py
+-rw-rw-rw-   0        0        0    18771 2022-12-19 15:44:51.000000 atomman-1.4.9/atomman/defect/Dislocation/_periodicarray.py
+-rw-rw-rw-   0        0        0    17233 2022-06-01 13:44:35.000000 atomman-1.4.9/atomman/defect/FreeSurface.py
+-rw-rw-rw-   0        0        0    55874 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/GammaSurface.py
+-rw-rw-rw-   0        0        0    11293 2022-12-14 20:52:28.000000 atomman-1.4.9/atomman/defect/IsotropicVolterraDislocation.py
+-rw-rw-rw-   0        0        0    49666 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/SDVPN.py
+-rw-rw-rw-   0        0        0    22452 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/StackingFault.py
+-rw-rw-rw-   0        0        0  1229822 2023-04-18 20:26:27.000000 atomman-1.4.9/atomman/defect/Strain.c
+-rw-rw-rw-   0        0        0   213504 2023-04-18 20:24:59.000000 atomman-1.4.9/atomman/defect/Strain.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0   210944 2023-04-18 20:26:06.000000 atomman-1.4.9/atomman/defect/Strain.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0   247296 2023-04-18 20:21:40.000000 atomman-1.4.9/atomman/defect/Strain.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   246272 2023-04-18 20:22:42.000000 atomman-1.4.9/atomman/defect/Strain.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0   246784 2023-04-18 20:23:49.000000 atomman-1.4.9/atomman/defect/Strain.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0    23229 2023-01-26 21:37:47.000000 atomman-1.4.9/atomman/defect/Strain.pyx
+-rw-rw-rw-   0        0        0    12083 2022-12-14 20:51:00.000000 atomman-1.4.9/atomman/defect/Stroh.py
+-rw-rw-rw-   0        0        0    15484 2023-01-03 20:56:30.000000 atomman-1.4.9/atomman/defect/VolterraDislocation.py
+-rw-rw-rw-   0        0        0     1643 2022-12-27 18:33:45.000000 atomman-1.4.9/atomman/defect/__init__.py
+-rw-rw-rw-   0        0        0    15133 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/differential_displacement.py
+-rw-rw-rw-   0        0        0    10116 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/dislocation_array.py
+-rw-rw-rw-   0        0        0     5531 2022-11-22 20:19:35.000000 atomman-1.4.9/atomman/defect/dislocation_dipole_displacement.py
+-rw-rw-rw-   0        0        0     8690 2022-12-08 13:35:46.000000 atomman-1.4.9/atomman/defect/dislocation_system_basis.py
+-rw-rw-rw-   0        0        0     3146 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/dislocation_system_transform.py
+-rw-rw-rw-   0        0        0     4612 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/disregistry.py
+-rw-rw-rw-   0        0        0    10974 2022-12-08 13:35:40.000000 atomman-1.4.9/atomman/defect/free_surface_basis.py
+-rw-rw-rw-   0        0        0     7070 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/nye_tensor.py
+-rw-rw-rw-   0        0        0     1937 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/nye_tensor_p.py
+-rw-rw-rw-   0        0        0     4457 2022-06-01 13:44:35.000000 atomman-1.4.9/atomman/defect/pn_arctan_disldensity.py
+-rw-rw-rw-   0        0        0     4280 2022-06-01 13:44:35.000000 atomman-1.4.9/atomman/defect/pn_arctan_disregistry.py
+-rw-rw-rw-   0        0        0    16811 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/defect/point.py
+-rw-rw-rw-   0        0        0   821806 2023-01-27 17:17:02.000000 atomman-1.4.9/atomman/defect/slip_vector.c
+-rw-rw-rw-   0        0        0   124416 2023-01-27 17:32:49.000000 atomman-1.4.9/atomman/defect/slip_vector.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0   123904 2023-01-27 17:33:23.000000 atomman-1.4.9/atomman/defect/slip_vector.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0   153600 2023-01-27 17:17:19.000000 atomman-1.4.9/atomman/defect/slip_vector.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0   152576 2023-01-27 17:31:40.000000 atomman-1.4.9/atomman/defect/slip_vector.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0   153088 2023-01-27 17:32:21.000000 atomman-1.4.9/atomman/defect/slip_vector.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0     3708 2019-10-21 19:44:39.000000 atomman-1.4.9/atomman/defect/slip_vector.pyx
+-rw-rw-rw-   0        0        0     4377 2022-12-14 20:52:55.000000 atomman-1.4.9/atomman/defect/solve_volterra_dislocation.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.866640 atomman-1.4.9/atomman/dump/
+-rw-rw-rw-   0        0        0     1627 2022-12-09 20:33:59.000000 atomman-1.4.9/atomman/dump/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.868641 atomman-1.4.9/atomman/dump/ase_Atoms/
+-rw-rw-rw-   0        0        0       39 2019-10-21 19:46:16.000000 atomman-1.4.9/atomman/dump/ase_Atoms/__init__.py
+-rw-rw-rw-   0        0        0     1987 2022-10-11 20:55:15.000000 atomman-1.4.9/atomman/dump/ase_Atoms/dump.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.873666 atomman-1.4.9/atomman/dump/atom_data/
+-rw-rw-rw-   0        0        0      141 2019-10-21 19:46:30.000000 atomman-1.4.9/atomman/dump/atom_data/__init__.py
+-rw-rw-rw-   0        0        0    14738 2022-03-15 14:18:11.000000 atomman-1.4.9/atomman/dump/atom_data/atoms_prop_info.py
+-rw-rw-rw-   0        0        0     9290 2022-07-13 15:17:50.000000 atomman-1.4.9/atomman/dump/atom_data/dump.py
+-rw-rw-rw-   0        0        0     3289 2022-03-15 14:18:35.000000 atomman-1.4.9/atomman/dump/atom_data/velocities_prop_info.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.876681 atomman-1.4.9/atomman/dump/atom_dump/
+-rw-rw-rw-   0        0        0       89 2019-10-21 19:49:17.000000 atomman-1.4.9/atomman/dump/atom_dump/__init__.py
+-rw-rw-rw-   0        0        0    10902 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/dump/atom_dump/dump.py
+-rw-rw-rw-   0        0        0     9697 2022-03-15 14:44:48.000000 atomman-1.4.9/atomman/dump/atom_dump/process_prop_info.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.879678 atomman-1.4.9/atomman/dump/conventional_to_primitive/
+-rw-rw-rw-   0        0        0       39 2022-12-09 19:26:10.000000 atomman-1.4.9/atomman/dump/conventional_to_primitive/__init__.py
+-rw-rw-rw-   0        0        0    11506 2022-12-09 20:45:01.000000 atomman-1.4.9/atomman/dump/conventional_to_primitive/dump.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.881642 atomman-1.4.9/atomman/dump/lammps_commands/
+-rw-rw-rw-   0        0        0       22 2020-10-29 19:01:14.000000 atomman-1.4.9/atomman/dump/lammps_commands/__init__.py
+-rw-rw-rw-   0        0        0     8107 2022-07-11 18:28:20.000000 atomman-1.4.9/atomman/dump/lammps_commands/dump.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.884677 atomman-1.4.9/atomman/dump/phonopy_Atoms/
+-rw-rw-rw-   0        0        0       39 2019-10-21 19:50:07.000000 atomman-1.4.9/atomman/dump/phonopy_Atoms/__init__.py
+-rw-rw-rw-   0        0        0     2175 2022-10-11 20:55:16.000000 atomman-1.4.9/atomman/dump/phonopy_Atoms/dump.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.886679 atomman-1.4.9/atomman/dump/poscar/
+-rw-rw-rw-   0        0        0       39 2019-10-21 19:50:20.000000 atomman-1.4.9/atomman/dump/poscar/__init__.py
+-rw-rw-rw-   0        0        0     3807 2022-03-15 14:56:04.000000 atomman-1.4.9/atomman/dump/poscar/dump.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.888677 atomman-1.4.9/atomman/dump/primitive_cell/
+-rw-rw-rw-   0        0        0       22 2022-06-01 13:44:35.000000 atomman-1.4.9/atomman/dump/primitive_cell/__init__.py
+-rw-rw-rw-   0        0        0     1692 2022-10-11 20:54:59.000000 atomman-1.4.9/atomman/dump/primitive_cell/dump.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.890681 atomman-1.4.9/atomman/dump/primitive_to_conventional/
+-rw-rw-rw-   0        0        0       39 2022-12-09 19:26:15.000000 atomman-1.4.9/atomman/dump/primitive_to_conventional/__init__.py
+-rw-rw-rw-   0        0        0     2308 2022-12-09 20:40:08.000000 atomman-1.4.9/atomman/dump/primitive_to_conventional/dump.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.893689 atomman-1.4.9/atomman/dump/pymatgen_Structure/
+-rw-rw-rw-   0        0        0       39 2019-10-21 19:50:45.000000 atomman-1.4.9/atomman/dump/pymatgen_Structure/__init__.py
+-rw-rw-rw-   0        0        0     1705 2022-10-11 20:55:31.000000 atomman-1.4.9/atomman/dump/pymatgen_Structure/dump.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.895677 atomman-1.4.9/atomman/dump/spglib_cell/
+-rw-rw-rw-   0        0        0       39 2019-10-21 19:51:00.000000 atomman-1.4.9/atomman/dump/spglib_cell/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-03-15 15:05:03.000000 atomman-1.4.9/atomman/dump/spglib_cell/dump.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.897678 atomman-1.4.9/atomman/dump/system_model/
+-rw-rw-rw-   0        0        0       39 2019-10-21 19:51:10.000000 atomman-1.4.9/atomman/dump/system_model/__init__.py
+-rw-rw-rw-   0        0        0     3836 2022-03-15 15:14:26.000000 atomman-1.4.9/atomman/dump/system_model/dump.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.901678 atomman-1.4.9/atomman/dump/table/
+-rw-rw-rw-   0        0        0       89 2019-10-21 19:52:52.000000 atomman-1.4.9/atomman/dump/table/__init__.py
+-rw-rw-rw-   0        0        0     5852 2022-10-11 21:05:43.000000 atomman-1.4.9/atomman/dump/table/dump.py
+-rw-rw-rw-   0        0        0     5355 2022-03-15 15:23:56.000000 atomman-1.4.9/atomman/dump/table/process_prop_info.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.910679 atomman-1.4.9/atomman/lammps/
+-rw-rw-rw-   0        0        0    13503 2022-10-04 19:31:09.000000 atomman-1.4.9/atomman/lammps/Log.py
+-rw-rw-rw-   0        0        0     6766 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/lammps/NEBLog.py
+-rw-rw-rw-   0        0        0     3143 2022-06-01 13:44:35.000000 atomman-1.4.9/atomman/lammps/Potential.py
+-rw-rw-rw-   0        0        0      703 2020-07-28 21:06:14.000000 atomman-1.4.9/atomman/lammps/__init__.py
+-rw-rw-rw-   0        0        0     1020 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/lammps/checkversion.py
+-rw-rw-rw-   0        0        0     2647 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/lammps/normalize.py
+-rw-rw-rw-   0        0        0     5497 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/lammps/run.py
+-rw-rw-rw-   0        0        0     7239 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/lammps/style.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.913643 atomman-1.4.9/atomman/library/
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.918642 atomman-1.4.9/atomman/library/Database/
+-rw-rw-rw-   0        0        0     2750 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/library/Database/__init__.py
+-rw-rw-rw-   0        0        0    17695 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/library/Database/_crystal_prototype.py
+-rw-rw-rw-   0        0        0    26265 2023-04-05 20:40:48.000000 atomman-1.4.9/atomman/library/Database/_reference_crystal.py
+-rw-rw-rw-   0        0        0    20741 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/library/Database/_relaxed_crystal.py
+-rw-rw-rw-   0        0        0      251 2021-08-03 11:18:29.000000 atomman-1.4.9/atomman/library/__init__.py
+-rw-rw-rw-   0        0        0     6638 2022-06-01 13:44:35.000000 atomman-1.4.9/atomman/library/load_lammps_potential.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.928643 atomman-1.4.9/atomman/library/record/
+-rw-rw-rw-   0        0        0    10137 2023-04-05 16:42:12.000000 atomman-1.4.9/atomman/library/record/CrystalPrototype.py
+-rw-rw-rw-   0        0        0     8913 2023-04-05 16:42:11.000000 atomman-1.4.9/atomman/library/record/Dislocation.py
+-rw-rw-rw-   0        0        0     6703 2023-04-05 16:42:09.000000 atomman-1.4.9/atomman/library/record/FreeSurface.py
+-rw-rw-rw-   0        0        0     6531 2023-04-05 16:42:08.000000 atomman-1.4.9/atomman/library/record/PointDefect.py
+-rw-rw-rw-   0        0        0    15181 2023-04-05 16:55:07.000000 atomman-1.4.9/atomman/library/record/ReferenceCrystal.py
+-rw-rw-rw-   0        0        0    15248 2023-04-05 16:54:38.000000 atomman-1.4.9/atomman/library/record/RelaxedCrystal.py
+-rw-rw-rw-   0        0        0     6885 2023-04-05 16:43:30.000000 atomman-1.4.9/atomman/library/record/StackingFault.py
+-rw-rw-rw-   0        0        0      711 2022-03-03 22:56:52.000000 atomman-1.4.9/atomman/library/record/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.929642 atomman-1.4.9/atomman/library/xsd/
+-rw-rw-rw-   0        0        0        0 2021-08-03 11:18:29.000000 atomman-1.4.9/atomman/library/xsd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.930652 atomman-1.4.9/atomman/library/xsl/
+-rw-rw-rw-   0        0        0        0 2021-08-03 11:18:29.000000 atomman-1.4.9/atomman/library/xsl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.931643 atomman-1.4.9/atomman/load/
+-rw-rw-rw-   0        0        0     1726 2022-10-11 20:58:20.000000 atomman-1.4.9/atomman/load/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.933687 atomman-1.4.9/atomman/load/ase_Atoms/
+-rw-rw-rw-   0        0        0       39 2019-10-21 20:07:58.000000 atomman-1.4.9/atomman/load/ase_Atoms/__init__.py
+-rw-rw-rw-   0        0        0     1585 2022-10-11 20:58:19.000000 atomman-1.4.9/atomman/load/ase_Atoms/load.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.939684 atomman-1.4.9/atomman/load/atom_data/
+-rw-rw-rw-   0        0        0      141 2019-10-21 20:07:40.000000 atomman-1.4.9/atomman/load/atom_data/__init__.py
+-rw-rw-rw-   0        0        0    14733 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/atom_data/atoms_prop_info.py
+-rw-rw-rw-   0        0        0    13973 2022-10-11 20:58:18.000000 atomman-1.4.9/atomman/load/atom_data/load.py
+-rw-rw-rw-   0        0        0     3284 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/atom_data/velocities_prop_info.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.942683 atomman-1.4.9/atomman/load/atom_dump/
+-rw-rw-rw-   0        0        0       89 2019-10-21 20:16:44.000000 atomman-1.4.9/atomman/load/atom_dump/__init__.py
+-rw-rw-rw-   0        0        0    10365 2022-10-11 20:58:17.000000 atomman-1.4.9/atomman/load/atom_dump/load.py
+-rw-rw-rw-   0        0        0     9630 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/atom_dump/process_prop_info.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.944643 atomman-1.4.9/atomman/load/cif/
+-rw-rw-rw-   0        0        0       39 2019-10-21 20:03:55.000000 atomman-1.4.9/atomman/load/cif/__init__.py
+-rw-rw-rw-   0        0        0     1956 2022-10-11 20:58:16.000000 atomman-1.4.9/atomman/load/cif/load.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.947682 atomman-1.4.9/atomman/load/crystal/
+-rw-rw-rw-   0        0        0       22 2020-07-23 19:09:45.000000 atomman-1.4.9/atomman/load/crystal/__init__.py
+-rw-rw-rw-   0        0        0     6396 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/crystal/load.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.950680 atomman-1.4.9/atomman/load/dft_reference/
+-rw-rw-rw-   0        0        0       22 2021-08-04 15:10:28.000000 atomman-1.4.9/atomman/load/dft_reference/__init__.py
+-rw-rw-rw-   0        0        0     2983 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/dft_reference/load.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.952679 atomman-1.4.9/atomman/load/phonopy_Atoms/
+-rw-rw-rw-   0        0        0       39 2019-10-21 20:03:35.000000 atomman-1.4.9/atomman/load/phonopy_Atoms/__init__.py
+-rw-rw-rw-   0        0        0     1699 2022-10-11 20:58:15.000000 atomman-1.4.9/atomman/load/phonopy_Atoms/load.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.954681 atomman-1.4.9/atomman/load/poscar/
+-rw-rw-rw-   0        0        0       39 2019-10-21 20:03:19.000000 atomman-1.4.9/atomman/load/poscar/__init__.py
+-rw-rw-rw-   0        0        0     3124 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/poscar/load.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.956680 atomman-1.4.9/atomman/load/prototype/
+-rw-rw-rw-   0        0        0       22 2020-07-23 19:09:45.000000 atomman-1.4.9/atomman/load/prototype/__init__.py
+-rw-rw-rw-   0        0        0     9720 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/prototype/load.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.959646 atomman-1.4.9/atomman/load/pymatgen_Structure/
+-rw-rw-rw-   0        0        0       39 2019-10-21 20:02:57.000000 atomman-1.4.9/atomman/load/pymatgen_Structure/__init__.py
+-rw-rw-rw-   0        0        0     1590 2022-10-11 20:58:14.000000 atomman-1.4.9/atomman/load/pymatgen_Structure/load.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.961680 atomman-1.4.9/atomman/load/spglib_cell/
+-rw-rw-rw-   0        0        0       39 2019-10-21 20:02:34.000000 atomman-1.4.9/atomman/load/spglib_cell/__init__.py
+-rw-rw-rw-   0        0        0     1030 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/spglib_cell/load.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.964645 atomman-1.4.9/atomman/load/system_model/
+-rw-rw-rw-   0        0        0       39 2019-10-21 20:02:23.000000 atomman-1.4.9/atomman/load/system_model/__init__.py
+-rw-rw-rw-   0        0        0     6303 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/system_model/load.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.968681 atomman-1.4.9/atomman/load/table/
+-rw-rw-rw-   0        0        0       89 2019-10-21 20:01:33.000000 atomman-1.4.9/atomman/load/table/__init__.py
+-rw-rw-rw-   0        0        0     5246 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/table/load.py
+-rw-rw-rw-   0        0        0     5527 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/load/table/process_prop_info.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.971680 atomman-1.4.9/atomman/mep/
+-rw-rw-rw-   0        0        0    12671 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/mep/BasePath.py
+-rw-rw-rw-   0        0        0    10414 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/mep/ISMPath.py
+-rw-rw-rw-   0        0        0     2165 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/mep/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.973681 atomman-1.4.9/atomman/mep/gradient/
+-rw-rw-rw-   0        0        0      103 2021-02-22 17:04:15.000000 atomman-1.4.9/atomman/mep/gradient/__init__.py
+-rw-rw-rw-   0        0        0     1714 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/mep/gradient/central_difference.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.978645 atomman-1.4.9/atomman/mep/integrator/
+-rw-rw-rw-   0        0        0      114 2021-02-22 17:04:37.000000 atomman-1.4.9/atomman/mep/integrator/__init__.py
+-rw-rw-rw-   0        0        0      892 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/mep/integrator/euler.py
+-rw-rw-rw-   0        0        0     1133 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/mep/integrator/rungekutta.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.981647 atomman-1.4.9/atomman/plot/
+-rw-rw-rw-   0        0        0      106 2019-10-21 18:43:36.000000 atomman-1.4.9/atomman/plot/__init__.py
+-rw-rw-rw-   0        0        0    18778 2023-01-26 22:32:59.000000 atomman-1.4.9/atomman/plot/interpolate_contour.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.991655 atomman-1.4.9/atomman/region/
+-rw-rw-rw-   0        0        0     4210 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/region/Cylinder.py
+-rw-rw-rw-   0        0        0     5557 2022-06-01 13:44:35.000000 atomman-1.4.9/atomman/region/Plane.py
+-rw-rw-rw-   0        0        0     2196 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/region/PlaneSet.py
+-rw-rw-rw-   0        0        0     1740 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/region/Shape.py
+-rw-rw-rw-   0        0        0     2301 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/region/Sphere.py
+-rw-rw-rw-   0        0        0      229 2020-08-24 20:38:08.000000 atomman-1.4.9/atomman/region/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:29.000645 atomman-1.4.9/atomman/thermo/
+-rw-rw-rw-   0        0        0     3809 2022-11-03 19:11:23.000000 atomman-1.4.9/atomman/thermo/EinsteinSolid.py
+-rw-rw-rw-   0        0        0     2105 2022-11-03 19:09:25.000000 atomman-1.4.9/atomman/thermo/IdealGas.py
+-rw-rw-rw-   0        0        0     8228 2023-03-10 19:19:42.000000 atomman-1.4.9/atomman/thermo/RDF.py
+-rw-rw-rw-   0        0        0    76536 2022-11-03 19:12:50.000000 atomman-1.4.9/atomman/thermo/UhlenbeckFordModel.py
+-rw-rw-rw-   0        0        0      146 2022-11-03 19:13:01.000000 atomman-1.4.9/atomman/thermo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:29.016645 atomman-1.4.9/atomman/tools/
+-rw-rw-rw-   0        0        0      937 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/tools/__init__.py
+-rw-rw-rw-   0        0        0     1278 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/tools/axes_check.py
+-rw-rw-rw-   0        0        0      955 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/tools/boolean.py
+-rw-rw-rw-   0        0        0     1075 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/tools/compositionstr.py
+-rw-rw-rw-   0        0        0     9197 2022-03-25 15:50:03.000000 atomman-1.4.9/atomman/tools/crystalsystem.py
+-rw-rw-rw-   0        0        0     6290 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/tools/duplicates_allclose.py
+-rw-rw-rw-   0        0        0     2627 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/tools/filltemplate.py
+-rw-rw-rw-   0        0        0     1158 2022-03-15 16:07:49.000000 atomman-1.4.9/atomman/tools/indexstr.py
+-rw-rw-rw-   0        0        0    15048 2022-12-09 16:03:02.000000 atomman-1.4.9/atomman/tools/miller.py
+-rw-rw-rw-   0        0        0     1552 2022-12-15 20:45:30.000000 atomman-1.4.9/atomman/tools/vect_angle.py
+-rw-rw-rw-   0        0        0    12639 2022-03-15 16:07:50.000000 atomman-1.4.9/atomman/unitconvert.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:28.756667 atomman-1.4.9/atomman.egg-info/
+-rw-rw-rw-   0        0        0     5054 2023-04-18 20:26:28.000000 atomman-1.4.9/atomman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6356 2023-04-18 20:26:28.000000 atomman-1.4.9/atomman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 20:26:28.000000 atomman-1.4.9/atomman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-07-10 18:43:04.000000 atomman-1.4.9/atomman.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      115 2023-04-18 20:26:28.000000 atomman-1.4.9/atomman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 20:26:28.000000 atomman-1.4.9/atomman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      154 2022-04-01 16:42:36.000000 atomman-1.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 20:26:29.020681 atomman-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     2075 2023-04-05 14:06:18.000000 atomman-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:26:29.018683 atomman-1.4.9/tests/
+-rw-rw-rw-   0        0        0      238 2022-02-16 20:04:46.000000 atomman-1.4.9/tests/test_root.py
+-rw-rw-rw-   0        0        0     1542 2022-10-03 15:24:21.000000 atomman-1.4.9/tests/test_unitconvert.py
```

### Comparing `atomman-1.4.8/LICENSE.TXT` & `atomman-1.4.9/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/PKG-INFO` & `atomman-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomman
-Version: 1.4.8
+Version: 1.4.9
 Summary: Atomistic Manipulation Toolkit
 Home-page: https://github.com/usnistgov/atomman/
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: atom,atomic,atomistic,molecular dynamics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `atomman-1.4.8/README.rst` & `atomman-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/UPDATES.rst` & `atomman-1.4.9/UPDATES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 Updates
 =======
+
+Version 1.4.9
+-------------
+
+- **atomman.thermo.RDF** updates to support more general use.
+
+- Handling of record queries updated to be consistent with yabadaba 0.2.0.
+
 Version 1.4.8
 -------------
 
 - **atomman.thermo** module added that provides tools and reference models
   related to thermodynamic calculations.
 
 - **atomman.tools.vect_angle** updated to allow for comparisons of multiple
```

### Comparing `atomman-1.4.8/atomman/__init__.py` & `atomman-1.4.9/atomman/__init__.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/cluster/BondAngleMap.py` & `atomman-1.4.9/atomman/cluster/BondAngleMap.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/Atoms.py` & `atomman-1.4.9/atomman/core/Atoms.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/Box.py` & `atomman-1.4.9/atomman/core/Box.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/ElasticConstants.py` & `atomman-1.4.9/atomman/core/ElasticConstants.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/NeighborList.py` & `atomman-1.4.9/atomman/core/NeighborList.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/System.py` & `atomman-1.4.9/atomman/core/System.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/displacement.py` & `atomman-1.4.9/atomman/core/displacement.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/dmag.c` & `atomman-1.4.9/atomman/core/dmag.c`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/dmag.pyx` & `atomman-1.4.9/atomman/core/dmag.pyx`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/dvect.c` & `atomman-1.4.9/atomman/core/dvect.c`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/dvect.pyx` & `atomman-1.4.9/atomman/core/dvect.pyx`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/nlist.c` & `atomman-1.4.9/atomman/core/nlist.c`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/core/nlist.pyx` & `atomman-1.4.9/atomman/core/nlist.pyx`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/DifferentialDisplacement.py` & `atomman-1.4.9/atomman/defect/DifferentialDisplacement.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/Dislocation/__init__.py` & `atomman-1.4.9/atomman/defect/Dislocation/__init__.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/Dislocation/_dipole.py` & `atomman-1.4.9/atomman/defect/Dislocation/_dipole.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/Dislocation/_monopole.py` & `atomman-1.4.9/atomman/defect/Dislocation/_monopole.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/Dislocation/_periodicarray.py` & `atomman-1.4.9/atomman/defect/Dislocation/_periodicarray.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/FreeSurface.py` & `atomman-1.4.9/atomman/defect/FreeSurface.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/GammaSurface.py` & `atomman-1.4.9/atomman/defect/GammaSurface.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/IsotropicVolterraDislocation.py` & `atomman-1.4.9/atomman/defect/IsotropicVolterraDislocation.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/SDVPN.py` & `atomman-1.4.9/atomman/defect/SDVPN.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/StackingFault.py` & `atomman-1.4.9/atomman/defect/StackingFault.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/Strain.c` & `atomman-1.4.9/atomman/defect/Strain.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "atomman.defect.Strain",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -212,15 +212,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -251,15 +251,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -26549,28 +26549,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
```

### Comparing `atomman-1.4.8/atomman/defect/Strain.pyx` & `atomman-1.4.9/atomman/defect/Strain.pyx`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/Stroh.py` & `atomman-1.4.9/atomman/defect/Stroh.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/VolterraDislocation.py` & `atomman-1.4.9/atomman/defect/VolterraDislocation.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/__init__.py` & `atomman-1.4.9/atomman/defect/__init__.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/differential_displacement.py` & `atomman-1.4.9/atomman/defect/differential_displacement.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/dislocation_array.py` & `atomman-1.4.9/atomman/defect/dislocation_array.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/dislocation_dipole_displacement.py` & `atomman-1.4.9/atomman/defect/dislocation_dipole_displacement.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/dislocation_system_basis.py` & `atomman-1.4.9/atomman/defect/dislocation_system_basis.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/dislocation_system_transform.py` & `atomman-1.4.9/atomman/defect/dislocation_system_transform.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/disregistry.py` & `atomman-1.4.9/atomman/defect/disregistry.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/free_surface_basis.py` & `atomman-1.4.9/atomman/defect/free_surface_basis.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/nye_tensor.py` & `atomman-1.4.9/atomman/defect/nye_tensor.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/nye_tensor_p.py` & `atomman-1.4.9/atomman/defect/nye_tensor_p.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/pn_arctan_disldensity.py` & `atomman-1.4.9/atomman/defect/pn_arctan_disldensity.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/pn_arctan_disregistry.py` & `atomman-1.4.9/atomman/defect/pn_arctan_disregistry.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/point.py` & `atomman-1.4.9/atomman/defect/point.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/slip_vector.c` & `atomman-1.4.9/atomman/defect/slip_vector.c`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/slip_vector.pyx` & `atomman-1.4.9/atomman/defect/slip_vector.pyx`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/defect/solve_volterra_dislocation.py` & `atomman-1.4.9/atomman/defect/solve_volterra_dislocation.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/__init__.py` & `atomman-1.4.9/atomman/dump/__init__.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/ase_Atoms/dump.py` & `atomman-1.4.9/atomman/dump/ase_Atoms/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/atom_data/atoms_prop_info.py` & `atomman-1.4.9/atomman/dump/atom_data/atoms_prop_info.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/atom_data/dump.py` & `atomman-1.4.9/atomman/dump/atom_data/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/atom_data/velocities_prop_info.py` & `atomman-1.4.9/atomman/dump/atom_data/velocities_prop_info.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/atom_dump/dump.py` & `atomman-1.4.9/atomman/dump/atom_dump/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/atom_dump/process_prop_info.py` & `atomman-1.4.9/atomman/dump/atom_dump/process_prop_info.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/conventional_to_primitive/dump.py` & `atomman-1.4.9/atomman/dump/conventional_to_primitive/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/lammps_commands/dump.py` & `atomman-1.4.9/atomman/dump/lammps_commands/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/phonopy_Atoms/dump.py` & `atomman-1.4.9/atomman/dump/phonopy_Atoms/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/poscar/dump.py` & `atomman-1.4.9/atomman/dump/poscar/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/primitive_cell/dump.py` & `atomman-1.4.9/atomman/dump/primitive_cell/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/primitive_to_conventional/dump.py` & `atomman-1.4.9/atomman/dump/primitive_to_conventional/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/pymatgen_Structure/dump.py` & `atomman-1.4.9/atomman/dump/pymatgen_Structure/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/spglib_cell/dump.py` & `atomman-1.4.9/atomman/dump/spglib_cell/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/system_model/dump.py` & `atomman-1.4.9/atomman/dump/system_model/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/table/dump.py` & `atomman-1.4.9/atomman/dump/table/dump.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/dump/table/process_prop_info.py` & `atomman-1.4.9/atomman/dump/table/process_prop_info.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/lammps/Log.py` & `atomman-1.4.9/atomman/lammps/Log.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/lammps/NEBLog.py` & `atomman-1.4.9/atomman/lammps/NEBLog.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/lammps/Potential.py` & `atomman-1.4.9/atomman/lammps/Potential.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/lammps/__init__.py` & `atomman-1.4.9/atomman/lammps/__init__.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/lammps/checkversion.py` & `atomman-1.4.9/atomman/lammps/checkversion.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/lammps/normalize.py` & `atomman-1.4.9/atomman/lammps/normalize.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/lammps/run.py` & `atomman-1.4.9/atomman/lammps/run.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/lammps/style.py` & `atomman-1.4.9/atomman/lammps/style.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/library/Database/__init__.py` & `atomman-1.4.9/atomman/library/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/library/Database/_crystal_prototype.py` & `atomman-1.4.9/atomman/library/Database/_crystal_prototype.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/library/Database/_reference_crystal.py` & `atomman-1.4.9/atomman/library/Database/_reference_crystal.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,19 +428,19 @@
         except:
             pass
 
     # Fetch from source database
     if 'oqmd-' in id:
         record = self.fetch_oqmd_crystal(id)
         if verbose:
-            print(f'Crystal retrieved from OQMD')
+            print('Crystal retrieved from OQMD')
     else:
         record = self.fetch_mp_crystal(id, api_key=api_key)
         if verbose:
-            print(f'Crystal retrieved from Materials Project')
+            print('Crystal retrieved from Materials Project')
 
     return record
 
 def fetch_mp_crystals(self,
                       id: str,
                       api_key: Optional[str] = None) -> list:
     """
```

### Comparing `atomman-1.4.8/atomman/library/Database/_relaxed_crystal.py` & `atomman-1.4.9/atomman/library/Database/_relaxed_crystal.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/library/load_lammps_potential.py` & `atomman-1.4.9/atomman/library/load_lammps_potential.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/library/record/CrystalPrototype.py` & `atomman-1.4.9/atomman/library/record/ReferenceCrystal.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # coding: utf-8
 
 # Standard Python imports
 import io
 from typing import Optional, Union, Tuple
+import uuid
 
 # https://github.com/usnistgov/DataModelDict
 from DataModelDict import DataModelDict as DM
 
 # https://github.com/usnistgov/yabadaba
 from yabadaba.record import Record
 from yabadaba import load_query
 
-# https://pandas.pydata.org/
-import pandas as pd
-
 # atomman imports
 from ... import System
 
-class CrystalPrototype(Record):
+class ReferenceCrystal(Record):
     """
-    Class for representing crystal_prototype records that describe common
-    crystal prototypes.
+    Class for representing reference_crystal records that provide the structure
+    information for DFT relaxed crystal structures obtained from DFT databases.
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None):
         """
         Initializes a Record object for a given style.
         
@@ -33,395 +31,408 @@
         model : str, file-like object, DataModelDict
             The contents of the record.
         name : str, optional
             The unique name to assign to the record.  If model is a file
             path, then the default record name is the file name without
             extension.
         """
-        if model is not None:
-            super().__init__(model=model, name=name)
-        elif name is not None:
-            self.name = name
+        # Init properties
+        self.__composition = None
+        self.__symbols = None
+        self.__natoms = None
+        self.__natypes = None
+        self.__crystalfamily = None
+        self.__a = None
+        self.__b = None
+        self.__c = None
+        self.__alpha = None
+        self.__beta = None
+        self.__gamma = None
+        self.__ucell = None
+
+        # Call super init
+        super().__init__(model=model, name=name)
 
     @property
     def style(self) -> str:
         """str: The record style"""
-        return 'crystal_prototype'
+        return 'reference_crystal'
 
     @property
     def modelroot(self) -> str:
         """str: The root element of the content"""
-        return 'crystal-prototype'
+        return 'reference-crystal'
 
     @property
     def xsd_filename(self) -> Tuple[str, str]:
         """tuple: The module path and file name of the record's xsd schema"""
         return ('atomman.library.xsd', f'{self.style}.xsd')
 
+    @property
+    def xsl_filename(self) -> Tuple[str, str]:
+        """tuple: The module path and file name of the record's xsl transformer"""
+        return ('atomman.library.xsl', f'{self.style}.xsl')
+    
+    @property
+    def id(self) -> str:
+        """str : The unique id for the record"""
+        return self.__id
+
+    @id.setter
+    def id(self, value: str):
+        if value is None:
+            self.__id = None
+        else:
+            self.__id = str(value)
+
+    @property
+    def key(self) -> str:
+        """str : A UUID4 key assigned to the record"""
+        return self.__key
+
+    @key.setter
+    def key(self, value: str):
+        if value is None:
+            self.__key = str(uuid.uuid4())
+        else:
+            self.__key = str(value)
+
+    @property
+    def sourcename(self) -> str:
+        """str : Name of the crystal's source database"""
+        return self.__sourcename
+
+    @sourcename.setter
+    def sourcename(self, value: str):
+        if value is None:
+            self.__sourcename = None
+        else:
+            self.__sourcename = str(value)
+
+    @property
+    def sourcelink(self) -> str:
+        """str : URL for the crystal's source database"""
+        return self.__sourcelink    
+
+    @sourcelink.setter
+    def sourcelink(self, value: str):
+        if value is None:
+            self.__sourcelink = None
+        else:
+            self.__sourcelink = str(value)
+
+    @property
+    def ucell(self) -> System:
+        """atomman.System : The unit cell system for the crystal"""
+        if self.__ucell is None:
+            raise ValueError('ucell information not set')
+        elif not isinstance(self.__ucell, System):
+            self.__ucell = System(model=self.__ucell)
+        return self.__ucell
+
+    @ucell.setter
+    def ucell(self, value: System):
+        if isinstance(value, System):
+            self.__ucell = value
+        else:
+            raise TypeError('ucell must be an atomman.System')
+
+    @property
+    def composition(self) -> str:
+        """str : The crystal's composition"""
+        if self.__composition is None:
+            self.__composition = self.ucell.composition
+        return self.__composition
+
+    @property
+    def symbols(self) -> list:
+        """list : The list of element model symbols"""
+        if self.__symbols is None:
+            self.__symbols = self.ucell.symbols
+        return self.__symbols
+
+    @property
+    def natoms(self) -> int:
+        """int : The number of atoms in the unit cell"""
+        if self.__natoms is None:
+            self.__natoms = self.ucell.natoms
+        return self.__natoms
+
+    @property
+    def natypes(self) -> int:
+        """int : The number of atom types in the unit cell"""
+        if self.__natypes is None:
+            self.__natypes = self.ucell.natypes
+        return self.__natypes
+
+    @property
+    def crystalfamily(self) -> str:
+        """str : The crystal's system family"""
+        if self.__crystalfamily is None:
+            self.__crystalfamily = self.ucell.box.identifyfamily()
+        return self.__crystalfamily
+
+    @property
+    def a(self) -> float:
+        """float : The unit cell's a lattice parameter"""
+        if self.__a is None:
+            self.__a = self.ucell.box.a
+        return self.__a
+
+    @property
+    def b(self) -> float:
+        """float : The unit cell's b lattice parameter"""
+        if self.__b is None:
+            self.__b = self.ucell.box.b
+        return self.__b
+
+    @property
+    def c(self) -> float:
+        """float : The unit cell's c lattice parameter"""
+        if self.__c is None:
+            self.__c = self.ucell.box.c
+        return self.__c
+
+    @property
+    def alpha(self) -> float:
+        """float : The unit cell's alpha lattice angle"""
+        if self.__alpha is None:
+            self.__alpha = self.ucell.box.alpha
+        return self.__alpha
+
+    @property
+    def beta(self) -> float:
+        """float : The unit cell's beta lattice angle"""
+        if self.__beta is None:
+            self.__beta = self.ucell.box.beta
+        return self.__beta
+
+    @property
+    def gamma(self) -> float:
+        """float : The unit cell's gamma lattice angle"""
+        if self.__gamma is None:
+            self.__gamma = self.ucell.box.gamma
+        return self.__gamma
+
+    def set_values(self,
+                   name: Optional[str] = None,
+                   id: Optional[str] = None,
+                   key: Optional[str] = None,
+                   sourcename: Optional[str] = None,
+                   sourcelink: Optional[str] = None,
+                   ucell: Optional[System] = None):
+        """
+        Sets multiple object values.
+
+        Parameters
+        ----------
+        name : str, optional
+            The name to use for saving the record.  Either name or id should
+            be given as they are treated as aliases for this record style.
+        id : str, optional
+            The unique identifier for the record.  Should be composed of a
+            source database tag plus the source database's unique identifier.
+        key : str, optional
+            A UUID4 key assigned to the record.  Note that if not given a new
+            random key will be assigned and therefore the keys might not match
+            if similar records were generated independently.
+        sourcename : str, optional
+            The name of the source database where the reference record was
+            retrieved.
+        sourcelink : str, optional
+            The URL to the source database where the reference record was
+            retrieved.
+        ucell : atomman.System, optional
+            A small unit cell system associated with the reference crystal.
+        """
+        
+        if name is None and id is not None:
+            self.name = id
+            self.id = id
+        elif name is not None and id is None:
+            self.name = name
+            self.id = name
+        else:
+            self.name = name
+            self.id = id
+
+        self.key = key
+        self.sourcename = sourcename
+        self.sourcelink = sourcelink
+        if ucell is not None:
+            self.ucell = ucell
+        
+        self.__symbols = None
+        self.__composition = None
+        self.__crystalfamily = None
+        self.__natypes = None
+        self.__a = None
+        self.__b = None
+        self.__c = None
+        self.__alpha = None
+        self.__beta = None
+        self.__gamma = None
+
+    def build_model(self) -> DM:
+        """
+        Returns the object info as data model content
+        
+        Returns
+        ----------
+        DataModelDict
+            The data model content.
+        """
+
+        refmodel = DM()
+        
+        refmodel['key'] = self.key
+        refmodel['id'] = self.id
+
+        refmodel['source'] = DM()
+        refmodel['source']['name'] = self.sourcename
+        refmodel['source']['link'] = self.sourcelink
+        
+        refmodel['system-info'] = DM()
+        symbols = self.symbols
+        if len(symbols) == 1:
+            refmodel['system-info']['symbol'] = self.symbols[0]
+        else:
+            refmodel['system-info']['symbol'] = self.symbols
+        refmodel['system-info']['composition'] = self.composition
+        
+        refmodel['system-info']['cell'] = DM()
+        refmodel['system-info']['cell']['crystal-family'] = self.crystalfamily
+        refmodel['system-info']['cell']['natypes'] = self.natypes
+        refmodel['system-info']['cell']['a'] = self.a
+        refmodel['system-info']['cell']['b'] = self.b
+        refmodel['system-info']['cell']['c'] = self.c
+        refmodel['system-info']['cell']['alpha'] = self.alpha
+        refmodel['system-info']['cell']['beta'] = self.beta
+        refmodel['system-info']['cell']['gamma'] = self.gamma
+        
+        refmodel['atomic-system'] = self.ucell.model()['atomic-system']
+
+        model = DM([('reference-crystal', refmodel)])
+        self._set_model(model)
+        return model
+        
     def load_model(self,
                    model: Union[str, io.IOBase, DM],
                    name: Optional[str] = None):
         """
         Loads record contents from a given model.
 
         Parameters
         ----------
         model : str or DataModelDict
             The model contents of the record to load.
         name : str, optional
             The name to assign to the record.  Often inferred from other
             attributes if not given.
         """
-        super().load_model(model, name=name)        
-        proto = self.model[self.modelroot]
+        super().load_model(model, name=name)
+        crystal = self.model[self.modelroot]
         
-        self.__key = proto['key']
-        self.__id = proto['id']
-        self.__commonname = proto['name']
-        self.__prototype = proto['prototype']
-        self.__pearson = proto['Pearson-symbol']
-        self.__strukturbericht = proto['Strukturbericht']
-        
-        self.__sg_number = proto['space-group']['number']
-        self.__sg_hm = proto['space-group']['Hermann-Maguin']
-        self.__sg_schoenflies = proto['space-group']['Schoenflies']
+        self.__key = crystal['key']
+        self.__id = crystal['id']
+        self.__sourcename = crystal['source']['name']
+        self.__sourcelink = crystal['source']['link']
         
-        self.__crystalfamily = proto['system-info']['cell']['crystal-family']
-        self.__natypes = proto['system-info']['cell']['natypes']
-        self.__ucell = None
+        self.__symbols = crystal['system-info'].aslist('symbol')
+        self.__composition = crystal['system-info']['composition']
+        self.__crystalfamily = crystal['system-info']['cell']['crystal-family']
+        self.__natypes = crystal['system-info']['cell']['natypes']
+        self.__a = crystal['system-info']['cell']['a']
+        self.__b = crystal['system-info']['cell']['b']
+        self.__c = crystal['system-info']['cell']['c']
+        self.__alpha = crystal['system-info']['cell']['alpha']
+        self.__beta = crystal['system-info']['cell']['beta']
+        self.__gamma = crystal['system-info']['cell']['gamma']
+
+        self.__natoms = crystal['atomic-system']['atoms']['natoms']
+
+        self.__ucell = crystal
 
         # Set name as id if no name given
         try:
             self.name
-        except:
+        except AttributeError:
             self.name = self.id
 
-    @property
-    def id(self) -> str:
-        """str : A unique id assigned to the record"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__id
-
-    @property
-    def key(self) -> str:
-        """str : A UUID4 key assigned to the record"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__key
-
-    @property
-    def commonname(self) -> str:
-        """str : A common name associated with the prototype"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__commonname
-    
-    @property
-    def prototype(self) -> str:
-        """str : A prototype composition associated with the prototype"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__prototype
-    
-    @property
-    def pearson(self) -> str:
-        """str : The prototype's Pearson symbol"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__pearson
-
-    @property
-    def strukturbericht(self) -> str:
-        """str : The prototype's Strukturbericht symbol"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__strukturbericht
-
-    @property
-    def sg_number(self) -> int:
-        """int : The prototype's space group number"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__sg_number
-
-    @property
-    def sg_hm(self) -> str:
-        """str : The prototype's space group international symbol"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__sg_hm
-
-    @property
-    def sg_schoenflies(self) -> str:
-        """str : The prototype's space group Schoenflies symbol"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__sg_schoenflies
-
-    @property
-    def crystalfamily(self) -> str:
-        """str : The prototype's system family"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__crystalfamily
-
-    @property
-    def natypes(self) -> int:
-        """int : Number of atom types"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__natypes
-
-    @property
-    def ucell(self) -> System:
-        """atomman.System : The unit cell for the prototype""" 
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        if self.__ucell is None:
-            self.__ucell = System(model=self.model)
-        return self.__ucell
-
-    def build_model(self) -> DM:
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.model
-
     def metadata(self) -> dict:
         """
         Generates a dict of simple metadata values associated with the record.
         Useful for quickly comparing records and for building pandas.DataFrames
         for multiple records of the same style.
         """
         params = {}
         params['name'] = self.name
         params['key'] = self.key
         params['id'] = self.id
-        params['commonname'] = self.commonname
-        params['prototype'] = self.prototype
-        params['pearson'] = self.pearson
-        params['strukturbericht'] = self.strukturbericht
-        params['sg_number'] = self.sg_number
-        params['sg_hm'] = self.sg_hm
-        params['sg_schoenflies'] = self.sg_schoenflies
+        params['sourcename'] = self.sourcename
+        params['sourcelink'] = self.sourcelink
+
         params['crystalfamily'] = self.crystalfamily
         params['natypes'] = self.natypes
-        
+        params['symbols'] = self.symbols
+        params['composition'] = self.composition
+
+        params['a'] = self.a
+        params['b'] = self.b
+        params['c'] = self.c
+        params['alpha'] = self.alpha
+        params['beta'] = self.beta
+        params['gamma'] = self.gamma
+        params['natoms'] = self.natoms
+
         return params
 
     @property
     def queries(self) -> dict:
         """dict: Query objects and their associated parameter names."""
         return {
             'key': load_query(
                 style='str_match',
                 name='key', 
-                path=f'{self.modelroot}.key'),
+                path=f'{self.modelroot}.key',
+                description="search by reference crystal's UUID key"),
             'id': load_query(
                 style='str_match',
                 name='id',
-                path=f'{self.modelroot}.id'),
-            'commonname': load_query(
-                style='str_match',
-                name='commonname',
-                path=f'{self.modelroot}.name'),
-            'prototype': load_query(
-                style='str_match',
-                name='prototype',
-                path=f'{self.modelroot}.prototype'),
-            'pearson': load_query(
+                path=f'{self.modelroot}.id',
+                description="search by reference crystal's id"),
+            'sourcename': load_query(
                 style='str_match',
-                name='pearson',
-                path=f'{self.modelroot}.Pearson-symbol'),
-            'strukturbericht': load_query(
+                name='sourcename',
+                path=f'{self.modelroot}.source.name',
+                description='search by name of the source'),
+            'sourcelink': load_query(
                 style='str_match',
-                name='strukturbericht',
-                path=f'{self.modelroot}.Strukturbericht'),
-            'sg_number': load_query(
-                style='int_match',
-                name='sg_number',
-                path=f'{self.modelroot}.space-group.number'),
-            'sg_hm': load_query(
-                style='str_match',
-                name='sg_hm',
-                path=f'{self.modelroot}.space-group.Hermann-Maguin'),
-            'sg_schoenflies': load_query(
-                style='str_match',
-                name='sg_schoenflies',
-                path=f'{self.modelroot}.space-group.Schoenflies'),
+                name='sourcelink',
+                path=f'{self.modelroot}.source.link',
+                description='search by URL host link for the source'),
             'crystalfamily': load_query(
                 style='str_match',
                 name='crystalfamily',
-                path=f'{self.modelroot}.system-info.cell.crystal-family'),
+                path=f'{self.modelroot}.system-info.cell.crystal-family',
+                description="search by reference crystal's crystal family"),
+            'composition': load_query(
+                style='str_match',
+                name='composition',
+                path=f'{self.modelroot}.system-info.composition',
+                description="search by reference crystal's composition"),
+            'symbols': load_query(
+                style='list_contains',
+                name='symbols',
+                path=f'{self.modelroot}.system-info.symbol',
+                description="search by reference crystal's symbols"),
+            'natoms': load_query(
+                style='int_match',
+                name='natoms',
+                path=f'{self.modelroot}.atomic-system.atoms.natoms',
+                description="search by number of atoms in the reference crystal"),
             'natypes': load_query(
                 style='int_match',
                 name='natypes',
-                path=f'{self.modelroot}.system-info.cell.natypes'),
+                path=f'{self.modelroot}.system-info.cell.natypes',
+                description="search by number of atom types in the reference crystal"),
         }
-
-    def pandasfilter(self,
-                     dataframe: pd.DataFrame,
-                     name: Union[str, list, None] = None,
-                     id: Union[str, list, None] = None,
-                     key: Union[str, list, None] = None,
-                     commonname: Union[str, list, None] = None,
-                     prototype: Union[str, list, None] = None,
-                     pearson: Union[str, list, None] = None,
-                     strukturbericht: Union[str, list, None] = None,
-                     sg_number: Union[int, list, None] = None,
-                     sg_hm: Union[str, list, None] = None,
-                     sg_schoenflies: Union[str, list, None] = None,
-                     crystalfamily: Union[str, list, None] = None,
-                     natypes: Union[int, list, None] = None) -> pd.Series:
-        """
-        Filters a pandas.DataFrame based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        dataframe : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        name : str or list
-            The record name(s) to parse by.
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        commonname : str or list
-            Prototype common name(s) to parse by.
-        prototype : str or list
-            Prototype composition(s) to parse by.
-        pearson : str or list
-            Pearson symbol(s) to parse by.
-        strukturbericht : str or list
-            Prototype Strukturbericht symbol(s) to parse by.
-        sg_number : int or list
-            Space group number(s) to parse by.
-        sg_hm : str or list
-            Space group international symbol(s) to parse by.
-        sg_schoenflies : str or list
-            Space group Schoenflies symbol(s) to parse by.
-        crystalfamily : str or list
-            Crystal structure families to parse by.
-        natypes : int or list
-            Number of atom types to parse by.
-
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-        matches = super().pandasfilter(dataframe, name=name, id=id, key=key,
-                                       commonname=commonname, prototype=prototype,
-                                       pearson=pearson, strukturbericht=strukturbericht,
-                                       sg_number=sg_number, sg_hm=sg_hm,
-                                       sg_schoenflies=sg_schoenflies,
-                                       crystalfamily=crystalfamily, natypes=natypes)
-        return matches
-
-    def mongoquery(self, 
-                   name: Union[str, list, None] = None,
-                   id: Union[str, list, None] = None,
-                   key: Union[str, list, None] = None,
-                   commonname: Union[str, list, None] = None,
-                   prototype: Union[str, list, None] = None,
-                   pearson: Union[str, list, None] = None,
-                   strukturbericht: Union[str, list, None] = None,
-                   sg_number: Union[int, list, None] = None,
-                   sg_hm: Union[str, list, None] = None,
-                   sg_schoenflies: Union[str, list, None] = None,
-                   crystalfamily: Union[str, list, None] = None,
-                   natypes: Union[int, list, None] = None) -> dict:
-        """
-        Builds a Mongo-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        name : str or list
-            The record name(s) to parse by.
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        commonname : str or list
-            Prototype common name(s) to parse by.
-        prototype : str or list
-            Prototype composition(s) to parse by.
-        pearson : str or list
-            Pearson symbol(s) to parse by.
-        strukturbericht : str or list
-            Prototype Strukturbericht symbol(s) to parse by.
-        sg_number : int or list
-            Space group number(s) to parse by.
-        sg_hm : str or list
-            Space group international symbol(s) to parse by.
-        sg_schoenflies : str or list
-            Space group Schoenflies symbol(s) to parse by.
-        crystalfamily : str or list
-            Crystal structure families to parse by.
-        natypes : int or list
-            Number of atom types to parse by.
-        
-        Returns
-        -------
-        dict
-            The Mongo-style query
-        """     
-        mquery = super().mongoquery(name=name, id=id, key=key,
-                                    commonname=commonname, prototype=prototype,
-                                    pearson=pearson, strukturbericht=strukturbericht,
-                                    sg_number=sg_number, sg_hm=sg_hm,
-                                    sg_schoenflies=sg_schoenflies,
-                                    crystalfamily=crystalfamily, natypes=natypes)
-        return mquery
-
-    def cdcsquery(self, 
-                  id: Union[str, list, None] = None,
-                  key: Union[str, list, None] = None,
-                  commonname: Union[str, list, None] = None,
-                  prototype: Union[str, list, None] = None,
-                  pearson: Union[str, list, None] = None,
-                  strukturbericht: Union[str, list, None] = None,
-                  sg_number: Union[int, list, None] = None,
-                  sg_hm: Union[str, list, None] = None,
-                  sg_schoenflies: Union[str, list, None] = None,
-                  crystalfamily: Union[str, list, None] = None,
-                  natypes: Union[int, list, None] = None) -> dict:
-        """
-        Builds a CDCS-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        commonname : str or list
-            Prototype common name(s) to parse by.
-        prototype : str or list
-            Prototype composition(s) to parse by.
-        pearson : str or list
-            Pearson symbol(s) to parse by.
-        strukturbericht : str or list
-            Prototype Strukturbericht symbol(s) to parse by.
-        sg_number : int or list
-            Space group number(s) to parse by.
-        sg_hm : str or list
-            Space group international symbol(s) to parse by.
-        sg_schoenflies : str or list
-            Space group Schoenflies symbol(s) to parse by.
-        crystalfamily : str or list
-            Crystal structure families to parse by.
-        natypes : int or list
-            Number of atom types to parse by.
-        
-        Returns
-        -------
-        dict
-            The CDCS-style query
-        """
-        mquery = super().cdcsquery(id=id, key=key,
-                                    commonname=commonname, prototype=prototype,
-                                    pearson=pearson, strukturbericht=strukturbericht,
-                                    sg_number=sg_number, sg_hm=sg_hm,
-                                    sg_schoenflies=sg_schoenflies,
-                                    crystalfamily=crystalfamily, natypes=natypes)
-        return mquery
```

### Comparing `atomman-1.4.8/atomman/library/record/Dislocation.py` & `atomman-1.4.9/atomman/library/record/Dislocation.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 from yabadaba.record import Record
 from yabadaba import load_query
 
 # http://www.numpy.org/
 import numpy as np
 import numpy.typing as npt
 
-# https://pandas.pydata.org/
-import pandas as pd
-
 class Dislocation(Record):
     """
     Class for representing dislocation records, which collect the parameters
     necessary for atomman to generate a particular dislocation type.
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
@@ -51,14 +48,19 @@
 
     @property
     def xsd_filename(self) -> Tuple[str, str]:
         """tuple: The module path and file name of the record's xsd schema"""
         return ('atomman.library.xsd', f'{self.style}.xsd')
 
     @property
+    def xsl_filename(self) -> Tuple[str, str]:
+        """tuple: The module path and file name of the record's xsl transformer"""
+        return ('atomman.library.xsl', f'{self.style}.xsl')
+
+    @property
     def modelroot(self) -> str:
         """str: The root element of the content"""
         return 'dislocation'
     
     @property
     def key(self) -> str:
         """str : A UUID4 key assigned to the record"""
@@ -164,16 +166,16 @@
         super().load_model(model, name=name)
         content = self.model[self.modelroot]
 
         self.key = content['key']
         self.id = content['id']
         self.character = content['character']
         self.burgers_vector = content['Burgers-vector']
-        self.slip_plane = content['slip-plane']
-        self.line_direction = content['line-direction']
+        self.slip_plane = np.asarray(content['slip-plane'], dtype=int)
+        self.line_direction = np.asarray(content['line-direction'], dtype=int)
         self.family = content['system-family']
         self.__parameters = dict(content['calculation-parameter'])
 
     def build_model(self) -> DM:
         """
         Returns the object info as data model content
         
@@ -228,114 +230,25 @@
     @property
     def queries(self) -> dict:
         """dict: Query objects and their associated parameter names."""
         return {
             'key': load_query(
                 style='str_match',
                 name='key', 
-                path=f'{self.modelroot}.key'),
+                path=f'{self.modelroot}.key',
+                description="search by dislocation parameter set's UUID key"),
             'id': load_query(
                 style='str_match',
                 name='id',
-                path=f'{self.modelroot}.id'),
+                path=f'{self.modelroot}.id',
+                description="search by dislocation parameter set's id"),
             'character': load_query(
                 style='str_match',
                 name='character',
-                path=f'{self.modelroot}.character'),
+                path=f'{self.modelroot}.character',
+                description="search by dislocation parameter set's dislocation character"),
             'family': load_query(
                 style='str_match',
                 name='family',
-                path=f'{self.modelroot}.system-family'),
+                path=f'{self.modelroot}.system-family',
+                description="search by the crystal prototype that the dislocation parameter set is for"),
         }
-
-    def pandasfilter(self,
-                     dataframe: pd.DataFrame,
-                     name: Union[str, list, None] = None,
-                     key: Union[str, list, None] = None,
-                     id: Union[str, list, None] = None,
-                     character: Union[str, list, None] = None,
-                     family: Union[str, list, None] = None) -> pd.Series:
-        """
-        Filters a pandas.DataFrame based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        dataframe : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        name : str or list
-            The record name(s) to parse by.
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        character : str or list
-            Dislocation character(s) to parse by.
-        family : str or list
-            Parent prototype/reference id(s) to parse by.
-        
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-        matches = super().pandasfilter(dataframe, name=name, key=key, id=id,
-                                       character=character, family=family)
-        return matches
-
-    def mongoquery(self,
-                   name: Union[str, list, None] = None,
-                   key: Union[str, list, None] = None,
-                   id: Union[str, list, None] = None,
-                   character: Union[str, list, None] = None,
-                   family: Union[str, list, None] = None) -> dict:
-        """
-        Builds a Mongo-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        name : str or list
-            The record name(s) to parse by.
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        character : str or list
-            Dislocation character(s) to parse by.
-        family : str or list
-            Parent prototype/reference id(s) to parse by.
-        
-        Returns
-        -------
-        dict
-            The Mongo-style query
-        """   
-        mquery = super().mongoquery(name=name, key=key, id=id,
-                                    character=character, family=family)
-        return mquery
-
-    def cdcsquery(self, 
-                  key: Union[str, list, None] = None,
-                  id: Union[str, list, None] = None,
-                  character: Union[str, list, None] = None,
-                  family: Union[str, list, None] = None) -> dict:
-        """
-        Builds a CDCS-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        character : str or list
-            Dislocation character(s) to parse by.
-        family : str or list
-            Parent prototype/reference id(s) to parse by.
-        
-        Returns
-        -------
-        dict
-            The CDCS-style query
-        """
-        mquery = super().cdcsquery(key=key, id=id,
-                                   character=character, family=family)
-        return mquery
```

### Comparing `atomman-1.4.8/atomman/library/record/FreeSurface.py` & `atomman-1.4.9/atomman/load/atom_dump/load.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,293 +1,260 @@
 # coding: utf-8
-
-# Standard Python imports
+# Standard Python libraries
 import io
-from typing import Optional, Union, Tuple
-
-# https://github.com/usnistgov/DataModelDict
-from DataModelDict import DataModelDict as DM
-
-# https://github.com/usnistgov/yabadaba
-from yabadaba.record import Record
-from yabadaba import load_query
-
-# https://pandas.pydata.org/
-import pandas as pd
-class FreeSurface(Record):
-    """
-    Class for representing free_surface records, which collect the parameters
-    necessary for atomman to generate a particular free surface.
+from collections import OrderedDict
+from typing import Optional, Tuple, Union
+                        
+# atomman imports
+import atomman.unitconvert as uc
+from ... import Atoms, Box, System
+from .process_prop_info import process_prop_info, standard_conversions
+from ...lammps import style
+from .. import load as amload
+from ...tools import uber_open_rmode
+
+def load(data: Union[str, io.IOBase],
+         symbols: Optional[tuple] = None,
+         lammps_units: str = 'metal',
+         prop_name: Optional[list] = None,
+         table_name: Optional[list] = None,
+         shape: Optional[list] = None,
+         unit: Optional[list] = None,
+         dtype: Optional[list] = None,
+         prop_info: Optional[list] = None,
+         return_prop_info: bool = False
+         ) -> Union[System, Tuple[System, list]]:
     """
-    def __init__(self,
-                 model: Union[str, io.IOBase, DM, None] = None,
-                 name: Optional[str] = None):
-        """
-        Initializes a Record object for a given style.
-        
-        Parameters
-        ----------
-        model : str, file-like object, DataModelDict
-            The contents of the record.
-        name : str, optional
-            The unique name to assign to the record.  If model is a file
-            path, then the default record name is the file name without
-            extension.
-        """
-        if model is not None:
-            super().__init__(model=model, name=name)
-        elif name is not None:
-            self.name = name
-
-    @property
-    def style(self) -> str:
-        """str: The record style"""
-        return 'free_surface'
-
-    @property
-    def xsd_filename(self) -> Tuple[str, str]:
-        """tuple: The module path and file name of the record's xsd schema"""
-        return ('atomman.library.xsd', f'{self.style}.xsd')
-
-    @property
-    def modelroot(self) -> str:
-        """str: The root element of the content"""
-        return 'free-surface'
-    
-    @property
-    def key(self) -> str:
-        """str : A UUID4 key assigned to the record"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__key
-
-    @key.setter
-    def key(self, value: str):
-        self.__key = str(value)
-    
-    @property
-    def id(self) -> str:
-        """str : A unique id assigned to the record"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__id
-
-    @id.setter
-    def id(self, value: str):
-        self.__id = str(value)
-
-    @property
-    def family(self) -> str:
-        """str : The prototype/reference id the defect is defined for"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__family
-
-    @family.setter
-    def family(self, value: str):
-        self.__family = str(value)
-
-    @property
-    def parameters(self) -> dict:
-        """dict : Defect parameters for atomman structure generator"""
-        if self.model is None:
-            raise AttributeError('No model information loaded')
-        return self.__parameters
-
-    def load_model(self,
-                   model: Union[str, io.IOBase, DM],
-                   name: Optional[str] = None):
-        """
-        Loads record contents from a given model.
-
-        Parameters
-        ----------
-        model : str or DataModelDict
-            The model contents of the record to load.
-        name : str, optional
-            The name to assign to the record.  Often inferred from other
-            attributes if not given.
-        """
-        super().load_model(model, name=name)
-        content = self.model[self.modelroot]
-
-        self.key = content['key']
-        self.id = content['id']
-        self.family = content['system-family']
-        self.__parameters = dict(content['calculation-parameter'])
-
-    def build_model(self) -> DM:
-        """
-        Returns the object info as data model content
-        
-        Returns
-        ----------
-        DataModelDict
-            The data model content.
-        """
-        model = DM()
-        model[self.modelroot] = content = DM()
-
-        content['key'] = self.key
-        content['id'] = self.id
-        content['system-family'] = self.family
-        content['calculation-parameter'] = DM(self.parameters)
-
-        self._set_model(model)
-        return model
-
-    def metadata(self) -> dict:
-        """
-        Generates a dict of simple metadata values associated with the record.
-        Useful for quickly comparing records and for building pandas.DataFrames
-        for multiple records of the same style.
-        """
-        meta = {}
-        meta['name'] = self.name
-        meta['id'] = self.id
-        meta['family'] = self.family
-        meta['hkl'] = self.parameters['hkl']
-        if 'shiftindex' in self.parameters:
-            meta['shiftindex'] = self.parameters['shiftindex']
-        meta['cutboxvector'] = self.parameters['cutboxvector']
-        
-        return meta
-
-    @property
-    def queries(self) -> dict:
-        """dict: Query objects and their associated parameter names."""
-        return {
-            'key': load_query(
-                style='str_match',
-                name='key', 
-                path=f'{self.modelroot}.key'),
-            'id': load_query(
-                style='str_match',
-                name='id',
-                path=f'{self.modelroot}.id'),
-            'family': load_query(
-                style='str_match',
-                name='family',
-                path=f'{self.modelroot}.system-family'),
-            'hkl': load_query(
-                style='str_match',
-                name='hkl',
-                path=f'{self.modelroot}.calculation-parameter.hkl'),
-            'shiftindex': load_query(
-                style='int_match',
-                name='shiftindex',
-                path=f'{self.modelroot}.calculation-parameter.shiftindex'),
-            'cutboxvector': load_query(
-                style='str_match',
-                name='cutboxvector',
-                path=f'{self.modelroot}.calculation-parameter.cutboxvector'),
-        }
-
-    def pandasfilter(self,
-                     dataframe: pd.DataFrame,
-                     name: Union[str, list, None] = None,
-                     key: Union[str, list, None] = None,
-                     id: Union[str, list, None] = None,
-                     family: Union[str, list, None] = None,
-                     hkl: Union[str, list, None] = None,
-                     shiftindex: Union[int, list, None] = None,
-                     cutboxvector: Union[str, list, None] = None) -> pd.Series:
-        """
-        Filters a pandas.DataFrame based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        dataframe : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        name : str or list
-            The record name(s) to parse by.
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        family : str or list
-            Parent prototype/reference id(s) to parse by.
-        hkl : str or list
-            Space delimited plane(s) to parse by.
-        shiftindex : int or list
-            The shift index indicating the termination plane.
-        cutboxvector : str or list
-            cutboxvector value(s) to parse by.
-        
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-        matches = super().pandasfilter(dataframe, name=name, key=key, id=id,
-                                       family=family, hkl=hkl, shiftindex=shiftindex,
-                                       cutboxvector=cutboxvector)
-        return matches
-
-    def mongoquery(self,
-                   name: Union[str, list, None] = None,
-                   key: Union[str, list, None] = None,
-                   id: Union[str, list, None] = None,
-                   family: Union[str, list, None] = None,
-                   hkl: Union[str, list, None] = None,
-                   shiftindex: Union[int, list, None] = None,
-                   cutboxvector: Union[str, list, None] = None) -> dict:
-        """
-        Builds a Mongo-style query based on kwargs values for the record style.
+    Reads in a LAMMPS atomic dump file into a System.
+    
+    Parameters
+    ----------
+    data : str or file-like object
+        The content, file path or file-like object containing the content to
+        read.
+    symbols : tuple, optional
+        Allows the list of element symbols to be assigned during loading.
+    lammps_units : str
+        The LAMMPS units option associated with the parameters.  Default value
+        is 'metal'.
+    prop_name : list, optional
+         The Atoms properties to generate.
+    table_name : list, optional
+        The table column name(s) that correspond to each prop_name.  If
+        prop_name, table_name and prop_info are not given, prop_name and
+        table_name will be read in from data.
+    shape : list, optional
+        The shape of each per-atom property.  If not given, will be taken from
+        standard LAMMPS parameter names, or left at () for direct 
+        property-table conversion.
+    unit : list, optional
+        Lists the units for each prop_name as stored in the table.  For a
+        value of None, no conversion will be performed for that property.  For
+        a value of 'scaled', the corresponding table values will be taken in
+        box-scaled units.  If not given, all unit values will be set to None
+        (i.e. no conversions).
+    dtype : list, optional
+        Allows for the data type of each property to be explicitly given.
+        Values of None will infer the data type from the corresponding
+        property values.  If not given, all values will be None.
+    prop_info : list of dict, optional
+        Structured form of property conversion parameters, in which each
+        dictionary in the list corresponds to a single atoms property.  Each
+        dictionary must have a 'prop_name' field, and can optionally have
+        'table_name', 'shape', 'unit', and 'dtype' fields.
+    return_prop_info : bool, optional
+        Flag indicating if the full prop_info is to be returned.  Default value
+        is False.
         
-        Parameters
-        ----------
-        name : str or list
-            The record name(s) to parse by.
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        family : str or list
-            Parent prototype/reference id(s) to parse by.
-        hkl : str or list
-            Space delimited plane(s) to parse by.
-        cutboxvector : str or list
-            cutboxvector value(s) to parse by.
+    Returns
+    -------
+    system : atomman.System
+        The generated system.
+    prop_info : list of dict
+        The full prop_info detailing the property-table conversion. Returned
+        if return_prop_info is True.
+    """
+    
+    lammps_unit = style.unit(lammps_units)
+    
+    # Initialize parameter values
+    pbc = None
+    box = None
+    natoms = None
+    atomsstart = None
+    xy = 0.0
+    xz = 0.0
+    yz = 0.0
+    
+    readnatoms = False
+    readtimestep = False
+    bcount = 3
+    
+    # Read str and files in the same way
+    with uber_open_rmode(data) as fp:
         
-        Returns
-        -------
-        dict
-            The Mongo-style query
-        """   
-        mquery = super().mongoquery(name=name, key=key, id=id,
-                                    family=family, hkl=hkl, shiftindex=shiftindex,
-                                    cutboxvector=cutboxvector)
-        return mquery
-
-    def cdcsquery(self,
-                  key: Union[str, list, None] = None,
-                  id: Union[str, list, None] = None,
-                  family: Union[str, list, None] = None,
-                  hkl: Union[str, list, None] = None,
-                  shiftindex: Union[int, list, None] = None,
-                  cutboxvector: Union[str, list, None] = None) -> dict:
-        """
-        Builds a CDCS-style query based on kwargs values for the record style.
+        # Loop over all lines in fp
+        for i, line in enumerate(fp):
+            terms = line.decode('UTF-8').split()
+            
+            # Skip blank lines
+            if len(terms) > 0:
+                
+                # Read number of atoms if time to do so
+                if readnatoms:
+                    natoms = int(terms[0])
+                    readnatoms = False
+                
+                # Read timestep if time to do so
+                elif readtimestep:
+                    #timestep = int(terms[0])
+                    readtimestep = False
+                
+                # Read x boundary condition values if time to do so
+                elif bcount == 0:
+                    xlo = uc.set_in_units(float(terms[0]), lammps_unit['length'])
+                    xhi = uc.set_in_units(float(terms[1]), lammps_unit['length'])
+                    if len(terms) == 3:
+                        xy = uc.set_in_units(float(terms[2]),
+                                             lammps_unit['length'])
+                    bcount += 1
+                
+                # Read y boundary condition values if time to do so
+                elif bcount == 1:
+                    ylo = uc.set_in_units(float(terms[0]), lammps_unit['length'])
+                    yhi = uc.set_in_units(float(terms[1]), lammps_unit['length'])
+                    if len(terms) == 3:
+                        xz = uc.set_in_units(float(terms[2]),
+                                             lammps_unit['length'])
+                    bcount += 1
+                
+                # Read z boundary condition values if time to do so
+                elif bcount == 2:
+                    zlo = uc.set_in_units(float(terms[0]), lammps_unit['length'])
+                    zhi = uc.set_in_units(float(terms[1]), lammps_unit['length'])
+                    if len(terms) == 3:
+                        yz = uc.set_in_units(float(terms[2]),
+                                             lammps_unit['length'])
+                        
+                        # Convert from max, min to hi, lo
+                        xlo = xlo - min((0.0, xy, xz, xy + xz))
+                        xhi = xhi - max((0.0, xy, xz, xy + xz))
+                        ylo = ylo - min((0.0, yz))
+                        yhi = yhi - max((0.0, yz))
+                    bcount += 1
+                
+                # Otherwise, only check lines starting with ITEM
+                elif terms[0] == 'ITEM:':
+                    
+                    # ITEM: TIMESTEP indicates it is time to read the timestep
+                    if terms[1] == 'TIMESTEP':
+                        readtimestep = True
+                    
+                    # ITEM: NUMBER indicates it is time to read natoms
+                    elif terms[1] == 'NUMBER':
+                        readnatoms = True
+                    
+                    # ITEM: BOX gives pbc and indicates it is time to read box parameters
+                    elif terms[1] == 'BOX':
+                        pbc = [True, True, True]
+                        for i in range(3):
+                            if terms[i + len(terms) - 3] != 'pp':
+                                pbc[i] = False
+                        bcount = 0
+                        
+                    # ITEM: ATOMS gives list of property names and indicates it is time to read atomic values
+                    elif terms[1] == 'ATOMS':
+                        
+                        # Read list of property names
+                        name_list = terms[2:]
+                        
+                        # Create default prop_name and table_name if needed
+                        if prop_info is None and prop_name is None:
+                            assert table_name is None, 'table_name cannot be given without prop_name'
+                            prop_name, table_name = matchprops(name_list)
+                            
+                        atomsstart = i + 1
+    
+    # Create system
+    box = Box(xlo=xlo, xhi=xhi,
+              ylo=ylo, yhi=yhi,
+              zlo=zlo, zhi=zhi,
+              xy=xy, xz=xz, yz=yz)
+    atoms = Atoms(natoms=natoms)
+    system = System(box=box, atoms=atoms, pbc=pbc)
+    
+    # Generate prop_info
+    prop_info = process_prop_info(prop_name=prop_name,
+                                  table_name=table_name,
+                                  shape=shape, unit=unit, dtype=dtype,
+                                  prop_info=prop_info,
+                                  lammps_units=lammps_units)
+    
+    # Remove duplicate pos fields
+    firstpos = True
+    short_prop_info = []
+    for pinfo in prop_info:
+        if pinfo['prop_name'] in ['pos', 'spos', 'upos', 'supos']:
+            if firstpos:
+                pinfo['prop_name'] = 'pos'
+            else:
+                continue
+        short_prop_info.append(pinfo)
+    
+    # Read atoms into system
+    system = amload('table', data, box=system.box, symbols=symbols, system=system,
+                  prop_info=short_prop_info, skiprows=atomsstart,
+                  nrows=natoms)
+    
+    if return_prop_info:
+        return system, short_prop_info
+    else:
+        return system
+    
+def matchprops(items):
+    """
+    Takes a list of table_names, pairs them up and matches them to prop_names.
+    
+    Parameters
+    ----------
+    items : list
+        One dimensional list of all table names.
+    
+    Returns
+    -------
+    prop_name : list
+        The list of system property names corresponding to items.
+    table_name : list
+        The list of items paired up and corresponding to the prop_name list.
+    """
+    
+    prop2table = OrderedDict()
+    for item in items:
+        # Search for prop_name match 
+        for sinfo in standard_conversions():
+            match = False
+            table_names = sinfo['table_name']
+            if not isinstance(table_names, list):
+                table_names = [table_names]
+            if item in table_names:
+                match = True
+                break
         
-        Parameters
-        ----------
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        family : str or list
-            Parent prototype/reference id(s) to parse by.
-        hkl : str or list
-            Space delimited plane(s) to parse by.
-        cutboxvector : str or list
-            cutboxvector value(s) to parse by.
+        if match is True:
+            name = sinfo['prop_name']
+        else:
+            name = item
         
-        Returns
-        -------
-        dict
-            The CDCS-style query
-        """
-        mquery = super().cdcsquery(key=key, id=id,
-                                    family=family, hkl=hkl, shiftindex=shiftindex,
-                                    cutboxvector=cutboxvector)
-        return mquery
+        if name not in prop2table:
+            if match is True:
+                for table_name in table_names:
+                    assert table_name in items, 'Incomplete propery ' + str(name)
+            prop2table[name] = []
+        prop2table[name].append(item)
+    
+    prop_name = list(prop2table.keys())
+    table_name = list(prop2table.values())
+    for i in range(len(table_name)):
+        if len(table_name[i]) == 1:
+            table_name[i] = table_name[i][0]
+    
+    return prop_name, table_name
```

### Comparing `atomman-1.4.8/atomman/library/record/PointDefect.py` & `atomman-1.4.9/atomman/library/record/CrystalPrototype.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 # https://github.com/usnistgov/DataModelDict
 from DataModelDict import DataModelDict as DM
 
 # https://github.com/usnistgov/yabadaba
 from yabadaba.record import Record
 from yabadaba import load_query
 
-# https://pandas.pydata.org/
-import pandas as pd
+# atomman imports
+from ... import System
 
-class PointDefect(Record):
+class CrystalPrototype(Record):
     """
-    Class for representing point_defect records, which collect the parameters
-    necessary for atomman to generate a particular point defect.
+    Class for representing crystal_prototype records that describe common
+    crystal prototypes.
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None):
         """
         Initializes a Record object for a given style.
         
@@ -30,251 +30,244 @@
         model : str, file-like object, DataModelDict
             The contents of the record.
         name : str, optional
             The unique name to assign to the record.  If model is a file
             path, then the default record name is the file name without
             extension.
         """
-        if model is not None:
-            super().__init__(model=model, name=name)
-        elif name is not None:
-            self.name = name
+        # Init properties
+        self.__ucell = None
 
+        # Call super init
+        super().__init__(model=model, name=name)
+        
     @property
     def style(self) -> str:
         """str: The record style"""
-        return 'point_defect'
+        return 'crystal_prototype'
+
+    @property
+    def modelroot(self) -> str:
+        """str: The root element of the content"""
+        return 'crystal-prototype'
 
     @property
     def xsd_filename(self) -> Tuple[str, str]:
         """tuple: The module path and file name of the record's xsd schema"""
         return ('atomman.library.xsd', f'{self.style}.xsd')
 
     @property
-    def modelroot(self) -> str:
-        """str: The root element of the content"""
-        return 'point-defect'
-    
+    def xsl_filename(self) -> Tuple[str, str]:
+        """tuple: The module path and file name of the record's xsl transformer"""
+        return ('atomman.library.xsl', f'{self.style}.xsl')
+
+    def load_model(self,
+                   model: Union[str, io.IOBase, DM],
+                   name: Optional[str] = None):
+        """
+        Loads record contents from a given model.
+
+        Parameters
+        ----------
+        model : str or DataModelDict
+            The model contents of the record to load.
+        name : str, optional
+            The name to assign to the record.  Often inferred from other
+            attributes if not given.
+        """
+        super().load_model(model, name=name)
+        proto = self.model[self.modelroot]
+        
+        self.__key = proto['key']
+        self.__id = proto['id']
+        self.__commonname = proto['name']
+        self.__prototype = proto['prototype']
+        self.__pearson = proto['Pearson-symbol']
+        self.__strukturbericht = proto['Strukturbericht']
+        
+        self.__sg_number = proto['space-group']['number']
+        self.__sg_hm = proto['space-group']['Hermann-Maguin']
+        self.__sg_schoenflies = proto['space-group']['Schoenflies']
+        
+        self.__crystalfamily = proto['system-info']['cell']['crystal-family']
+        self.__natypes = proto['system-info']['cell']['natypes']
+        self.__ucell = None
+
+        # Set name as id if no name given
+        try:
+            self.name
+        except AttributeError:
+            self.name = self.id
+
+    @property
+    def id(self) -> str:
+        """str : A unique id assigned to the record"""
+        if self.model is None:
+            raise AttributeError('No model information loaded')
+        return self.__id
+
     @property
     def key(self) -> str:
         """str : A UUID4 key assigned to the record"""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self.__key
 
-    @key.setter
-    def key(self, value: str):
-        self.__key = str(value)
+    @property
+    def commonname(self) -> str:
+        """str : A common name associated with the prototype"""
+        if self.model is None:
+            raise AttributeError('No model information loaded')
+        return self.__commonname
     
     @property
-    def id(self) -> str:
-        """str : A unique id assigned to the record"""
+    def prototype(self) -> str:
+        """str : A prototype composition associated with the prototype"""
         if self.model is None:
             raise AttributeError('No model information loaded')
-        return self.__id
+        return self.__prototype
+    
+    @property
+    def pearson(self) -> str:
+        """str : The prototype's Pearson symbol"""
+        if self.model is None:
+            raise AttributeError('No model information loaded')
+        return self.__pearson
 
-    @id.setter
-    def id(self, value: str):
-        self.__id = str(value)
+    @property
+    def strukturbericht(self) -> str:
+        """str : The prototype's Strukturbericht symbol"""
+        if self.model is None:
+            raise AttributeError('No model information loaded')
+        return self.__strukturbericht
 
     @property
-    def family(self) -> str:
-        """str : The prototype/reference id the defect is defined for"""
+    def sg_number(self) -> int:
+        """int : The prototype's space group number"""
         if self.model is None:
             raise AttributeError('No model information loaded')
-        return self.__family
+        return self.__sg_number
 
-    @family.setter
-    def family(self, value: str):
-        self.__family = str(value)
+    @property
+    def sg_hm(self) -> str:
+        """str : The prototype's space group international symbol"""
+        if self.model is None:
+            raise AttributeError('No model information loaded')
+        return self.__sg_hm
 
     @property
-    def parameters(self) -> list:
-        """list : Defect parameters for atomman structure generator"""
+    def sg_schoenflies(self) -> str:
+        """str : The prototype's space group Schoenflies symbol"""
         if self.model is None:
             raise AttributeError('No model information loaded')
-        return self.__parameters
+        return self.__sg_schoenflies
 
-    def load_model(self,
-                   model: Union[str, io.IOBase, DM],
-                   name: Optional[str] = None):
-        """
-        Loads record contents from a given model.
+    @property
+    def crystalfamily(self) -> str:
+        """str : The prototype's system family"""
+        if self.model is None:
+            raise AttributeError('No model information loaded')
+        return self.__crystalfamily
 
-        Parameters
-        ----------
-        model : str or DataModelDict
-            The model contents of the record to load.
-        name : str, optional
-            The name to assign to the record.  Often inferred from other
-            attributes if not given.
-        """
-        super().load_model(model, name=name)
-        content = self.model[self.modelroot]
+    @property
+    def natypes(self) -> int:
+        """int : Number of atom types"""
+        if self.model is None:
+            raise AttributeError('No model information loaded')
+        return self.__natypes
 
-        self.key = content['key']
-        self.id = content['id']
-        self.family = content['system-family']
-        self.__parameters = []
-        for cp in content.aslist('calculation-parameter'):
-            self.__parameters.append(dict(cp))
+    @property
+    def ucell(self) -> System:
+        """atomman.System : The unit cell for the prototype""" 
+        if self.model is None:
+            raise AttributeError('No model information loaded')
+        if self.__ucell is None:
+            self.__ucell = System(model=self.model)
+        return self.__ucell
 
     def build_model(self) -> DM:
-        """
-        Returns the object info as data model content
-        
-        Returns
-        ----------
-        DataModelDict
-            The data model content.
-        """
-        model = DM()
-        model[self.modelroot] = content = DM()
-
-        content['key'] = self.key
-        content['id'] = self.id
-        content['system-family'] = self.family
-        for cp in self.parameters:
-            content.append('calculation-parameter', DM(cp))
-
-        self._set_model(model)
-        return model
+        if self.model is None:
+            raise AttributeError('No model information loaded')
+        return self.model
 
     def metadata(self) -> dict:
         """
         Generates a dict of simple metadata values associated with the record.
         Useful for quickly comparing records and for building pandas.DataFrames
         for multiple records of the same style.
         """
-        meta = {}
-        meta['name'] = self.name
-        meta['id'] = self.id
-        meta['family'] = self.family
-        
-        meta['ptd_type'] = []
-        meta['pos'] = []
-        meta['atype'] = []
-        meta['db_vect'] = []
-        meta['scale'] = []
-        for cp in self.parameters:
-            meta['ptd_type'].append(cp.get('ptd_type', None))
-            meta['pos'].append(cp.get('pos', None))
-            meta['atype'].append(cp.get('atype', None))
-            meta['db_vect'].append(cp.get('db_vect', None))
-            meta['scale'].append(cp.get('scale', None))
+        params = {}
+        params['name'] = self.name
+        params['key'] = self.key
+        params['id'] = self.id
+        params['commonname'] = self.commonname
+        params['prototype'] = self.prototype
+        params['pearson'] = self.pearson
+        params['strukturbericht'] = self.strukturbericht
+        params['sg_number'] = self.sg_number
+        params['sg_hm'] = self.sg_hm
+        params['sg_schoenflies'] = self.sg_schoenflies
+        params['crystalfamily'] = self.crystalfamily
+        params['natypes'] = self.natypes
         
-        return meta
+        return params
 
     @property
     def queries(self) -> dict:
         """dict: Query objects and their associated parameter names."""
         return {
             'key': load_query(
                 style='str_match',
                 name='key', 
-                path=f'{self.modelroot}.key'),
+                path=f'{self.modelroot}.key',
+                description="search by crystal prototype's UUID key"),
             'id': load_query(
                 style='str_match',
                 name='id',
-                path=f'{self.modelroot}.id'),
-            'family': load_query(
+                path=f'{self.modelroot}.id',
+                description="search by crystal prototype's id"),
+            'commonname': load_query(
+                style='str_match',
+                name='commonname',
+                path=f'{self.modelroot}.name',
+                description="search by crystal prototype's common name"),
+            'prototype': load_query(
+                style='str_match',
+                name='prototype',
+                path=f'{self.modelroot}.prototype',
+                description="search by crystal prototype's prototype composition"),
+            'pearson': load_query(
+                style='str_match',
+                name='pearson',
+                path=f'{self.modelroot}.Pearson-symbol',
+                description="search by crystal prototype's Pearson symbol"),
+            'strukturbericht': load_query(
+                style='str_match',
+                name='strukturbericht',
+                path=f'{self.modelroot}.Strukturbericht',
+                description="search by crystal prototype's Strukturbericht symbol"),
+            'sg_number': load_query(
+                style='int_match',
+                name='sg_number',
+                path=f'{self.modelroot}.space-group.number',
+                description="search by crystal prototype's space group number"),
+            'sg_hm': load_query(
+                style='str_match',
+                name='sg_hm',
+                path=f'{self.modelroot}.space-group.Hermann-Maguin',
+                description="search by crystal prototype's space group Hermann-Maguin symbol"),
+            'sg_schoenflies': load_query(
                 style='str_match',
-                name='family',
-                path=f'{self.modelroot}.system-family'),
-            'ptd_type': load_query(
-                style='list_contains',
-                name='ptd_type',
-                path=f'{self.modelroot}.calculation-parameter.ptd_type'),
+                name='sg_schoenflies',
+                path=f'{self.modelroot}.space-group.Schoenflies',
+                description="search by crystal prototype's space group Schoenflies symbol"),
+            'crystalfamily': load_query(
+                style='str_match',
+                name='crystalfamily',
+                path=f'{self.modelroot}.system-info.cell.crystal-family',
+                description="search by crystal prototype's crystal family"),
+            'natypes': load_query(
+                style='int_match',
+                name='natypes',
+                path=f'{self.modelroot}.system-info.cell.natypes',
+                description="search by number of atom types in the crystal prototype"),
         }
-
-    def pandasfilter(self,
-                     dataframe: pd.DataFrame,
-                     name: Union[str, list, None] = None,
-                     key: Union[str, list, None] = None,
-                     id: Union[str, list, None] = None,
-                     family: Union[str, list, None] = None,
-                     ptd_type: Union[str, list, None] = None) -> pd.Series:
-        """
-        Filters a pandas.DataFrame based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        dataframe : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        name : str or list
-            The record name(s) to parse by.
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        family : str or list
-            Parent prototype/reference id(s) to parse by.
-        ptd_type : str or list
-            Point defect type(s) to parse by.
-        
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-        matches = super().pandasfilter(dataframe, name=name, key=key, id=id,
-                                       family=family, ptd_type=ptd_type)
-        return matches
-
-    def mongoquery(self,
-                   name: Union[str, list, None] = None,
-                   key: Union[str, list, None] = None,
-                   id: Union[str, list, None] = None,
-                   family: Union[str, list, None] = None,
-                   ptd_type: Union[str, list, None] = None) -> dict:
-        """
-        Builds a Mongo-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        name : str or list
-            The record name(s) to parse by.
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        family : str or list
-            Parent prototype/reference id(s) to parse by.
-        ptd_type : str or list
-            Point defect type(s) to parse by.
-        
-        Returns
-        -------
-        dict
-            The Mongo-style query
-        """   
-        mquery = super().mongoquery(name=name, key=key, id=id,
-                                    family=family, ptd_type=ptd_type)
-        return mquery
-
-    def cdcsquery(self,
-                  key: Union[str, list, None] = None,
-                  id: Union[str, list, None] = None,
-                  family: Union[str, list, None] = None,
-                  ptd_type: Union[str, list, None] = None) -> dict:
-        """
-        Builds a CDCS-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        id : str or list
-            The record id(s) to parse by.
-        key : str or list
-            The record key(s) to parse by.
-        family : str or list
-            Parent prototype/reference id(s) to parse by.
-        ptd_type : str or list
-            Point defect type(s) to parse by.
-        
-        Returns
-        -------
-        dict
-            The CDCS-style query
-        """
-        mquery = super().cdcsquery(key=key, id=id,
-                                    family=family, ptd_type=ptd_type)
-        return mquery
```

### Comparing `atomman-1.4.8/atomman/library/record/__init__.py` & `atomman-1.4.9/atomman/library/record/__init__.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/__init__.py` & `atomman-1.4.9/atomman/load/__init__.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/ase_Atoms/load.py` & `atomman-1.4.9/atomman/load/ase_Atoms/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/atom_data/atoms_prop_info.py` & `atomman-1.4.9/atomman/load/atom_data/atoms_prop_info.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/atom_data/load.py` & `atomman-1.4.9/atomman/load/atom_data/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/atom_data/velocities_prop_info.py` & `atomman-1.4.9/atomman/load/atom_data/velocities_prop_info.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/atom_dump/process_prop_info.py` & `atomman-1.4.9/atomman/load/atom_dump/process_prop_info.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/cif/load.py` & `atomman-1.4.9/atomman/load/cif/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/crystal/load.py` & `atomman-1.4.9/atomman/load/crystal/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/dft_reference/load.py` & `atomman-1.4.9/atomman/load/dft_reference/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/phonopy_Atoms/load.py` & `atomman-1.4.9/atomman/load/phonopy_Atoms/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/poscar/load.py` & `atomman-1.4.9/atomman/load/poscar/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/prototype/load.py` & `atomman-1.4.9/atomman/load/prototype/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/pymatgen_Structure/load.py` & `atomman-1.4.9/atomman/load/pymatgen_Structure/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/spglib_cell/load.py` & `atomman-1.4.9/atomman/load/spglib_cell/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/system_model/load.py` & `atomman-1.4.9/atomman/load/system_model/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/table/load.py` & `atomman-1.4.9/atomman/load/table/load.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/load/table/process_prop_info.py` & `atomman-1.4.9/atomman/load/table/process_prop_info.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/mep/BasePath.py` & `atomman-1.4.9/atomman/mep/BasePath.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/mep/ISMPath.py` & `atomman-1.4.9/atomman/mep/ISMPath.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/mep/__init__.py` & `atomman-1.4.9/atomman/mep/__init__.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/mep/gradient/central_difference.py` & `atomman-1.4.9/atomman/mep/gradient/central_difference.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/mep/integrator/euler.py` & `atomman-1.4.9/atomman/mep/integrator/euler.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/mep/integrator/rungekutta.py` & `atomman-1.4.9/atomman/mep/integrator/rungekutta.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/plot/interpolate_contour.py` & `atomman-1.4.9/atomman/plot/interpolate_contour.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/region/Cylinder.py` & `atomman-1.4.9/atomman/region/Cylinder.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/region/Plane.py` & `atomman-1.4.9/atomman/region/Plane.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/region/PlaneSet.py` & `atomman-1.4.9/atomman/region/PlaneSet.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/region/Shape.py` & `atomman-1.4.9/atomman/region/Shape.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/region/Sphere.py` & `atomman-1.4.9/atomman/region/Sphere.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/thermo/EinsteinSolid.py` & `atomman-1.4.9/atomman/thermo/EinsteinSolid.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/thermo/IdealGas.py` & `atomman-1.4.9/atomman/thermo/IdealGas.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/thermo/UhlenbeckFordModel.py` & `atomman-1.4.9/atomman/thermo/UhlenbeckFordModel.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/tools/__init__.py` & `atomman-1.4.9/atomman/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/tools/axes_check.py` & `atomman-1.4.9/atomman/tools/axes_check.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/tools/boolean.py` & `atomman-1.4.9/atomman/tools/boolean.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/tools/compositionstr.py` & `atomman-1.4.9/atomman/tools/compositionstr.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/tools/crystalsystem.py` & `atomman-1.4.9/atomman/tools/crystalsystem.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/tools/duplicates_allclose.py` & `atomman-1.4.9/atomman/tools/duplicates_allclose.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/tools/filltemplate.py` & `atomman-1.4.9/atomman/tools/filltemplate.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/tools/indexstr.py` & `atomman-1.4.9/atomman/tools/indexstr.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/tools/miller.py` & `atomman-1.4.9/atomman/tools/miller.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/tools/vect_angle.py` & `atomman-1.4.9/atomman/tools/vect_angle.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman/unitconvert.py` & `atomman-1.4.9/atomman/unitconvert.py`

 * *Files identical despite different names*

### Comparing `atomman-1.4.8/atomman.egg-info/PKG-INFO` & `atomman-1.4.9/atomman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomman
-Version: 1.4.8
+Version: 1.4.9
 Summary: Atomistic Manipulation Toolkit
 Home-page: https://github.com/usnistgov/atomman/
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: atom,atomic,atomistic,molecular dynamics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `atomman-1.4.8/atomman.egg-info/SOURCES.txt` & `atomman-1.4.9/atomman.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -187,8 +187,10 @@
 atomman/tools/boolean.py
 atomman/tools/compositionstr.py
 atomman/tools/crystalsystem.py
 atomman/tools/duplicates_allclose.py
 atomman/tools/filltemplate.py
 atomman/tools/indexstr.py
 atomman/tools/miller.py
-atomman/tools/vect_angle.py
+atomman/tools/vect_angle.py
+tests/test_root.py
+tests/test_unitconvert.py
```

### Comparing `atomman-1.4.8/setup.py` & `atomman-1.4.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,12 +62,12 @@
         'numpy>=1.15',
         'matplotlib',
         'scipy',
         'pandas',
         'cython',
         'requests',
         'toolz',
-        'potentials==0.3.5'
+        'potentials==0.3.6'
     ],
     include_package_data = True,
     zip_safe = False
 )
```

