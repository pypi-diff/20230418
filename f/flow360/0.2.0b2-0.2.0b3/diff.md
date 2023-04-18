# Comparing `tmp/flow360-0.2.0b2.tar.gz` & `tmp/flow360-0.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-0.2.0b2.tar", max compression
+gzip compressed data, was "flow360-0.2.0b3.tar", max compression
```

## Comparing `flow360-0.2.0b2.tar` & `flow360-0.2.0b3.tar`

### file list

```diff
@@ -1,57 +1,59 @@
--rw-r--r--   0        0        0    26526 2023-04-13 03:45:55.319405 flow360-0.2.0b2/LICENSE
--rw-r--r--   0        0        0     1473 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/__init__.py
--rw-r--r--   0        0        0       53 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/cli/__init__.py
--rw-r--r--   0        0        0     1126 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/cli/app.py
--rw-r--r--   0        0        0        0 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     2869 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     1466 2023-04-13 03:45:55.319405 flow360-0.2.0b2/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0     8842 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      687 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/cloud/security.py
--rw-r--r--   0        0        0        0 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/__init__.py
--rw-r--r--   0        0        0    22372 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/case.py
--rw-r--r--   0        0        0      142 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/constants.py
--rw-r--r--   0        0        0    32080 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/flow360_params.py
--rw-r--r--   0        0        0      220 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/meshing/__init__.py
--rw-r--r--   0        0        0     6145 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/meshing/params.py
--rw-r--r--   0        0        0    18009 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/params_base.py
--rw-r--r--   0        0        0     7550 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/resource_base.py
--rw-r--r--   0        0        0    10105 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0     2326 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/types.py
--rw-r--r--   0        0        0     1019 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/utils.py
--rw-r--r--   0        0        0     2940 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/validator.py
--rw-r--r--   0        0        0    21661 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     2137 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/environment.py
--rw-r--r--   0        0        0      237 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/__init__.py
--rw-r--r--   0        0        0     4024 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/actuatorDisk/flow360.json
--rw-r--r--   0        0        0      447 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/actuator_disk.py
--rw-r--r--   0        0        0    24017 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/airplane/geometry.csm
--rw-r--r--   0        0        0      675 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/airplane/surface_params.json
--rw-r--r--   0        0        0     3702 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/airplane/volume_params.json
--rw-r--r--   0        0        0      292 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/airplane.py
--rw-r--r--   0        0        0     5515 2023-04-13 03:45:55.323405 flow360-0.2.0b2/flow360/examples/base_test_case.py
--rw-r--r--   0        0        0  1157943 2023-04-13 03:45:55.327405 flow360-0.2.0b2/flow360/examples/betDisk/flow360.json
--rw-r--r--   0        0        0  1158028 2023-04-13 03:45:55.331405 flow360-0.2.0b2/flow360/examples/betLine/flow360.json
--rw-r--r--   0        0        0  1158029 2023-04-13 03:45:55.331405 flow360-0.2.0b2/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      432 2023-04-13 03:45:55.331405 flow360-0.2.0b2/flow360/examples/bet_disk.py
--rw-r--r--   0        0        0      432 2023-04-13 03:45:55.331405 flow360-0.2.0b2/flow360/examples/bet_line.py
--rw-r--r--   0        0        0     1430 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/cylinder/flow360.json
--rw-r--r--   0        0        0     1492 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0      373 2023-04-13 03:45:55.331405 flow360-0.2.0b2/flow360/examples/cylinder.py
--rw-r--r--   0        0        0       63 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/om6wing/Flow360Mesh.json
--rw-r--r--   0        0        0     1500 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/om6wing/case.yaml
--rw-r--r--   0        0        0     2509 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/om6wing/flow360.json
--rw-r--r--   0        0        0     2305 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      391 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/om6wing.py
--rw-r--r--   0        0        0     2744 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/flow360.json
--rw-r--r--   0        0        0      913 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/flow360mesh.json
--rw-r--r--   0        0        0     3379 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
--rw-r--r--   0        0        0     3376 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
--rw-r--r--   0        0        0      347 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/examples/rotating_spheres.py
--rw-r--r--   0        0        0     1354 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/exceptions.py
--rw-r--r--   0        0        0     5810 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/log.py
--rw-r--r--   0        0        0     1146 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/solver_version.py
--rw-r--r--   0        0        0       38 2023-04-13 03:45:55.335405 flow360-0.2.0b2/flow360/version.py
--rw-r--r--   0        0        0     1480 2023-04-13 03:46:12.223660 flow360-0.2.0b2/pyproject.toml
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 flow360-0.2.0b2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-04-18 16:43:34.940230 flow360-0.2.0b3/LICENSE
+-rw-r--r--   0        0        0     1427 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     1126 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cli/app.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     2897 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     1466 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0     8847 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      687 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cloud/security.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/__init__.py
+-rw-r--r--   0        0        0    23078 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/case.py
+-rw-r--r--   0        0        0      142 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/constants.py
+-rw-r--r--   0        0        0    25502 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/flow360_params/flow360_params.py
+-rw-r--r--   0        0        0    18013 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/flow360_params/params_base.py
+-rw-r--r--   0        0        0     7651 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/flow360_params/solvers.py
+-rw-r--r--   0        0        0      220 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     6160 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0     8159 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/resource_base.py
+-rw-r--r--   0        0        0    10172 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2327 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/types.py
+-rw-r--r--   0        0        0     1019 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/utils.py
+-rw-r--r--   0        0        0     2955 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/validator.py
+-rw-r--r--   0        0        0    21592 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     2137 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/environment.py
+-rw-r--r--   0        0        0      237 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     4024 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      447 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      292 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5406 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157943 2023-04-18 16:43:34.948230 flow360-0.2.0b3/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1158028 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1158029 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      432 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      432 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0     1430 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      373 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0       63 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0     1500 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     2509 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0      427 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
+-rw-r--r--   0        0        0     2305 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      391 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0     2744 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      347 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     1354 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/exceptions.py
+-rw-r--r--   0        0        0     5809 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/log.py
+-rw-r--r--   0        0        0     1146 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/solver_version.py
+-rw-r--r--   0        0        0       38 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/version.py
+-rw-r--r--   0        0        0     1465 2023-04-18 16:43:57.257523 flow360-0.2.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b3/PKG-INFO
```

### Comparing `flow360-0.2.0b2/LICENSE` & `flow360-0.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/__init__.py` & `flow360-0.2.0b3/flow360/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,49 @@
 """
 This module is flow360.
 """
 from .cli import flow360
-from .environment import Env
-from .version import __version__
-
-from .component.surface_mesh import SurfaceMesh
-from .component.surface_mesh import SurfaceMeshList as MySurfaceMeshes
-from .component.volume_mesh import VolumeMesh
-from .component.volume_mesh import VolumeMeshList as MyVolumeMeshes
+from .cloud.s3_utils import ProgressCallbackInterface
+from .component import meshing
 from .component.case import Case
 from .component.case import CaseList as MyCases
