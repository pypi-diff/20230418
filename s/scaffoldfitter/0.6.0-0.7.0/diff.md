# Comparing `tmp/scaffoldfitter-0.6.0.tar.gz` & `tmp/scaffoldfitter-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaffoldfitter-0.6.0.tar", last modified: Thu Feb  9 03:25:44 2023, max compression
+gzip compressed data, was "scaffoldfitter-0.7.0.tar", last modified: Mon Apr 17 23:27:23 2023, max compression
```

## Comparing `scaffoldfitter-0.6.0.tar` & `scaffoldfitter-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 03:25:44.923043 scaffoldfitter-0.6.0/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      595 2022-07-26 04:30:00.000000 scaffoldfitter-0.6.0/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1523 2023-02-09 03:25:44.922793 scaffoldfitter-0.6.0/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      146 2022-07-26 04:30:53.000000 scaffoldfitter-0.6.0/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-02-09 03:25:44.923126 scaffoldfitter-0.6.0/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1506 2023-02-09 03:24:19.000000 scaffoldfitter-0.6.0/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 03:25:44.917343 scaffoldfitter-0.6.0/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 03:25:44.920487 scaffoldfitter-0.6.0/src/scaffoldfitter/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-04-29 01:16:20.000000 scaffoldfitter-0.6.0/src/scaffoldfitter/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    83772 2023-02-09 03:24:19.000000 scaffoldfitter-0.6.0/src/scaffoldfitter/fitter.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1004 2021-04-29 01:16:20.000000 scaffoldfitter-0.6.0/src/scaffoldfitter/fitterjson.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6564 2021-11-05 08:45:17.000000 scaffoldfitter-0.6.0/src/scaffoldfitter/fitterstep.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    21528 2023-02-09 03:24:19.000000 scaffoldfitter-0.6.0/src/scaffoldfitter/fitterstepalign.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5127 2023-02-09 03:24:19.000000 scaffoldfitter-0.6.0/src/scaffoldfitter/fitterstepconfig.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    29084 2023-02-09 03:24:19.000000 scaffoldfitter-0.6.0/src/scaffoldfitter/fitterstepfit.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-02-09 03:25:44.922449 scaffoldfitter-0.6.0/src/scaffoldfitter.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1523 2023-02-09 03:25:44.000000 scaffoldfitter-0.6.0/src/scaffoldfitter.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      516 2023-02-09 03:25:44.000000 scaffoldfitter-0.6.0/src/scaffoldfitter.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-02-09 03:25:44.000000 scaffoldfitter-0.6.0/src/scaffoldfitter.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2021-04-29 01:16:31.000000 scaffoldfitter-0.6.0/src/scaffoldfitter.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002       58 2023-02-09 03:25:44.000000 scaffoldfitter-0.6.0/src/scaffoldfitter.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       15 2023-02-09 03:25:44.000000 scaffoldfitter-0.6.0/src/scaffoldfitter.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:27:23.668990 scaffoldfitter-0.7.0/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      595 2022-07-26 04:30:00.000000 scaffoldfitter-0.7.0/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1503 2023-04-17 23:27:23.668727 scaffoldfitter-0.7.0/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      136 2023-04-17 23:22:31.000000 scaffoldfitter-0.7.0/README.rst
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-17 23:27:23.669075 scaffoldfitter-0.7.0/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1472 2023-04-17 23:26:11.000000 scaffoldfitter-0.7.0/setup.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:27:23.661914 scaffoldfitter-0.7.0/src/
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:27:23.666278 scaffoldfitter-0.7.0/src/scaffoldfitter/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-04-29 01:16:20.000000 scaffoldfitter-0.7.0/src/scaffoldfitter/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    83748 2023-04-17 23:22:31.000000 scaffoldfitter-0.7.0/src/scaffoldfitter/fitter.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1004 2021-04-29 01:16:20.000000 scaffoldfitter-0.7.0/src/scaffoldfitter/fitterjson.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     6564 2021-11-05 08:45:17.000000 scaffoldfitter-0.7.0/src/scaffoldfitter/fitterstep.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    22789 2023-04-17 23:22:31.000000 scaffoldfitter-0.7.0/src/scaffoldfitter/fitterstepalign.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5127 2023-02-09 03:24:19.000000 scaffoldfitter-0.7.0/src/scaffoldfitter/fitterstepconfig.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    29075 2023-04-17 23:22:31.000000 scaffoldfitter-0.7.0/src/scaffoldfitter/fitterstepfit.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:27:23.668356 scaffoldfitter-0.7.0/src/scaffoldfitter.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1503 2023-04-17 23:27:23.000000 scaffoldfitter-0.7.0/src/scaffoldfitter.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      516 2023-04-17 23:27:23.000000 scaffoldfitter-0.7.0/src/scaffoldfitter.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-17 23:27:23.000000 scaffoldfitter-0.7.0/src/scaffoldfitter.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2021-04-29 01:16:31.000000 scaffoldfitter-0.7.0/src/scaffoldfitter.egg-info/not-zip-safe
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-17 23:27:23.000000 scaffoldfitter-0.7.0/src/scaffoldfitter.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       15 2023-04-17 23:27:23.000000 scaffoldfitter-0.7.0/src/scaffoldfitter.egg-info/top_level.txt
```

### Comparing `scaffoldfitter-0.6.0/LICENSE` & `scaffoldfitter-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scaffoldfitter-0.6.0/PKG-INFO` & `scaffoldfitter-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: scaffoldfitter
-Version: 0.6.0
-Summary: Scaffold/model geometric fitting library using OpenCMISS-Zinc.
+Version: 0.7.0
+Summary: Scaffold/model geometric fitting library using Zinc.
 Home-page: https://github.com/ABI-Software/scaffoldfitter
 Author: Auckland Bioengineering Institute
 Author-email: r.christie@auckland.ac.nz
 License: Apache Software License
 Description: Scaffold Fitter
         ===============
         
