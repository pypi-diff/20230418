# Comparing `tmp/curveengine-1.0.0-py3-none-any.whl.zip` & `tmp/curveengine-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9586 bytes, number of entries: 10
--rw-r--r--  2.0 unx     6722 b- defN 23-Apr-15 01:11 curveengine.py
+Zip file size: 10087 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     6770 b- defN 23-Apr-18 01:53 curveengine.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 23:51 parsing/__init__.py
 -rw-r--r--  2.0 unx      454 b- defN 23-Apr-13 14:34 parsing/enums.py
--rw-r--r--  2.0 unx     4093 b- defN 23-Apr-18 00:03 parsing/others.py
--rw-r--r--  2.0 unx    13033 b- defN 23-Apr-15 00:43 parsing/parsers.py
+-rw-r--r--  2.0 unx     4557 b- defN 23-Apr-18 01:18 parsing/others.py
+-rw-r--r--  2.0 unx    14342 b- defN 23-Apr-18 01:49 parsing/parsers.py
 -rw-r--r--  2.0 unx    17797 b- defN 23-Apr-14 23:47 parsing/ratehelpers.py
--rw-r--r--  2.0 unx      327 b- defN 23-Apr-18 00:39 curveengine-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 00:39 curveengine-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Apr-18 00:39 curveengine-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      759 b- defN 23-Apr-18 00:39 curveengine-1.0.0.dist-info/RECORD
-10 files, 43297 bytes uncompressed, 8304 bytes compressed:  80.8%
+-rw-r--r--  2.0 unx      327 b- defN 23-Apr-18 01:54 curveengine-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 01:54 curveengine-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-18 01:54 curveengine-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      759 b- defN 23-Apr-18 01:54 curveengine-1.0.1.dist-info/RECORD
+10 files, 45118 bytes uncompressed, 8805 bytes compressed:  80.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: parsing/parsers.py
 Comment: 
 
 Filename: parsing/ratehelpers.py
 Comment: 
 
-Filename: curveengine-1.0.0.dist-info/METADATA
+Filename: curveengine-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: curveengine-1.0.0.dist-info/WHEEL
+Filename: curveengine-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: curveengine-1.0.0.dist-info/top_level.txt
+Filename: curveengine-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: curveengine-1.0.0.dist-info/RECORD
+Filename: curveengine-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## curveengine.py

```diff
@@ -26,15 +26,15 @@
         for curve in data['curves']:
             curveName = curve['curveName']
             tmpData[curveName] = curve
 
         dependencies = getDependencyList(data)
         sortedList = topologicalSort(dependencies)
         for curveName in sortedList:
-            parsed = parse(**tmpData[curveName])
+            parsed = parse(level=curveName,**tmpData[curveName])
             if curveName not in self.indexes.keys():
                 self.__buildIndexes(parsed)
             if curveName not in self.curves.keys():
                 self.__buildCurve(parsed)
 
     def __buildIndexes(self, data):
         name = data['curveName']
@@ -68,15 +68,15 @@
         self.indexes[curveName] = self.indexes[curveName].clone(
             self.curveHandles[curveName])
         self.curves[curveName] = curve
 
     def __buildPiecewiseCurve(self, data):
         rateHelpers = []
         config = data['curveConfig']
-        for rateHelper in config['rateHelpers']:
+        for i, rateHelper in enumerate(config['rateHelpers']):
             helperType = rateHelper['helperType']
             helperConfig = rateHelper['helperConfig']
             if 'discountCurve' not in helperConfig.keys():
                 helperConfig['discountCurve'] = None
             marketConfig = rateHelper['marketConfig']
             try:
                 if helperType == HelperType.Deposit:
@@ -106,19 +106,19 @@
                 elif helperType == HelperType.Bond:
                     helper = createFixedRateBondHelper(
                         helperConfig, marketConfig, self.curveHandles, self.indexes)
                 else:
                     raise Exception(
                         'Unknown rate helper type: {}'.format(helperType))
             except KeyError as e:
-                raise KeyError('Failed to create rate helper {helper} at curve {curveName}: Key not found: {error} '.format(
-                    helper=helperType, curveName=data['curveName'], error=e))
+                raise KeyError('Failed to create rate helper {helper}/{i} at curve {curveName}: Key not found: {error} '.format(
+                    helper=helperType, curveName=data['curveName'], error=e, i=i))
             except Exception as e:
-                raise Exception('Failed to create rate helper {helper} at curve {curveName}: {error} '.format(
-                    helper=helperType, curveName=data['curveName'], error=e))
+                raise Exception('Failed to create rate helper {helper}/{i} at curve {curveName}: {error} '.format(
+                    helper=helperType, curveName=data['curveName'], error=e, i=i))
             rateHelpers.append(helper)
 
         refDate = ore.Settings.instance().evaluationDate
         dayCounter = config['dayCounter']
 
         curve = ore.PiecewiseLogLinearDiscount(
             refDate, rateHelpers, dayCounter)
```

## parsing/others.py