-from .component import flow360_params
-
-from .component.meshing.params import SurfaceMeshingParams, VolumeMeshingParams
-from .component import meshing
-
-from .component.flow360_params import (
+from .component.flow360_params import solvers
+from .component.flow360_params.flow360_params import (
+    Boundaries,
     Flow360MeshParams,
-    MeshBoundary,
     Flow360Params,
-    Boundaries,
-    Geometry,
     Freestream,
-    TimeStepping,
-    TimeSteppingCFL,
-    TurbulenceModelSolver,
+    FreestreamBoundary,
+    Geometry,
+    IsothermalWall,
+    MassInflow,
+    MassOutflow,
+    MeshBoundary,
     NavierStokesSolver,
-    SlidingInterface,
-)
-
-from .component.flow360_params import (
     NoSlipWall,
+    SlidingInterface,
+    SlidingInterfaceBoundary,
     SlipWall,
-    FreestreamBoundary,
-    IsothermalWall,
-    SubsonicOutflowPressure,
-    SubsonicOutflowMach,
     SubsonicInflow,
-    SlidingInterfaceBoundary,
+    SubsonicOutflowMach,
+    SubsonicOutflowPressure,
+    TimeStepping,
+    TimeSteppingCFL,
+    TurbulenceModelSolver,
     WallFunction,
-    MassInflow,
-    MassOutflow,
 )
-
-
-from .cloud.s3_utils import ProgressCallbackInterface
+from .component.meshing.params import SurfaceMeshingParams, VolumeMeshingParams
+from .component.surface_mesh import SurfaceMesh
+from .component.surface_mesh import SurfaceMeshList as MySurfaceMeshes
+from .component.volume_mesh import VolumeMesh
+from .component.volume_mesh import VolumeMeshList as MyVolumeMeshes
+from .environment import Env
+from .version import __version__
 
 
 # pylint: disable=too-few-public-methods,invalid-name
 class turbulence:
     """turbulece models shortcut: eg. flow360.turbulence.SA"""
 
-    SA = flow360_params.TurbulenceModelModelType.SA
-    SST = flow360_params.TurbulenceModelModelType.SST
-    NONE = flow360_params.TurbulenceModelModelType.NONE
+    SA = solvers.TurbulenceModelModelType.SA
+    SST = solvers.TurbulenceModelModelType.SST
+    NONE = solvers.TurbulenceModelModelType.NONE
```

### Comparing `flow360-0.2.0b2/flow360/cli/app.py` & `flow360-0.2.0b3/flow360/cli/app.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/cloud/http_util.py` & `flow360-0.2.0b3/flow360/cloud/http_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 http.get(path)
 """
 from functools import wraps
 
 import requests
 
 from ..environment import Env
-from ..version import __version__
-from ..exceptions import AuthorisationError, WebNotFoundError, WebError
+from ..exceptions import AuthorisationError, WebError, WebNotFoundError
 from ..log import log
-
+from ..version import __version__
 from .security import api_key
 
 
 def api_key_auth(request):
     """
     Set the authentication.
     :param request:
     :return:
     """
     key = api_key(Env.current.apikey_profile)
     if not key:
-        raise ValueError("API key not found, please set it by commandline: flow360 configure.")
+        raise AuthorisationError(
+            "API key not found, please set it by commandline: flow360 configure."
+        )
     request.headers["simcloud-api-key"] = key
     request.headers["flow360-python-version"] = __version__
     return request
 
 
 def http_interceptor(func):
     """
@@ -53,15 +54,15 @@
         if resp.status_code == 404:
             raise WebNotFoundError(f"Web {args[1]}: Not found error: {resp.json()}")
 
         if resp.status_code == 200:
             result = resp.json()
             return result.get("data")
 
-        raise Exception(f"Web {args[1]}: Unexpected response error: {resp.status_code}")
+        raise WebError(f"Web {args[1]}: Unexpected response error: {resp.status_code}")
 
     return wrapper
 
 
 class Http:
     """
     Http util class.
```

### Comparing `flow360-0.2.0b2/flow360/cloud/rest_api.py` & `flow360-0.2.0b3/flow360/cloud/rest_api.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/cloud/s3_utils.py` & `flow360-0.2.0b3/flow360/cloud/s3_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 s3 util file for material uploading and downloading.
 """
 import os
 import urllib
+from abc import ABC, abstractmethod
 from datetime import datetime
 from enum import Enum
-from abc import ABC, abstractmethod
 
 import boto3
 from boto3.s3.transfer import TransferConfig
 
 # pylint: disable=unused-import
 from botocore.exceptions import ClientError as CloudFileNotFoundError
 from pydantic import BaseModel, Field
@@ -19,14 +19,15 @@
     Progress,
     TextColumn,
     TimeRemainingColumn,
     TransferSpeedColumn,
 )
 
 from ..environment import Env
+from ..log import log
 from .http_util import http
 
 
 class ProgressCallbackInterface(ABC):
     """
     Progress callback abstract class
     """
@@ -183,16 +184,15 @@
         Upload a file to s3.
         :param resource_id:
         :param remote_file_name:
         :param file_name:
         :return:
         """
         if not os.path.exists(file_name):
-            print(f"file {file_name} does not Exist!")
-            raise FileNotFoundError()
+            raise FileNotFoundError(f"file {file_name} does not Exist!")
 
         token = self._get_s3_sts_token(resource_id, remote_file_name)
         client = token.get_client()
         if progress_callback:
             progress_callback.total = float(os.path.getsize(file_name))
             client.upload_file(
                 Bucket=token.get_bucket(),
@@ -238,15 +238,15 @@
         in the same folder as the file on cloud. Only works when to_file is a folder name.
         :param overwrite: if True overwrite if file exists, otherwise don't download
         :param progress_callback: provide custom callback for progress
         :return:
         """
         to_file = create_base_folder(resource_id, remote_file_name, to_file, keep_folder)
         if os.path.exists(to_file) and not overwrite:
-            print(f"Skipping {remote_file_name}, file exists.")
+            log.info(f"Skipping {remote_file_name}, file exists.")
             return
         token = self._get_s3_sts_token(resource_id, remote_file_name)
         client = token.get_client()
         meta_data = client.head_object(Bucket=token.get_bucket(), Key=token.get_s3_key())
         if progress_callback:
             progress_callback.total = meta_data.get("ContentLength", 0)
             client.download_file(
```

### Comparing `flow360-0.2.0b2/flow360/cloud/security.py` & `flow360-0.2.0b3/flow360/cloud/security.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/component/case.py` & `flow360-0.2.0b3/flow360/component/case.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 Case component
 """
 from __future__ import annotations
+
 import json
 from enum import Enum
 from typing import Iterator, List
+
 from pydantic import Field
 from pylab import show, subplots
 
-from ..cloud.s3_utils import S3TransferType, CloudFileNotFoundError
 from ..cloud.rest_api import RestApi
+from ..cloud.s3_utils import CloudFileNotFoundError, S3TransferType
+from ..log import log
+from .flow360_params.flow360_params import Flow360Params
 from .resource_base import (
-    Flow360ResourceBaseModel,
     Flow360Resource,
+    Flow360ResourceBaseModel,
     Flow360ResourceListBase,
     ResourceDraft,
     before_submit_only,
     is_object_cloud_resource,
 )
-from .flow360_params import Flow360Params
 from .utils import is_valid_uuid
 from .validator import Validator
 
 
 class CaseBase:
     """
     Case Base component
@@ -53,20 +56,20 @@
         :param params:
         :param tags:
         :return:
         """
 
         name = name or self.name or self.info.name
         params = params or self.params.copy(deep=True)
-        new_case = Case.new(name, params, other_case=self, tags=tags)
+        new_case = Case.create(name, params, other_case=self, tags=tags)
         return new_case
 
     def continuation(
         self, name: str = None, params: Flow360Params = None, tags: List[str] = None
-    ) -> Case:
+    ) -> CaseDraft:
         """
         Alias for fork a case to continue simulation
         :param name:
         :param params:
         :param tags:
         :return:
         """
@@ -83,15 +86,15 @@
         :param params:
         :param tags:
         :return:
         """
 
         name = name or self.name or self.info.name
         params = params or self.params.copy(deep=True)
-        return Case.new(name, params, parent_case=self, tags=tags)
+        return Case.create(name, params, parent_case=self, tags=tags)
 
 
 class CaseMeta(Flow360ResourceBaseModel):
     """
     CaseMeta data component
     """
 
@@ -108,21 +111,39 @@
 
 # pylint: disable=too-many-instance-attributes
 class CaseDraft(CaseBase, ResourceDraft):
     """
     Case Draft component (before submission)
     """
 
-    def __init__(self):
-        self.other_case = None
-        self.parent_case = None
-        self.parent_id = None
-        self.tags = None
+    # pylint: disable=too-many-arguments
+    def __init__(
+        self,
+        name: str,
+        params: Flow360Params,
+        volume_mesh_id: str = None,
+        tags: List[str] = None,
+        parent_id=None,
+        other_case: Case = None,
+        parent_case: Case = None,
+        solver_version: str = None,
+    ):
+        self.name = name
+        self.params = params
+        self.volume_mesh_id = volume_mesh_id
+        self.parent_case = parent_case
+        self.parent_id = parent_id
+        self.other_case = other_case
+        self.tags = tags
+        self.solver_version = solver_version
         self._id = None
         self._submitted_case = None
+        ResourceDraft.__init__(self)
+
+        self.validate_case_inputs()
 
     def __str__(self):
         return self.params.__str__()
 
     @property
     def params(self) -> Flow360Params:
         """
@@ -195,22 +216,27 @@
 
         volume_mesh_id = volume_mesh_id or self.other_case.volume_mesh_id
 
         is_valid_uuid(volume_mesh_id)
         is_valid_uuid(parent_id, ignore_none=True)
         self.validator_api(self.params, volume_mesh_id=volume_mesh_id)
 
+        data = {
+            "name": self.name,
+            "meshId": volume_mesh_id,
+            "runtimeParams": self.params.to_flow360_json(),
+            "tags": self.tags,
+            "parentId": parent_id,
+        }
+
+        if self.solver_version:
+            data["solverVersion"] = self.solver_version
+
         resp = RestApi(self._endpoint).post(
-            json={
-                "name": self.name,
-                "meshId": volume_mesh_id,
-                "runtimeParams": self.params.to_flow360_json(),
-                "tags": self.tags,
-                "parentId": parent_id,
-            },
+            json=data,
             path=f"volumemeshes/{volume_mesh_id}/case",
         )
         info = CaseMeta(**resp)
         self._id = info.id
 
         self._submitted_case = Case(self.id)
         return self._submitted_case
@@ -308,25 +334,25 @@
     @property
     def results(self) -> CaseResults:
         """
         returns results object to managing case results
         """
         return self._results
 
-    def download_log(self, log, to_file=".", keep_folder: bool = True):
+    def download_log(self, log_file, to_file=".", keep_folder: bool = True):
         """
         Download log
-        :param log:
+        :param log_file:
         :param to_file: file name on local disk, could be either folder or file name.
         :param keep_folder: If true, the downloaded file will be put in the same folder as the file on cloud. Only work
         when file_name is a folder name.
         :return:
         """
 
-        self.download_file(f"logs/{log.value}", to_file, keep_folder)
+        self.download_file(f"logs/{log_file.value}", to_file, keep_folder)
 
     def is_steady(self):
         """
         returns True when case is steady state
         """
         return self.params.time_stepping.time_step_size == "inf"
 
@@ -373,23 +399,24 @@
         """
         get case from cloud
         """
         return cls(case_id)
 
     # pylint: disable=too-many-arguments
     @classmethod
-    def new(
+    def create(
         cls,
         name: str,
         params: Flow360Params,
         volume_mesh_id: str = None,
         tags: List[str] = None,
         parent_id=None,
         other_case: Case = None,
         parent_case: Case = None,
+        solver_version: str = None,
     ) -> CaseDraft:
         """
         Create new case
         :param name:
         :param params:
         :param volume_mesh_id:
         :param other_case:
@@ -402,25 +429,24 @@
         assert name
         assert volume_mesh_id or other_case or parent_id or parent_case
         assert params
 
         if not isinstance(params, Flow360Params):
             raise ValueError("params are not of type Flow360Params.")
 
-        new_case = CaseDraft()
-        new_case.name = name
-        new_case.volume_mesh_id = volume_mesh_id
-        new_case.other_case = other_case
-        new_case.params = params.copy(deep=True)
-        new_case.tags = tags
-        new_case.parent_id = parent_id
-        new_case.parent_case = parent_case
-
-        new_case.validate_case_inputs()
-
+        new_case = CaseDraft(
+            name=name,
+            volume_mesh_id=volume_mesh_id,
+            params=params.copy(),
+            parent_id=parent_id,
+            other_case=other_case,
+            parent_case=parent_case,
+            tags=tags,
+            solver_version=solver_version,
+        )
         return new_case
 
 
 class CaseResultType(Enum):
     """
     Case results types
     """
@@ -721,28 +747,28 @@
 
         if bet_forces or all:
             try:
                 self.download_file(CaseDownloadable.BET_FORCES, overwrite=overwrite)
             except CloudFileNotFoundError as err:
                 if not self._case.has_bet_disks():
                     if bet_forces:
-                        print("Case does not have any BET disks.")
+                        log.warning("Case does not have any BET disks.")
                 else:
-                    print("A problem occured when trying to download bet disk forces.")
+                    log.error("A problem occured when trying to download bet disk forces.")
                     raise err
 
         if actuator_disk_output or all:
             try:
                 self.download_file(CaseDownloadable.ACTUATOR_DISK_OUTPUT, overwrite=overwrite)
             except CloudFileNotFoundError as err:
                 if not self._case.has_actuator_disks():
                     if actuator_disk_output:
-                        print("Case does not have any actuator disks.")
+                        log.warning("Case does not have any actuator disks.")
                 else:
-                    print("A problem occured when trying to download actuator disk results")
+                    log.error("A problem occured when trying to download actuator disk results")
                     raise err
 
 
 class CaseList(Flow360ResourceListBase):
     """
     Case List component
     """
```

### Comparing `flow360-0.2.0b2/flow360/component/flow360_params.py` & `flow360-0.2.0b3/flow360/component/flow360_params/flow360_params.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """
 Flow360 solver parameters
 """
 from __future__ import annotations
-from typing import Dict, List, Optional, Union
-from enum import Enum
+
 import math
 from abc import ABC
-from typing_extensions import Literal
+from typing import Dict, List, Optional, Union
+
 import pydantic as pd
+from typing_extensions import Literal
 
-from .types import (
+from ...exceptions import ConfigError, Flow360NotImplementedError, ValidationError
+from ..constants import constants
+from ..types import (
     Axis,
+    BoundaryVelocityType,
     Coordinate,
-    PositiveFloat,
     MomentLengthType,
-    BoundaryVelocityType,
-    PositiveInt,
-    NonNegativeInt,
     Omega,
-    Velocity,
+    PositiveFloat,
+    PositiveInt,
     TimeStep,
+    Velocity,
 )
+from ..utils import _get_value_or_none, beta_feature
 from .params_base import Flow360BaseModel, Flow360SortableBaseModel, export_to_flow360
-from .utils import beta_feature, _get_value_or_none
-from .constants import constants
-from ..exceptions import ValidationError, ConfigError, Flow360NotImplementedError
+from .solvers import NavierStokesSolver, TurbulenceModelSolver
 
 
 # pylint: disable=invalid-name
 def get_time_non_dim_unit(mesh_unit_length, C_inf, extra_msg=""):
     """
     returns time non-dimensionalisation
     """
@@ -436,21 +437,41 @@
 
 # pylint: disable=E0213
 class TimeStepping(Flow360BaseModel):
     """
     Time stepping component
     """
 
-    physical_steps: Optional[int] = pd.Field(alias="physicalSteps")
-    max_pseudo_steps: Optional[int] = pd.Field(alias="maxPseudoSteps")
+    physical_steps: Optional[PositiveInt] = pd.Field(alias="physicalSteps")
+    max_pseudo_steps: Optional[PositiveInt] = pd.Field(alias="maxPseudoSteps")
     time_step_size: Optional[
         Union[pd.confloat(gt=0, allow_inf_nan=False), TimeStep, Literal["inf"]]
     ] = pd.Field(alias="timeStepSize", default="inf")
     CFL: Optional[TimeSteppingCFL] = pd.Field()
 
+    # pylint: disable=no-self-argument
+    @pd.root_validator(pre=True)
+    def handle_max_physical_steps(cls, values):
+        """
+        root validator to handle maxPhysicalSteps (deprecated) alias for physical_steps
+        """
+
+        max_physical_steps = values.get("maxPhysicalSteps", None)
+        physical_steps = values.get("physicalSteps", values.get("physical_steps", None))
+
+        if max_physical_steps is not None:
+            if physical_steps is not None:
+                allowed = ["maxPhysicalSteps", "physicalSteps"]
+                raise ValidationError(f"Only one of {allowed} can be used.")
+
+            values["physical_steps"] = max_physical_steps
+            values.pop("maxPhysicalSteps")
+
+        return values
+
     @classmethod
     def default_steady(cls):
         """
         returns default steady settings
         """
         return cls(
             physical_steps=1,
@@ -695,204 +716,14 @@
 
     # pylint: disable=missing-class-docstring,too-few-public-methods
     class Config(Flow360BaseModel.Config):
         exclude_on_flow360_export = {"speed", "density"}
         require_one_of = ["Mach", "speed"]
 
 
-class GenericSolverSettings(Flow360BaseModel):
-    """:class:`GenericSolverSettings` class"""
-
-    absolute_tolerance: Optional[PositiveFloat] = pd.Field(alias="absoluteTolerance")
-    relative_tolerance: Optional[float] = pd.Field(alias="relativeTolerance")
-    linear_iterations: Optional[PositiveInt] = pd.Field(alias="linearIterations")
-    update_jacobian_frequency: Optional[PositiveInt] = pd.Field(alias="updateJacobianFrequency")
-    equation_eval_frequency: Optional[PositiveInt] = pd.Field(alias="equationEvalFrequency")
-    max_force_jac_update_physical_steps: Optional[NonNegativeInt] = pd.Field(
-        alias="maxForceJacUpdatePhysicalSteps"
-    )
-    order_of_accuracy: Optional[Literal[1, 2]] = pd.Field(alias="orderOfAccuracy")
-    kappaMUSCL: Optional[pd.confloat(ge=-1, le=1)] = pd.Field()
-
-
-class NavierStokesSolver(GenericSolverSettings):
-    """:class:`NavierStokesSolver` class for setting up Navier-Stokes solver
-
-    Parameters
-    ----------
-
-    absoluteTolerance :
-        Tolerance for the NS residual, below which the solver goes to the next physical step
-
-    relativeTolerance :
-        Tolerance to the relative residual, below which the solver goes to the next physical step. Relative residual is
-        defined as the ratio of the current pseudoStep’s residual to the maximum residual present in the first
-        10 pseudoSteps within the current physicalStep. NOTE: relativeTolerance is ignored in steady simulations and
-        only absoluteTolerance is used as the convergence criterion
-
-    CFLMultiplier :
-        Factor to the CFL definitions defined in “timeStepping” section
-
-    kappaMUSCL :
-        Kappa for the MUSCL scheme, range from [-1, 1], with 1 being unstable. The default value of -1 leads to a 2nd
-        order upwind scheme and is the most stable. A value of 0.33 leads to a blended upwind/central scheme and is
-        recommended for low subsonic flows leading to reduced dissipation
-
-    linearIterations :
-        Number of linear solver iterations
-
-    updateJacobianFrequency :
-        Frequency at which the jacobian is updated.
-
-    equationEvalFrequency :
-        Frequency at which to update the NS equation in loosely-coupled simulations
-
-    maxForceJacUpdatePhysicalSteps :
-        When which physical steps, the jacobian matrix is updated every pseudo step
-
-    orderOfAccuracy :
-        Order of accuracy in space
-
-    limitVelocity :
-        Limiter for velocity
-
-    limitPressureDensity :
-        Limiter for pressure and density
-
-
-    Returns
-    -------
-    :class:`NavierStokesSolver`
-        An instance of the component class NavierStokesSolver.
-
-    Example
-    -------
-    >>> ns = NavierStokesSolver(absolute_tolerance=1e-10)
-    """
-
-    CFL_multiplier: Optional[PositiveFloat] = pd.Field(alias="CFLMultiplier")
-    limit_velocity: Optional[bool] = pd.Field(alias="limitVelocity")
-    limit_pressure_density: Optional[bool] = pd.Field(alias="limitPressureDensity")
-
-
-class TurbulenceModelModelType(str, Enum):
-    """Turbulence model type"""
-
-    SA = "SpalartAllmaras"
-    SST = "kOmegaSST"
-    NONE = "None"
-
-
-class TurbulenceModelConstants(Flow360BaseModel):
-    """TurbulenceModelConstants"""
-
-    C_DES: Optional[float]
-    C_d: Optional[float]
-    C_DES1: Optional[float]
-    C_DES2: Optional[float]
-    C_d1: Optional[float]
-    C_d2: Optional[float]
-
-
-class TurbulenceModelSolver(GenericSolverSettings):
-    """:class:`TurbulenceModelSolver` class for setting up turbulence model solver
-
-    Parameters
-    ----------
-
-    model_type :
-        Turbulence model type can be: “SpalartAllmaras”, “kOmegaSST” or "None"
-
-    absoluteTolerance :
-        Tolerance for the NS residual, below which the solver goes to the next physical step
-
-    relativeTolerance :
-        Tolerance to the relative residual, below which the solver goes to the next physical step. Relative residual is
-        defined as the ratio of the current pseudoStep’s residual to the maximum residual present in the first
-        10 pseudoSteps within the current physicalStep. NOTE: relativeTolerance is ignored in steady simulations and
-        only absoluteTolerance is used as the convergence criterion
-
-    linearIterations :
-        Number of linear solver iterations
-
-    updateJacobianFrequency :
-        Frequency at which the jacobian is updated.
-
-    equationEvalFrequency :
-        Frequency at which to update the NS equation in loosely-coupled simulations
-
-    maxForceJacUpdatePhysicalSteps :
-        When which physical steps, the jacobian matrix is updated every pseudo step
-
-    orderOfAccuracy :
-        Order of accuracy in space
-
-    reconstruction_gradient_limiter :
-        The strength of gradient limiter used in reconstruction of solution variables at the faces (specified in the
-        range [0.0, 2.0]). 0.0 corresponds to setting the gradient equal to zero, and 2.0 means no limiting.
-
-    rotation_correction : bool, optional
-        Rotation correction for the turbulence model. Only support for SpalartAllmaras
-
-    quadratic_constitutive_relation : bool, optional
-        Use quadratic constitutive relation for turbulence shear stress tensor instead of Boussinesq Approximation
-
-    DDES : bool, optional
-        Enables Delayed Detached Eddy Simulation. Supported for both SpalartAllmaras and kOmegaSST turbulence models,
-        with and without AmplificationFactorTransport transition model enabled.
-
-    grid_size_for_LES : Literal['maxEdgeLength', 'meanEdgeLength'], optional
-        Specifes the length used for the computation of LES length scale. The allowed inputs are "maxEdgeLength"
-        (default) and "meanEdgeLength"
-
-    model_constants :
-        Here, user can change the default values used for DDES coefficients in the solver:
-        SpalartAllmaras: "C_DES" (= 0.72), "C_d" (= 8.0)
-        kOmegaSST: "C_DES1" (= 0.78), "C_DES2" (= 0.61), "C_d1" (= 20.0), "C_d2" (= 3.0)
-        (values shown in the parentheses are the default values used in Flow360)
-        An example with kOmegaSST mode would be: {"C_DES1": 0.85, "C_d1": 8.0}
-
-    Returns
-    -------
-    :class:`TurbulenceModelSolver`
-        An instance of the component class TurbulenceModelSolver.
-
-    Example
-    -------
-    >>> ts = TurbulenceModelSolver(model_type='SA', absolute_tolerance=1e-10)
-    """
-
-    model_type: TurbulenceModelModelType = pd.Field(
-        alias="modelType", default=TurbulenceModelModelType.SA
-    )
-    reconstruction_gradient_limiter: Optional[pd.confloat(ge=0, le=2)] = pd.Field(
-        alias="reconstructionGradientLimiter"
-    )
-    rotation_correction: Optional[bool] = pd.Field(alias="rotationCorrection")
-    quadratic_constitutive_relation: Optional[bool] = pd.Field(
-        alias="quadraticConstitutiveRelation"
-    )
-    DDES: Optional[bool]
-    grid_size_for_LES: Optional[Literal["maxEdgeLength", "meanEdgeLength"]] = pd.Field(
-        alias="gridSizeForLES"
-    )
-    model_constants: Optional[TurbulenceModelConstants] = pd.Field(alias="modelConstants")
-
-    @pd.validator("model_type", pre=True, always=True)
-    def validate_model_type(cls, v):
-        """Turbulence model validator"""
-        if v == "SA":
-            return TurbulenceModelModelType.SA
-        if v == "SST":
-            return TurbulenceModelModelType.SST
-        if v == "None":
-            return TurbulenceModelModelType.NONE
-        return v
-
-
 class Flow360Params(Flow360BaseModel):
     """
     Flow360 solver parameters
     """
 
     geometry: Optional[Geometry] = pd.Field()
     boundaries: Optional[Boundaries] = pd.Field()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flow360-0.2.0b2/flow360/component/meshing/params.py` & `flow360-0.2.0b3/flow360/component/meshing/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Flow360 meshing parameters
 """
-from typing import Optional, Union, List
-from typing_extensions import Literal
-import pydantic as pd
+from typing import List, Optional, Union
 
-from ..types import PositiveFloat, NonNegativeFloat, Coordinate, Axis, Size
+import pydantic as pd
+from typing_extensions import Literal
 
-from ..params_base import Flow360BaseModel, Flow360SortableBaseModel
 from ...exceptions import ValidationError
+from ..flow360_params.params_base import Flow360BaseModel, Flow360SortableBaseModel
+from ..types import Axis, Coordinate, NonNegativeFloat, PositiveFloat, Size
 
 
 class Aniso(Flow360BaseModel):
     """Aniso edge"""
 
     type = pd.Field("aniso", const=True)
     method: Literal["angle", "height", "aspectRatio"] = pd.Field()
```

### Comparing `flow360-0.2.0b2/flow360/component/params_base.py` & `flow360-0.2.0b3/flow360/component/flow360_params/params_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 Flow360 solver parameters
 """
 from __future__ import annotations
-from typing import Any, Optional, List
-from functools import wraps
+
 import json
-from typing_extensions import Literal
+from functools import wraps
+from typing import Any, List, Optional
+
+import numpy as np
+import pydantic as pd
 import rich
 import yaml
-import numpy as np
 from pydantic import BaseModel
 from pydantic.fields import ModelField
-import pydantic as pd
+from typing_extensions import Literal
 
-from .types import TYPE_TAG_STR
-from ..exceptions import FileError, ConfigError, ValidationError
-from ..log import log
+from ...exceptions import ConfigError, FileError, ValidationError
+from ...log import log
+from ..types import TYPE_TAG_STR
 
 
 def json_dumps(value, *args, **kwargs):
     """custom json dump with sort_keys=True"""
     return json.dumps(value, sort_keys=True, *args, **kwargs)
 
 
@@ -147,15 +149,15 @@
                 raise ConfigError(f"One of {cls.Config.require_one_of} is required.")
         return values
 
     def copy(self, update=None, **kwargs) -> Flow360BaseModel:
         """Copy a Flow360BaseModel.  With ``deep=True`` as default."""
         if "deep" in kwargs and kwargs["deep"] is False:
             raise ValueError("Can't do shallow copy of component, set `deep=True` in copy().")
-        kwargs.update(dict(deep=True))
+        kwargs.update({"deep": True})
         new_copy = BaseModel.copy(self, update=update, **kwargs)
         return self.validate(new_copy.dict())
 
     def help(self, methods: bool = False) -> None:
         """Prints message describing the fields and methods of a :class:`Flow360BaseModel`.
 
         Parameters
```

### Comparing `flow360-0.2.0b2/flow360/component/resource_base.py` & `flow360-0.2.0b3/flow360/component/resource_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Flow360 base Model
 """
+import traceback
+from abc import ABC
 from datetime import datetime
 from enum import Enum
-from typing import List, Optional, Union
 from functools import wraps
-from abc import ABC
+from typing import List, Optional, Union
+
 from pydantic import BaseModel, Extra, Field
 
 from ..cloud.rest_api import RestApi
+from ..log import log
 
 
 class Flow360Status(Enum):
     """
     Flow360Status component
     """
 
@@ -106,14 +109,21 @@
 
 class ResourceDraft(ABC):
     """
     Abstract base class for resources in draft state (before submission).
     """
 
     _id = None
+    traceback = None
+
+    def __init__(self):
+        # remove from traceback:
+        # 1. This line (self.traceback)
+        # 2. Call of this init
+        self.traceback = traceback.format_stack()[:-2]
 
     @property
     def id(self):
         """
         returns id of resource
         """
         return self._id
@@ -126,14 +136,24 @@
         bool
             True if resource is cloud resources (after submission), False otherwise
         """
         if self.id is None:
             return False
         return True
 
+    def __del__(self):
+        if self.is_cloud_resource() is False and self.traceback is not None:
+            log.warning(
+                f"\
+You have not submitted your {self.__class__.__name__} to cloud. \
+It will not be process. Please run .submit() after .create()"
+            )
+            for line in self.traceback:
+                print(line.strip())
+
 
 class Flow360Resource(RestApi):
     """
     Flow360 base resource model
     """
 
     def __init__(self, resource_type, info_type_class, *args, s3_transfer_method=None, **kwargs):
```

### Comparing `flow360-0.2.0b2/flow360/component/surface_mesh.py` & `flow360-0.2.0b3/flow360/component/surface_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
 Surface mesh component
 """
 from __future__ import annotations
+
 import os
 from enum import Enum
-from typing import Union, List, Iterator
+from typing import Iterator, List, Union
+
 import pydantic as pd
 
+from ..cloud.rest_api import RestApi
+from ..cloud.s3_utils import S3TransferType
+from ..exceptions import FileError as FlFileError
+from ..exceptions import ValueError as FlValueError
+from .flow360_params.params_base import params_generic_validator
+from .meshing.params import SurfaceMeshingParams, VolumeMeshingParams
 from .resource_base import (
-    Flow360ResourceBaseModel,
     Flow360Resource,
+    Flow360ResourceBaseModel,
     Flow360ResourceListBase,
     ResourceDraft,
 )
-from .params_base import params_generic_validator
-from .volume_mesh import VolumeMeshDraft
-from .meshing.params import SurfaceMeshingParams, VolumeMeshingParams
 from .validator import Validator
-from ..cloud.s3_utils import S3TransferType
-from ..cloud.rest_api import RestApi
-from ..exceptions import FileError as FlFileError
-from ..exceptions import ValueError as FlValueError
+from .volume_mesh import VolumeMeshDraft
 
 
 class SurfaceMeshDownloadable(Enum):
     """
     Surface Mesh downloadable files
     """
 
@@ -78,14 +80,15 @@
         self.name = name
         self.tags = tags
         self.solver_version = solver_version
         self._id = None
         self.params = params
         self._validate()
         self.params = params.copy(deep=True)
+        ResourceDraft.__init__(self)
 
     def _validate(self):
         _, ext = os.path.splitext(self.geometry_file)
         if ext not in [".csm", ".egads"]:
             raise FlValueError(
                 f"Unsupported geometry file extensions: {ext}. Supported: [csm, egads]."
             )
@@ -266,23 +269,23 @@
         Get surface mesh from cloud
         :param surface_mesh_id:
         :return:
         """
         return cls(surface_mesh_id)
 
     @classmethod
-    def new(
+    def create(
         cls,
         geometry_file: str,
         params: SurfaceMeshingParams,
         name: str = None,
         tags: List[str] = None,
         solver_version: str = None,
     ) -> SurfaceMeshDraft:
-        """ "New surface mesh from geometry"
+        """ "Create new surface mesh from geometry"
 
         Parameters
         ----------
         geometry_file : str
             _description_
         params : SurfaceMeshingParams
             _description_
@@ -303,15 +306,15 @@
             params=params,
             name=name,
             tags=tags,
             solver_version=solver_version,
         )
         return new_surface_mesh
 
-    def new_volume_mesh(
+    def create_volume_mesh(
         self,
         name: str,
         params: VolumeMeshingParams,
         tags: List[str] = None,
         solver_version=None,
     ) -> VolumeMeshDraft:
         """
```

### Comparing `flow360-0.2.0b2/flow360/component/types.py` & `flow360-0.2.0b3/flow360/component/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Defines 'types' that various fields can be """
 
-from typing import Tuple, Union, List, Optional
-from typing_extensions import Annotated, Literal
+from typing import List, Optional, Tuple, Union
 
 import pydantic as pd
+from typing_extensions import Annotated, Literal
+
 from ..exceptions import ValidationError
 
 # type tag default name
 TYPE_TAG_STR = "_type"
 
 
 def annotate_type(UnionType):  # pylint:disable=invalid-name
```

### Comparing `flow360-0.2.0b2/flow360/component/utils.py` & `flow360-0.2.0b3/flow360/component/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Utility functions
 """
-from functools import wraps
 import uuid
+from functools import wraps
 
 from ..log import log
 
 
 # pylint: disable=redefined-builtin
 def is_valid_uuid(id, ignore_none=False):
     """
```

### Comparing `flow360-0.2.0b2/flow360/component/validator.py` & `flow360-0.2.0b3/flow360/component/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Validator API
 """
 from enum import Enum
 from typing import Union
 
-from .flow360_params import Flow360Params
-from .meshing.params import SurfaceMeshingParams, VolumeMeshingParams
 from ..cloud.rest_api import RestApi
-from ..exceptions import ValueError as FlValueError
 from ..exceptions import ValidationError
+from ..exceptions import ValueError as FlValueError
 from ..log import log
+from .flow360_params.flow360_params import Flow360Params
+from .meshing.params import SurfaceMeshingParams, VolumeMeshingParams
 
 
 class Validator(Enum):
     """ ":class: Validator"""
 
     VOLUME_MESH = "VolumeMesh"
     SURFACE_MESH = "SurfaceMesh"
```

### Comparing `flow360-0.2.0b2/flow360/component/volume_mesh.py` & `flow360-0.2.0b3/flow360/component/volume_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 """
 Volume mesh component
 """
 from __future__ import annotations
+
 import os.path
 from enum import Enum
-from typing import Optional, Union, List, Iterator
+from typing import Iterator, List, Optional, Union
+
 import numpy as np
 from pydantic import Extra, Field, validator
 
-from ..cloud.s3_utils import S3TransferType
 from ..cloud.rest_api import RestApi
+from ..cloud.s3_utils import S3TransferType
+from ..exceptions import FileError as FlFileError
+from ..exceptions import Flow360NotImplementedError
+from ..exceptions import ValueError as FlValueError
+from ..log import log
 from ..solver_version import Flow360Version
-from .resource_base import (
-    Flow360ResourceBaseModel,
-    Flow360Resource,
-    Flow360ResourceListBase,
-    ResourceDraft,
-)
-from .flow360_params import (
+from .case import Case, CaseDraft
+from .flow360_params.flow360_params import (
     Flow360MeshParams,
     Flow360Params,
     NoSlipWall,
     _GenericBoundaryWrapper,
 )
+from .flow360_params.params_base import params_generic_validator
 from .meshing.params import VolumeMeshingParams
-from .case import Case, CaseDraft
-from .params_base import params_generic_validator
+from .resource_base import (
+    Flow360Resource,
+    Flow360ResourceBaseModel,
+    Flow360ResourceListBase,
+    ResourceDraft,
+)
 from .validator import Validator
 
-from ..log import log
-from ..exceptions import ValueError as FlValueError
-from ..exceptions import FileError as FlFileError
-from ..exceptions import Flow360NotImplementedError
-
 try:
     import h5py
 
     _H5PY_AVAILABLE = True
 except ImportError:
     _H5PY_AVAILABLE = False
 
@@ -53,15 +54,14 @@
     return data_str
 
 
 def get_no_slip_walls(params: Union[Flow360Params, Flow360MeshParams]):
     """
     Get wall boundary names
     :param params:
-    :param solver_version:
     :return:
     """
     assert params
 
     if (
         isinstance(params, Flow360MeshParams)
         and params.boundaries
@@ -79,15 +79,14 @@
     return []
 
 
 def get_boundries_from_sliding_interfaces(params: Union[Flow360Params, Flow360MeshParams]):
     """
     Get wall boundary names
     :param params:
-    :param solver_version:
     :return:
     """
     assert params
     res = []
 
     if params.sliding_interfaces and params.sliding_interfaces.rotating_patches:
         res += params.sliding_interfaces.rotating_patches[:]
@@ -153,23 +152,18 @@
     :param params:
     :param solver_version:
     :return:
     """
     assert cgns_file
     assert params
     boundaries_in_file = get_boundaries_from_file(cgns_file, solver_version)
-
     boundaries_in_params = get_no_slip_walls(params) + get_boundries_from_sliding_interfaces(params)
-    print(get_no_slip_walls(params), boundaries_in_params)
-
     boundaries_in_file = set(boundaries_in_file)
     boundaries_in_params = set(boundaries_in_params)
 
-    print(boundaries_in_file, boundaries_in_params)
-
     if not boundaries_in_file.issuperset(boundaries_in_params):
         raise FlValueError(
             "The following input boundary names from mesh json are not found in mesh:"
             + f" {' '.join(boundaries_in_params - boundaries_in_file)}."
             + f" Boundary names in cgns: {' '.join(boundaries_in_file)}"
             + f" Boundary names in params: {' '.join(boundaries_in_file)}"
         )
@@ -304,15 +298,15 @@
     """
 
     id: str = Field(alias="meshId")
     name: str = Field(alias="meshName")
     created_at: str = Field(alias="meshAddTime")
     surface_mesh_id: Optional[str] = Field(alias="surfaceMeshId")
     mesh_params: Union[Flow360MeshParams, None, dict] = Field(alias="meshParams")
-    mesh_format: VolumeMeshFileFormat = Field(alias="meshFormat")
+    mesh_format: Union[VolumeMeshFileFormat, None] = Field(alias="meshFormat")
     endianness: UGRIDEndianness = Field(alias="meshEndianness")
     compression: CompressionFormat = Field(alias="meshCompression")
     boundaries: Union[List, None]
 
     @validator("mesh_params", pre=True)
     def init_mesh_params(cls, value):
         """
@@ -365,40 +359,40 @@
         surface_mesh_id=None,
         tags: List[str] = None,
         solver_version=None,
         endianess: UGRIDEndianness = None,
         isascii: bool = False,
     ):
         if file_name is not None and not os.path.exists(file_name):
-            raise FlFileError(f"{file_name} not found.")
+            raise FlFileError(f"File '{file_name}' not found.")
 
         if endianess is not None:
             raise Flow360NotImplementedError(
                 "endianess selections not supported, it is inferred from filename"
             )
 
         if isascii is True:
             raise Flow360NotImplementedError("isascii not supported")
 
         self.params = None
         if params is not None:
+            if not isinstance(params, Flow360MeshParams):
+                raise ValueError(f"params={params} are not of type Flow360MeshParams")
             self.params = params.copy(deep=True)
 
-        # if not params or not isinstance(params, Flow360MeshParams):
-        #     raise ValueError(f'params={params} are not of type Flow360MeshParams')
-
         if name is None and file_name is not None:
             name = os.path.splitext(os.path.basename(file_name))[0]
 
         self.file_name = file_name
         self.name = name
         self.surface_mesh_id = surface_mesh_id
         self.tags = tags
         self.solver_version = solver_version
         self._id = None
+        ResourceDraft.__init__(self)
 
     def _submit_from_surface(self):
         self.validator_api(self.params, solver_version=self.solver_version)
         body = {
             "name": self.name,
             "tags": self.tags,
             "surfaceMeshId": self.surface_mesh_id,
@@ -463,15 +457,14 @@
             Use for custom progress bar, by default None
 
         Returns
         -------
         VolumeMesh
             VolumeMesh object with id
         """
-        print(self.surface_mesh_id, self.name, self.params, self.file_name)
 
         if self.file_name is not None:
             return self._submit_upload_mesh(progress_callback)
 
         if self.surface_mesh_id is not None and self.name is not None and self.params is not None:
             return self._submit_from_surface()
 
@@ -665,15 +658,15 @@
             solver_version=solver_version,
             params=params,
             endianess=endianess,
             isascii=isascii,
         )
 
     @classmethod
-    def new(
+    def create(
         cls,
         name: str,
         params: VolumeMeshingParams,
         surface_mesh_id,
         tags: List[str] = None,
         solver_version=None,
     ) -> VolumeMeshDraft:
@@ -685,29 +678,32 @@
             name=name,
             surface_mesh_id=surface_mesh_id,
             solver_version=solver_version,
             params=params,
             tags=tags,
         )
 
-    def new_case(
+    def create_case(
         self,
         name: str,
         params: Flow360Params,
         tags: List[str] = None,
+        solver_version: str = None,
     ) -> CaseDraft:
         """
         Create new case
         :param name:
         :param params:
         :param tags:
         :return:
         """
 
-        return Case.new(name, params, volume_mesh_id=self.id, tags=tags)
+        return Case.create(
+            name, params, volume_mesh_id=self.id, tags=tags, solver_version=solver_version
+        )
 
 
 class VolumeMeshList(Flow360ResourceListBase):
     """
     VolumeMesh List component
     """
```

### Comparing `flow360-0.2.0b2/flow360/environment.py` & `flow360-0.2.0b3/flow360/environment.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/actuatorDisk/flow360.json` & `flow360-0.2.0b3/flow360/examples/actuatorDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/airplane/geometry.csm` & `flow360-0.2.0b3/flow360/examples/airplane/geometry.csm`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/airplane/surface_params.json` & `flow360-0.2.0b3/flow360/examples/airplane/surface_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/airplane/volume_params.json` & `flow360-0.2.0b3/flow360/examples/airplane/volume_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/base_test_case.py` & `flow360-0.2.0b3/flow360/examples/base_test_case.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 base component for examples
 """
 
 
-import os
-import requests
 import glob
-from pathlib import Path
+import os
 from abc import ABC, abstractmethod, abstractstaticmethod
+from pathlib import Path
+
+import requests
 
 from ..solver_version import Flow360Version
 
 here = os.path.dirname(os.path.abspath(__file__))
 
 
 def download(url, filename):
@@ -21,205 +22,185 @@
         fh.write(response.content)
 
 
 def version_parse(str):
     return Flow360Version(str.strip("lgte"))
 
 
+class classproperty(property):
+    def __get__(self, owner_self, owner_cls):
+        return self.fget(owner_cls)
+
+
 class url_base(ABC):
     @property
     @abstractmethod
     def geometry(self):
-        pass
+        """geometry"""
 
     @property
     @abstractmethod
     def mesh(self):
-        pass
+        """mesh"""
 
     @property
     @abstractmethod
     def mesh_json(self):
-        pass
+        """mesh_json"""
 
     @property
     @abstractmethod
     def case_json(self):
-        pass
+        """case_json"""
 
     @property
     @abstractmethod
     def case_yaml(self):
-        pass
+        """case_yaml"""
 
+    @property
     @abstractmethod
     def surface_json(self):
-        pass
+        """surface_json"""
 
+    @property
     @abstractmethod
     def surface_yaml(self):
-        pass
+        """surface_yaml"""
 
 
 class BaseTestCase(ABC):
     _solver_version = None
 
     @property
     @abstractstaticmethod
-    def name():
-        pass
+    def name(cls):
+        """name"""
 
     @property
     @abstractstaticmethod
     def url(cls) -> url_base:
-        pass
+        """url"""
 
     @classmethod
     def _get_version_prefix(cls):
         if cls._solver_version == None:
             return ""
 
         versionList = [
             os.path.basename(f) for f in glob.glob(os.path.join(here, cls.name, "release-*"))
         ]
         versionList.sort(key=version_parse)
-
         for v in versionList:
-            try:
-                if version_parse(v) == version_parse(cls._solver_version):
-                    return v
-            except:
-                pass
+            if v == cls._solver_version:
+                return v
 
             suffix = v[-2:]
             if suffix == "ge":
                 if version_parse(v) >= version_parse(cls._solver_version):
                     return v
             elif suffix == "gt":
                 if version_parse(v) > version_parse(cls._solver_version):
                     return v
 
         versionList.reverse()
         for v in versionList:
+            suffix = v[-2:]
             if suffix == "le":
                 if version_parse(v) <= version_parse(cls._solver_version):
                     return v
             elif suffix == "lt":
                 if version_parse(v) < version_parse(cls._solver_version):
                     return v
 
         return ""
 
     @classmethod
     def _real_path(cls, *args):
         return os.path.join(here, cls.name, *args)
 
-    @classmethod
-    @property
+    @classproperty
     def _geometry_filename(cls):
         return cls._real_path(os.path.basename(cls.url.geometry))
 
-    @classmethod
-    @property
+    @classproperty
     def _mesh_filename(cls):
         return cls._real_path(os.path.basename(cls.url.mesh))
 
-    @classmethod
-    @property
+    @classproperty
     def _mesh_json(cls):
         versionPrefix = cls._get_version_prefix()
         return cls._real_path(versionPrefix, os.path.basename(cls.url.mesh_json))
 
-    @classmethod
-    @property
+    @classproperty
     def _case_json(cls):
         versionPrefix = cls._get_version_prefix()
         return cls._real_path(versionPrefix, os.path.basename(cls.url.case_json))
 
-    @classmethod
-    @property
+    @classproperty
     def _case_yaml(cls):
         versionPrefix = cls._get_version_prefix()
         return cls._real_path(versionPrefix, os.path.basename(cls.url.case_yaml))
 
-    @classmethod
-    @property
+    @classproperty
     def _surface_json(cls):
         versionPrefix = cls._get_version_prefix()
         return cls._real_path(versionPrefix, os.path.basename(cls.url.surface_json))
 
-    @classmethod
-    @property
+    @classproperty
     def _volume_json(cls):
         versionPrefix = cls._get_version_prefix()
         return cls._real_path(versionPrefix, os.path.basename(cls.url.volume_json))
 
     @classmethod
     def is_file_downloaded(cls, file):
         if not os.path.exists(file):
-            raise RuntimeError(f"File not found. Run get_files() first to download files.")
+            raise FileNotFoundError(f"File not found. Run get_files() first to download files.")
         return file
 
-    @classmethod
-    @property
+    @classproperty
     def geometry(cls):
         return cls.is_file_downloaded(cls._geometry_filename)
 
-    @classmethod
-    @property
+    @classproperty
     def mesh_filename(cls):
         return cls.is_file_downloaded(cls._mesh_filename)
 
-    @classmethod
-    @property
+    @classproperty
     def mesh_json(cls):
         return cls.is_file_downloaded(cls._mesh_json)
 
-    @classmethod
-    @property
+    @classproperty
     def case_json(cls):
         return cls.is_file_downloaded(cls._case_json)
 
-    @classmethod
-    @property
+    @classproperty
     def case_yaml(cls):
         return cls.is_file_downloaded(cls._case_yaml)
 
-    @classmethod
-    @property
+    @classproperty
     def surface_json(cls):
         return cls.is_file_downloaded(cls._surface_json)
 
-    @classmethod
-    @property
+    @classproperty
     def volume_json(cls):
         return cls.is_file_downloaded(cls._volume_json)
 
     @classmethod
     def set_version(cls, version):
         cls._solver_version = version
 
     @classmethod
+    def _get_file(cls, remote_filename, local_filename):
+        if not os.path.exists(local_filename):
+            download(remote_filename, local_filename)
+
+    @classmethod
     def get_files(cls):
-        try:
-            if not os.path.exists(cls._mesh_filename):
-                download(cls.url.mesh, cls._mesh_filename)
-        except AttributeError:
-            pass
-
-        try:
-            if not os.path.exists(cls._mesh_json):
-                download(cls.url.mesh_json, cls._mesh_json)
-        except AttributeError:
-            pass
-
-        try:
-            if not os.path.exists(cls._case_json):
-                download(cls.url.case_json, cls._case_json)
-        except AttributeError:
-            pass
-
-        try:
-            if not os.path.exists(cls._case_yaml):
-                download(cls.url.case_yaml, cls._case_yaml)
-        except AttributeError:
-            pass
+        if hasattr(cls.url, "mesh"):
+            cls._get_file(cls.url.mesh, cls._mesh_filename)
+        if hasattr(cls.url, "mesh_json"):
+            cls._get_file(cls.url.mesh_json, cls._mesh_json)
+        if hasattr(cls.url, "case_json"):
+            cls._get_file(cls.url.case_json, cls._case_json)
+        if hasattr(cls.url, "case_yaml"):
+            cls._get_file(cls.url.case_yaml, cls._case_yaml)
```

### Comparing `flow360-0.2.0b2/flow360/examples/betDisk/flow360.json` & `flow360-0.2.0b3/flow360/examples/betDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/betLine/flow360.json` & `flow360-0.2.0b3/flow360/examples/betLine/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/betLine/release-21.3.3.0ge/flow360.json` & `flow360-0.2.0b3/flow360/examples/betLine/release-21.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/cylinder/flow360.json` & `flow360-0.2.0b3/flow360/examples/cylinder/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b3/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/om6wing/case.yaml` & `flow360-0.2.0b3/flow360/examples/om6wing/case.yaml`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/om6wing/flow360.json` & `flow360-0.2.0b3/flow360/examples/om6wing/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json` & `flow360-0.2.0b3/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/rotatingSpheres/flow360.json` & `flow360-0.2.0b3/flow360/examples/rotatingSpheres/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/rotatingSpheres/flow360mesh.json` & `flow360-0.2.0b3/flow360/examples/rotatingSpheres/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json` & `flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json` & `flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json` & `flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/exceptions.py` & `flow360-0.2.0b3/flow360/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/flow360/log.py` & `flow360-0.2.0b3/flow360/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Logging for Flow360."""
 
 from typing import Union
-from typing_extensions import Literal
 
 from rich.console import Console
-
+from typing_extensions import Literal
 
 LogLevel = Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
 LogValue = Union[int, LogLevel]
 
 # Logging levels compatible with logging module
 _level_value = {
     "DEBUG": 10,
```

### Comparing `flow360-0.2.0b2/flow360/solver_version.py` & `flow360-0.2.0b3/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b2/pyproject.toml` & `flow360-0.2.0b3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow360"
-version = "v0.2.0b2"
+version = "v0.2.0b3"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7.4"
 pydantic = "^1.9.2"
 pytest = "^7.1.2"
@@ -12,33 +12,31 @@
 toml = "^0.10.2"
 requests = "^2.28.1"
 boto3 = "^1.24.63"
 numpy = [{ python = "^3.7", version = "^1.19.0" },
     { python = "^3.8", version = "^1.20.0" },
     { python = "^3.9", version = "^1.23.0" },
     { python = "^3.10", version = "^1.23.0" }]
-h5py = "^3.7.0"
 matplotlib =  [{ python = "^3.7", version = "^3.5.3" },
     { python = "^3.8", version = "^3.6.2" },
     { python = "^3.9", version = "^3.6.2" },
     { python = "^3.10", version = "^3.6.2" }]
 pyyaml = "^6.0"
-
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-autohooks = "^22.8.1"
-autohooks-plugin-black = "^22.8.1"
-autohooks-plugin-pylint = "^22.8.1"
-autohooks-plugin-isort = "^22.8.0"
-pylint = "^2.15.0"
-
+rich = "^13.3.4"
+h5py = "^3.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
+autohooks = "^23.4.0"
+autohooks-plugin-black = "^22.11.0"
+autohooks-plugin-isort = "^22.8.0"
+autohooks-plugin-pylint = "^22.8.1"
+pytest = "^7.3.0"
+pylint = "^2.17.2"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 line-length = 100
 target-version = ["py37", "py38", "py39", "py310", "py311"]
```

### Comparing `flow360-0.2.0b2/PKG-INFO` & `flow360-0.2.0b3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 0.2.0b2
+Version: 0.2.0b3
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.24.63,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: h5py (>=3.7.0,<4.0.0)
+Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0) ; python_version >= "3.8" and python_version < "4.0"
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0) ; python_version >= "3.9" and python_version < "4.0"
 Requires-Dist: numpy (>=1.19.0,<2.0.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: numpy (>=1.20.0,<2.0.0) ; python_version >= "3.8" and python_version < "4.0"
 Requires-Dist: numpy (>=1.23.0,<2.0.0) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: numpy (>=1.23.0,<2.0.0) ; python_version >= "3.9" and python_version < "4.0"
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