-        Scaffold/model fitter using OpenCMISS-Zinc.
+        Scaffold/model fitter using Zinc.
         
         Install with the following command::
         
           pip install scaffoldfitter
```

### Comparing `scaffoldfitter-0.6.0/setup.py` & `scaffoldfitter-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 
 readme = readfile("README.rst", split=True)
 # For requirements not hosted on PyPi place listings
 # into the 'requirements.txt' file.
 requires = [
     # minimal requirements listing
-    "opencmiss.maths",
-    "opencmiss.utils >= 0.3",
-    "opencmiss.zinc >= 3.10"
+    "cmlibs.maths",
+    "cmlibs.utils",
+    "cmlibs.zinc"
 ]
 readme.extend(['', 'License', '=======', '', '::', ''])
 source_license = readfile("LICENSE")
 
 setup(
     name="scaffoldfitter",
-    version="0.6.0",
-    description="Scaffold/model geometric fitting library using OpenCMISS-Zinc.",
+    version="0.7.0",
+    description="Scaffold/model geometric fitting library using Zinc.",
     long_description="\n".join(readme) + source_license,
     long_description_content_type="text/x-rst",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Medical Science Apps."
     ],
```

### Comparing `scaffoldfitter-0.6.0/src/scaffoldfitter/fitter.py` & `scaffoldfitter-0.7.0/src/scaffoldfitter/fitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Main class for fitting scaffolds.
 """
 
 import json
 
-from opencmiss.maths.vectorops import sub
-from opencmiss.utils.zinc.field import assignFieldParameters, createFieldFiniteElementClone, getGroupList, \
+from cmlibs.maths.vectorops import sub
+from cmlibs.utils.zinc.field import assignFieldParameters, createFieldFiniteElementClone, getGroupList, \
     findOrCreateFieldFiniteElement, findOrCreateFieldStoredMeshLocation, getUniqueFieldName, orphanFieldByName
-from opencmiss.utils.zinc.finiteelement import evaluateFieldNodesetMean, evaluateFieldNodesetRange, \
+from cmlibs.utils.zinc.finiteelement import evaluateFieldNodesetMean, evaluateFieldNodesetRange, \
     findNodeWithName, getMaximumNodeIdentifier
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.context import Context
-from opencmiss.zinc.element import Elementbasis, Elementfieldtemplate
-from opencmiss.zinc.field import Field, FieldFindMeshLocation, FieldGroup
-from opencmiss.zinc.result import RESULT_OK, RESULT_WARNING_PART_DONE
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.context import Context
+from cmlibs.zinc.element import Elementbasis, Elementfieldtemplate
+from cmlibs.zinc.field import Field, FieldFindMeshLocation, FieldGroup
+from cmlibs.zinc.result import RESULT_OK, RESULT_WARNING_PART_DONE
 from scaffoldfitter.fitterstep import FitterStep
 from scaffoldfitter.fitterstepconfig import FitterStepConfig
 from scaffoldfitter.fitterstepfit import FitterStepFit
 
 
 class Fitter:
```

### Comparing `scaffoldfitter-0.6.0/src/scaffoldfitter/fitterjson.py` & `scaffoldfitter-0.7.0/src/scaffoldfitter/fitterjson.py`

 * *Files identical despite different names*

### Comparing `scaffoldfitter-0.6.0/src/scaffoldfitter/fitterstep.py` & `scaffoldfitter-0.7.0/src/scaffoldfitter/fitterstep.py`

 * *Files identical despite different names*

### Comparing `scaffoldfitter-0.6.0/src/scaffoldfitter/fitterstepalign.py` & `scaffoldfitter-0.7.0/src/scaffoldfitter/fitterstepalign.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Fit step for gross alignment and scale.
 """
 import copy
 import math
 