```diff
@@ -56,58 +56,69 @@
     endOfMonth = indexConfig['endOfMonth']
     convention = indexConfig['convention']
     index = ore.IborIndex(name, tenor, fixingDays, currency,
                           calendar, convention, endOfMonth, dayCounter)
     return index
 
 
-
 def getDependencyList(data: dict) -> dict:
     """
-    Get the dependency list for the curves
+    Get the dependency list for the curves.
 
     Parameters
     ----------
     data : dict
-        Dictionary containing the curve data
+        Dictionary containing the curve data.
 
     Returns
     -------
     dict
-        Dictionary containing the dependency list
+        Dictionary containing the dependency list.
 
     Notes
     -----
     The dependency list is a dictionary with the curve name as key and a set of
     curve names as value. The set contains the names of the curves that the
     curve depends on.
     """
-    # possible curve related keys
+    # Possible curve related keys
     pc = ['discountCurve', 'collateralCurve']
-    # possible index related keys
+    # Possible index related keys
     pi = ['index', 'shortIndex', 'longIndex']
 
-    dependecies = {}
+    checkDictKeys(data, ['curves'], level='')
+
+    dependencies = {}
     for curve in data['curves']:
+        checkDictKeys(curve, ['curveName', 'curveConfig'], level='curves')
+
         curveName = curve['curveName']
-        if curveName not in dependecies.keys():
-            dependecies[curveName] = set()
+        if curveName not in dependencies.keys():
+            dependencies[curveName] = set()
 
         curveConfig = curve['curveConfig']
+        checkDictKeys(curveConfig, ['curveType',
+                      'rateHelpers'], level=r'{curve}\curves'.format(curve=curveName))
+
         curveType = CurveType(curveConfig['curveType'])
         if curveType == CurveType.Piecewise:
             for rateHelper in curveConfig['rateHelpers']:
-                config = rateHelper['helperConfig']
+                checkDictKeys(rateHelper, ['helperType', 'helperConfig'],
+                              level=r'{curve}\curves\rateHelpers'.format(curve=curveName))
+                helperConfig = rateHelper['helperConfig']
                 for key in pc:
-                    if key in config.keys():
-                        dependecies[curveName].add(config[key])
-                for key in pi:
-                    if key in config.keys():
-                        dependecies[curveName].add(config[key])
-    return dependecies
+                    if key in helperConfig:
+                        dependencies[curveName].add(helperConfig[key])
+                    for key in pi:
+                        if key in helperConfig:
+                            dependencies[curveName].add(helperConfig[key])
+    return dependencies
+
+
+
 
 
 def topologicalSort(dependencies):
     """
     Sort the dependency list topologically
 
     Parameters
```

## parsing/parsers.py

```diff
@@ -1,25 +1,59 @@
 import ORE as ore
 from parsing.enums import *
 
 
-def parse(**kwargs):
+def checkDictKeys(data: dict, keys: list, level: str = ''):
+    """
+    Check if all the keys are present in the dictionary.
+
+    Parameters
+    ----------
+    data : dict
+        The dictionary to be checked.
+    keys : list
+        A list of keys to be checked for presence.
+    level : str, optional
+        The level where the error occurred (default is '').
+
+    Raises
+    ------
+    KeyError
+        If any key is missing from the dictionary.
+    """
+    for key in keys:
+        try:
+            _ = data[key]
+        except KeyError:
+            raise KeyError(f"Missing key: '{key}' in {level}.")
+
+
+def parse(level, **kwargs):
     results = {}
     for key, value in kwargs.items():
+        level_key = level + '\\' + key
         if key in ['helperConfig', 'curveIndex', 'curveConfig']:
-            results[key] = parse(**value)
+            results[key] = parse(level=level_key, **value)
 
         elif key == 'nodes':
-            results[key] = [parseNode(v) for v in value]
+            try:
+                results[key] = [parseNode(v) for v in value]
+            except KeyError:
+                raise KeyError(
+                    f"Missing key: 'date' or 'rate' in {level_key}.")
+            except ValueError:
+                raise ValueError(
+                    f"Unable to parse item 'date' or 'rate' in {level_key}.")
 
         elif key == 'marketConfig':
-            results[key] = parseMarketConfig(value)
+            results[key] = parseMarketConfig(level_key, value)
 
         elif key in ['curves', 'rateHelpers']:
-            results[key] = [parse(**v) for v in value]
+            results[key] = [parse(level=level_key + '\\{}'.format(i), **v)
+                            for i, v in enumerate(value)]
 
         elif key in ['date', 'startDate', 'endDate']:
             results[key] = parseDate(value)
 
         elif key == 'helperType':
             results[key] = HelperType(value)
 
@@ -61,21 +95,23 @@
             if isinstance(value, int):
                 results[key] = value
             else:
                 raise ValueError(
                     'unable to parse item {0} with value {1}'.format(key, value))
 
         elif key in ['discountCurve', 'index', 'shortIndex', 'longIndex', 'curveName']:
+            checkDictKeys(kwargs, [key], level=level_key)
             if isinstance(value, str):
                 results[key] = value
             else:
                 raise ValueError(
                     'unable to parse item {0} with value {1}'.format(key, value))
 
         elif key in ['couponRate']:
+            checkDictKeys(kwargs, [key], level=level_key)
             if isinstance(value, float):
                 results[key] = value
             else:
                 raise ValueError(
                     'unable to parse item {0} with value {1}'.format(key, value))
 
         elif key == 'month':
@@ -83,30 +119,32 @@
 
         else:
             results[key] = value
 
     return results
 
 
-def parseMarketConfig(marketConfig):
+def parseMarketConfig(level, marketConfig):
     results = {}
     if isinstance(marketConfig, dict):
         for key, value in marketConfig.items():
             if key in ['spread', 'fxSpot', 'fxPoints', 'price']:
                 if isinstance(value, float):
                     results[key] = value
                 elif isinstance(value, dict):
+                    checkDictKeys(value, ['value'], level=level)
                     results[key] = value['value']
                 else:
                     raise ValueError(
                         'unable to parse item in market config {0} with value {1}'.format(key, value))
             elif key == 'rate':
                 if isinstance(value, float):
                     results[key] = value
                 elif isinstance(value, dict):
+                    checkDictKeys(value, ['value'], level=level)
                     results[key] = value['value']
                 else:
                     raise ValueError(
                         'unable to parse item in market config {0} with value {1}'.format(key, value))
 
     else:
         raise NotImplementedError(
```