-from opencmiss.maths.vectorops import add, div, euler_to_rotation_matrix, matrix_vector_mult, mult, sub
-from opencmiss.utils.zinc.field import get_group_list, create_field_euler_angles_rotation_matrix
-from opencmiss.utils.zinc.finiteelement import evaluate_field_nodeset_mean, getNodeNameCentres
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.element import Mesh
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.optimisation import Optimisation
-from opencmiss.zinc.result import RESULT_OK, RESULT_WARNING_PART_DONE
+from cmlibs.maths.vectorops import add, div, euler_to_rotation_matrix, matrix_vector_mult, mult, sub, identity_matrix
+from cmlibs.utils.zinc.field import get_group_list, create_field_euler_angles_rotation_matrix
+from cmlibs.utils.zinc.finiteelement import evaluate_field_nodeset_mean, getNodeNameCentres
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.element import Mesh
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.optimisation import Optimisation
+from cmlibs.zinc.result import RESULT_OK, RESULT_WARNING_PART_DONE
 from scaffoldfitter.fitterstep import FitterStep
 
 
 def createFieldsTransformations(coordinates: Field, rotation_angles=None, scale_value=1.0,
                                 translation_offsets=None, translation_scale_factor=1.0):
     """
     Create constant fields for rotation, scale and translation containing the supplied
@@ -31,15 +31,15 @@
     """
     if rotation_angles is None:
         rotation_angles = [0.0, 0.0, 0.0]
     if translation_offsets is None:
         translation_offsets = [0.0, 0.0, 0.0]
     components_count = coordinates.getNumberOfComponents()
     assert (components_count == 3) and (len(rotation_angles) == components_count) and isinstance(scale_value, float) \
-           and (len(translation_offsets) == components_count), "createFieldsTransformations.  Invalid arguments"
+        and (len(translation_offsets) == components_count), "createFieldsTransformations.  Invalid arguments"
     fieldmodule = coordinates.getFieldmodule()
     with ChangeManager(fieldmodule):
         # Rotate, scale, and translate model, in that order
         rotation = fieldmodule.createFieldConstant(rotation_angles)
         scale = fieldmodule.createFieldConstant(scale_value)
         translation = fieldmodule.createFieldConstant(translation_offsets)
         rotation_matrix = create_field_euler_angles_rotation_matrix(fieldmodule, rotation)
@@ -200,15 +200,15 @@
         if self._alignGroups or self._alignMarkers:
             self._doAutoAlign()
         fieldmodule = self._fitter.getFieldmodule()
         with ChangeManager(fieldmodule):
             # rotate, scale and translate model
             modelCoordinatesTransformed = createFieldsTransformations(
                 modelCoordinates, self._rotation, self._scale, self._translation)[0]
-            fieldassignment = self._fitter.getModelCoordinatesField().createFieldassignment(modelCoordinatesTransformed)
+            fieldassignment = modelCoordinates.createFieldassignment(modelCoordinatesTransformed)
             result = fieldassignment.assign()
             assert result in [RESULT_OK, RESULT_WARNING_PART_DONE], "Align:  Failed to transform model"
             self._fitter.updateModelReferenceCoordinates()
             del fieldassignment
             del modelCoordinatesTransformed
         self._fitter.calculateDataProjections(self)
         if modelFileNameStem:
@@ -275,14 +275,35 @@
                         print("Align:  Model marker '" + modelName + "' not found in data")
             if writeDiagnostics:
                 for dataName in dataMarkers:
                     print("Align:  Data marker '" + dataName + "' not found in model")
 
         self._optimiseAlignment(pointMap)
 
+    def getTransformationMatrix(self):
+        '''
+        :return: 4x4 row-major transformation matrix with first index down rows, second across columns,
+        suitable for multiplication p' = Mp where p = [ x, y, z, h ].
+        '''
+        # apply transformation in order: scale then rotation then translation
+        if not all((v == 0.0) for v in self._rotation):
+            rotationMatrix = euler_to_rotation_matrix(self._rotation)
+            return [
+                [rotationMatrix[0][0]*self._scale, rotationMatrix[0][1]*self._scale, rotationMatrix[0][2]*self._scale, self._translation[0]],
+                [rotationMatrix[1][0]*self._scale, rotationMatrix[1][1]*self._scale, rotationMatrix[1][2]*self._scale, self._translation[1]],
+                [rotationMatrix[2][0]*self._scale, rotationMatrix[2][1]*self._scale, rotationMatrix[2][2]*self._scale, self._translation[2]],
+                [0.0, 0.0, 0.0, 1.0]]
+        if not (self._scale == 1.0 and all((v == 0.0) for v in self._translation)):
+            return [
+                [self._scale, 0.0, 0.0, self._translation[0]],
+                [0.0, self._scale, 0.0, self._translation[1]],
+                [0.0, 0.0, self._scale, self._translation[2]],
+                [0.0, 0.0, 0.0, 1.0]]
+        return identity_matrix(4)
+
     def _optimiseAlignment(self, pointMap):
         """
         Calculate transformation from modelCoordinates to dataMarkers
         over the markers, by scaling, translating and rotating model.
         On success, sets transformation parameters in object.
         :param pointMap: dict name -> (modelCoordinates, dataCoordinates)
         """
@@ -422,14 +443,15 @@
             "Align:  Failed to evaluate transformation for alignment to groups/markers"
 
         self._scale = unitScale * dataScale / modelScale
         rotationMatrix = euler_to_rotation_matrix(self._rotation)
         self._translation = sub(add(mult(unitTranslation, dataScale), dataCM),
                                 mult(matrix_vector_mult(rotationMatrix, modelCM), self._scale))
 
+
 def evaluate_field_mesh_integral(field: Field, coordinates: Field, mesh: Mesh, number_of_points=4):
     """
     Integrate value of a field over mesh using Gaussian Quadrature.
     :param field: Field to integrate over mesh.
     :param coordinates: Field giving spatial coordinates to integrate over.
     :param mesh: The mesh or mesh group to integrate over.
     :param number_of_points: Number of integration points in each dimension.
```

### Comparing `scaffoldfitter-0.6.0/src/scaffoldfitter/fitterstepconfig.py` & `scaffoldfitter-0.7.0/src/scaffoldfitter/fitterstepconfig.py`

 * *Files identical despite different names*

### Comparing `scaffoldfitter-0.6.0/src/scaffoldfitter/fitterstepfit.py` & `scaffoldfitter-0.7.0/src/scaffoldfitter/fitterstepfit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Fit step for gross alignment and scale.
 """
 
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.optimisation import Optimisation
-from opencmiss.zinc.result import RESULT_OK
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.optimisation import Optimisation
+from cmlibs.zinc.result import RESULT_OK
 from scaffoldfitter.fitterstep import FitterStep
 import sys
 
 
 class FitterStepFit(FitterStep):
 
     _jsonTypeId = "_FitterStepFit"
```

### Comparing `scaffoldfitter-0.6.0/src/scaffoldfitter.egg-info/PKG-INFO` & `scaffoldfitter-0.7.0/src/scaffoldfitter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: scaffoldfitter
-Version: 0.6.0
-Summary: Scaffold/model geometric fitting library using OpenCMISS-Zinc.
+Version: 0.7.0
+Summary: Scaffold/model geometric fitting library using Zinc.
 Home-page: https://github.com/ABI-Software/scaffoldfitter
 Author: Auckland Bioengineering Institute
 Author-email: r.christie@auckland.ac.nz
 License: Apache Software License
 Description: Scaffold Fitter
         ===============
         
-        Scaffold/model fitter using OpenCMISS-Zinc.
+        Scaffold/model fitter using Zinc.
         
         Install with the following command::
         
           pip install scaffoldfitter
```

### Comparing `scaffoldfitter-0.6.0/src/scaffoldfitter.egg-info/SOURCES.txt` & `scaffoldfitter-0.7.0/src/scaffoldfitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

