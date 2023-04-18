# Comparing `tmp/pyscos2000-0.1.0.tar.gz` & `tmp/pyscos2000-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscos2000-0.1.0.tar", last modified: Thu Feb 23 13:53:17 2023, max compression
+gzip compressed data, was "pyscos2000-0.2.0.tar", last modified: Tue Apr 18 06:43:22 2023, max compression
```

## Comparing `pyscos2000-0.1.0.tar` & `pyscos2000-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-02-23 13:53:17.187939 pyscos2000-0.1.0/
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1097 2023-02-23 13:34:11.000000 pyscos2000-0.1.0/LICENSE
--rw-r--r--   0 robertl   (1000) robertl   (1000)      700 2023-02-23 13:53:17.187939 pyscos2000-0.1.0/PKG-INFO
--rw-r--r--   0 robertl   (1000) robertl   (1000)      958 2023-02-23 13:33:27.000000 pyscos2000-0.1.0/README.md
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-02-23 13:53:17.187939 pyscos2000-0.1.0/pyscos2000/
--rw-r--r--   0 robertl   (1000) robertl   (1000)      653 2022-10-07 13:50:33.000000 pyscos2000-0.1.0/pyscos2000/__init__.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     2550 2022-10-05 07:22:54.000000 pyscos2000-0.1.0/pyscos2000/browser.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     3195 2022-10-04 10:09:36.000000 pyscos2000-0.1.0/pyscos2000/checker.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)    10518 2022-11-24 11:41:57.000000 pyscos2000-0.1.0/pyscos2000/concrete.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)    10180 2022-11-24 11:25:34.000000 pyscos2000-0.1.0/pyscos2000/instance.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     6327 2023-01-26 11:48:30.000000 pyscos2000-0.1.0/pyscos2000/parametertypes.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1203 2022-09-23 08:00:41.000000 pyscos2000-0.1.0/pyscos2000/reporter.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     8931 2023-02-16 14:32:02.000000 pyscos2000-0.1.0/pyscos2000/schema.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)    37245 2023-02-16 15:30:57.000000 pyscos2000-0.1.0/pyscos2000/scos2000.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1005 2022-10-07 13:50:15.000000 pyscos2000-0.1.0/pyscos2000/shared.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     2035 2022-09-23 08:09:36.000000 pyscos2000-0.1.0/pyscos2000/synthetic.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)       22 2022-08-16 13:11:39.000000 pyscos2000-0.1.0/pyscos2000/version.py
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-02-23 13:53:17.187939 pyscos2000-0.1.0/pyscos2000.egg-info/
--rw-r--r--   0 robertl   (1000) robertl   (1000)      700 2023-02-23 13:53:17.000000 pyscos2000-0.1.0/pyscos2000.egg-info/PKG-INFO
--rw-r--r--   0 robertl   (1000) robertl   (1000)      541 2023-02-23 13:53:17.000000 pyscos2000-0.1.0/pyscos2000.egg-info/SOURCES.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)        1 2023-02-23 13:53:17.000000 pyscos2000-0.1.0/pyscos2000.egg-info/dependency_links.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)       56 2023-02-23 13:53:17.000000 pyscos2000-0.1.0/pyscos2000.egg-info/entry_points.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)       29 2023-02-23 13:53:17.000000 pyscos2000-0.1.0/pyscos2000.egg-info/requires.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)       11 2023-02-23 13:53:17.000000 pyscos2000-0.1.0/pyscos2000.egg-info/top_level.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)      897 2023-02-23 13:53:17.187939 pyscos2000-0.1.0/setup.cfg
--rw-r--r--   0 robertl   (1000) robertl   (1000)       38 2022-08-16 13:42:40.000000 pyscos2000-0.1.0/setup.py
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-02-23 13:53:17.187939 pyscos2000-0.1.0/tests/
--rw-r--r--   0 robertl   (1000) robertl   (1000)     3904 2022-10-05 13:55:31.000000 pyscos2000-0.1.0/tests/test_capcalib.py
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-04-18 06:43:22.574742 pyscos2000-0.2.0/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1097 2023-02-23 13:34:11.000000 pyscos2000-0.2.0/LICENSE
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1699 2023-04-18 06:43:22.574742 pyscos2000-0.2.0/PKG-INFO
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      958 2023-02-23 13:33:27.000000 pyscos2000-0.2.0/README.md
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-04-18 06:43:22.571408 pyscos2000-0.2.0/pyscos2000/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      653 2022-10-07 13:50:33.000000 pyscos2000-0.2.0/pyscos2000/__init__.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     2550 2022-10-05 07:22:54.000000 pyscos2000-0.2.0/pyscos2000/browser.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     3195 2022-10-04 10:09:36.000000 pyscos2000-0.2.0/pyscos2000/checker.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    10518 2022-11-24 11:41:57.000000 pyscos2000-0.2.0/pyscos2000/concrete.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    10646 2023-04-18 06:43:13.000000 pyscos2000-0.2.0/pyscos2000/instance.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     6327 2023-01-26 11:48:30.000000 pyscos2000-0.2.0/pyscos2000/parametertypes.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1203 2022-09-23 08:00:41.000000 pyscos2000-0.2.0/pyscos2000/reporter.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    11907 2023-04-18 06:43:13.000000 pyscos2000-0.2.0/pyscos2000/schema.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    48311 2023-04-18 06:43:13.000000 pyscos2000-0.2.0/pyscos2000/scos2000.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1005 2022-10-07 13:50:15.000000 pyscos2000-0.2.0/pyscos2000/shared.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     2035 2022-09-23 08:09:36.000000 pyscos2000-0.2.0/pyscos2000/synthetic.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       21 2023-04-18 06:43:13.000000 pyscos2000-0.2.0/pyscos2000/version.py
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-04-18 06:43:22.574742 pyscos2000-0.2.0/pyscos2000.egg-info/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1699 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/PKG-INFO
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      541 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/SOURCES.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)        1 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/dependency_links.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       56 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/entry_points.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       29 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/requires.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       11 2023-04-18 06:43:22.000000 pyscos2000-0.2.0/pyscos2000.egg-info/top_level.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      977 2023-04-18 06:43:22.574742 pyscos2000-0.2.0/setup.cfg
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       38 2022-08-16 13:42:40.000000 pyscos2000-0.2.0/setup.py
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-04-18 06:43:22.574742 pyscos2000-0.2.0/tests/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     3845 2023-04-17 14:14:58.000000 pyscos2000-0.2.0/tests/test_capcalib.py
```

### Comparing `pyscos2000-0.1.0/LICENSE` & `pyscos2000-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/README.md` & `pyscos2000-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/pyscos2000/__init__.py` & `pyscos2000-0.2.0/pyscos2000/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/pyscos2000/browser.py` & `pyscos2000-0.2.0/pyscos2000/browser.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/pyscos2000/checker.py` & `pyscos2000-0.2.0/pyscos2000/checker.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/pyscos2000/concrete.py` & `pyscos2000-0.2.0/pyscos2000/concrete.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/pyscos2000/instance.py` & `pyscos2000-0.2.0/pyscos2000/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,20 @@
         return self.column.is_key
 
     @property
     def type(self):
         """The column type of this cell"""
         return self.column.type
 
+    def __len__(self):
+        if len(self.rawvalue) == 0:
+            return 0
+
+        return len(self._value)
+
     def __eq__(self, other):
         if isinstance(other, TableCell):
             return self._value == other._value
         if isinstance(other, type(self._value)):
             return self._value == other
         raise ValueError(f"{type(other).__name__} not comparable to {type(self._value)}")
 
@@ -159,23 +165,31 @@
 
     def find(self, values):
         """Return a list of all matching rows given these ``values``
 
         - ``values`` can be a tuple or list to match against the columns in order,
         - ``values`` can also be a dictionary to match the respective named column
           against the given value
+
+        In both use-cases the values may also be of type TableCell.
         """
         if isinstance(values, dict):
             for row in self.rows:
-                matches = all(sval == row[name].value
+                matches = all(sval.value == row[name].value
+                              if isinstance(sval, self.CELL_TYPE)
+                              else sval == row[name].value
                               for name, sval in values.items())
                 if matches:
                     yield row
 
         if isinstance(values, (tuple, list)):
+            values = [v.value
+                      if isinstance(v, self.CELL_TYPE)
+                      else v
+                      for v in values]
             for row in self.rows:
                 matches = all(value == row[idx].value
                               for idx, value in enumerate(values))
                 if matches:
                     yield row
 
     def parse(self):
@@ -313,8 +327,8 @@
     """CSV dialect for SCOS-style ``.dat`` files"""
     delimiter = '\t'
     doublequote = False
     escapechar = None
     lineterminator = '\r\n'
     quoting = csv.QUOTE_NONE
     skipinitialspace = False
-    strict = True
+    strict = True
```

### Comparing `pyscos2000-0.1.0/pyscos2000/parametertypes.py` & `pyscos2000-0.2.0/pyscos2000/parametertypes.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/pyscos2000/reporter.py` & `pyscos2000-0.2.0/pyscos2000/reporter.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/pyscos2000/schema.py` & `pyscos2000-0.2.0/pyscos2000/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 class PacketHeaderElementType(enum.Enum):
     FIXED = 'F'
     APID = 'A'
     SERVICETYPE = 'T'
     SERVICESUBTYPE = 'S'
     ACK = 'K'
     OTHER = 'P'
+    UNDEF1 = 'O'  # found in the wild
 
 
 class Plannable(enum.Enum):
     ALL = 'A'
     FLIGHTDYNAMICS = 'F'
     SOC = 'S'
     NOT = 'N'
@@ -185,14 +186,120 @@
     BINARY = 'B'
     OCTAL = 'O'
     DECIMAL = 'D'
     HEXADECIMAL = 'H'
     NORMAL = 'N'
 
 
+class TimeTagType(enum.Enum):
+    YES = 'Y'
+    NONE = 'N'
+    ONBOARD = 'B'
+
+
+class PlannableBySource(enum.Enum):
+    ALL = 'A'
+    FLIGHT_DYNAMICS = 'F'
+    SOC = 'S'
+    NOT_PLANNABLE = 'N'
+
+
+class StandaloneExecution(enum.Enum):
+    ALLOWED = 'Y'
+    NOT_ALLOWED = 'N'
+
+
+class SequenceElementType(enum.Enum):
+    COMMAND = 'C'
+    SEQUENCE = 'S'
+    COMMENT = 'T'
+    FPARAM_COMMAND = 'F'
+    FPARAM_SEQUENCE = 'P'
+
+
+class ReleaseTimeType(enum.Enum):
+    RELATIVE_PREVIOUS = 'R'
+    RELATIVE_START = 'A'
+
+
+class RelativePosition(enum.Enum):
+    START = 'S'
+    MIDDLE = 'M'
+    END = 'E'
+
+
+class CommandSequenceInterlock(enum.Enum):
+    GLOBAL = 'G'
+    LOCAL = 'L'
+    SUBSYSTEM = 'S'
+    BELONG = 'B'
+    LOCALFAILURE = 'F'
+    SUBSYSTEMFAILURE = 'T'
+    NONE = 'N'
+
+
+class CommandValueRepresentation(enum.Enum):
+    RAW = 'R'
+    ENGINEERING = 'E'
+    DEFAULT = 'D'
+    DYNAMIC_DEFAULT = 'T'
+
+
+class ValueEditable(enum.Enum):
+    """Whether the parameter value of a sequence element parameter is modifiable
+    after after loading it onto the stack
+
+    SDF_FTYPE field of SDF table
+    """
+    EDITABLE = 'E'
+    FIXED = 'F'
+
+    def __bool__(self):
+        return self == ValueEditable.EDITABLE
+
+
+class ValueSource(enum.Enum):
+    """Command sequence element parameter source
+
+    SDF_VTYPE field of SDF table
+    """
+
+    RAW = 'R'
+    """Value is taken from SDF_VALUE and interpreted as raw"""
+
+    ENG = 'E'
+    """Value is taken from SDF_VALUE and interpreted as engineering"""
+
+    FORMAL = 'F'
+    ELEMENT = 'P'
+    SEQUENCE = 'S'
+
+    DEFAULT = 'D'
+    """For command parameters, the value should be taken from the default value"""
+
+
+class FormatParameterType(enum.Enum):
+    """Type of a command sequence formal parameter
+
+    CSP_TYPE field of CSP table"""
+    COMMAND = 'C'
+    SEQUENCE = 'S'
+    PARAMETER = 'P'
+
+
+class CommandElementType(enum.Enum):
+    """Command element type
+
+    CDF_ELTYPE field of CDF table
+    """
+    AREA = 'A'
+    FIXED = 'F'
+    EDITABLE = 'E'
+
+
 class TableColumnType:
     """The type of a column in an SCOS table definition"""
 
     def parse(self, text):
         """Parse the raw ``text`` and return the converted value"""
         if text is None:
             return None
@@ -344,14 +451,62 @@
 
 
 class DisplayFormatColumn(EnumColumnType):
     """Column for Display Format settings"""
     ENUM = DisplayFormat
 
 
+class TimeTagTypeColumn(EnumColumnType):
+    ENUM = TimeTagType
+
+
+class PlannableBySourceColumn(EnumColumnType):
+    ENUM = PlannableBySource
+
+
+class StandaloneExecutionColumn(EnumColumnType):
+    ENUM = StandaloneExecution
+
+
+class SequenceElementTypeColumn(EnumColumnType):
+    ENUM = SequenceElementType
+
+
+class ReleaseTimeTypeColumn(EnumColumnType):
+    ENUM = ReleaseTimeType
+
+
+class RelativePositionColumn(EnumColumnType):
+    ENUM = RelativePosition
+
+
+class CommandSequenceInterlockColumn(EnumColumnType):
+    ENUM = CommandSequenceInterlock
+
+
+class ValueEditableColumn(EnumColumnType):
+    ENUM = ValueEditable
+
+
+class ValueSourceColumn(EnumColumnType):
+    ENUM = ValueSource
+
+
+class FormatParameterTypeColumn(EnumColumnType):
+    ENUM = FormatParameterType
+
+
+class CommandElementTypeColumn(EnumColumnType):
+    ENUM = CommandElementType
+
+
+class CommandValueRepresentationColumn(EnumColumnType):
+    ENUM = CommandValueRepresentation
+
+
 class ColumnDefinition:
     """A column in an SCOS table definition"""
     def __init__(self,
                  name,
                  type_,
                  description="",
                  optional=False,
```

### Comparing `pyscos2000-0.1.0/pyscos2000/scos2000.py` & `pyscos2000-0.2.0/pyscos2000/scos2000.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     CalibrationCategoryColumn, EventPacketIndicator,
     EndianessColumn, OutputViewColumn, InterpolationColumn,
     ParameterNatureColumn, JustifyColumn, NumericFormatTypeColumn,
     RadixColumn, LimitInterpretationColumn, LimitTypeInterpretationColumn,
     MonitoringCheckFlagColumn, PacketHeaderElementTypeColumn, PlannableColumn,
     CommandVerificationColumn, CommandInputFormatColumn, CommandCategoryColumn,
     CommandInterlockColumn, DisplayFormatColumn, IntegerFormatTypeColumn,
+    TimeTagTypeColumn, PlannableBySourceColumn, StandaloneExecutionColumn,
+    SequenceElementTypeColumn, ReleaseTimeTypeColumn, RelativePositionColumn,
+    CommandSequenceInterlockColumn, ValueEditableColumn, CommandElementTypeColumn,
+    ValueSourceColumn, FormatParameterTypeColumn, CommandValueRepresentationColumn,
     )
 from .parametertypes import ParameterType, SignedIntegerParameter, UnsignedIntegerParameter
 from .synthetic import DynamicSyntheticParameter
 
 
 class SyntheticImplementationMissingError(RuntimeError):
     """Raised when the implementation of a synthetic parameter is missing"""
@@ -407,35 +411,262 @@
             ColumnDefinition('CPC_RADIX', RadixColumn(), optional=True, default='D'),
             ColumnDefinition('CPC_UNIT', String(4), optional=True),
             ColumnDefinition('CPC_CATEG', CommandCategoryColumn(), optional=True, default='N'),
             ColumnDefinition('CPC_PRFREF', String(10), optional=True),
             ColumnDefinition('CPC_CCAREF', String(10), optional=True),
             ColumnDefinition('CPC_PAFREF', String(10), optional=True),
             ColumnDefinition('CPC_INTER', OutputViewColumn(), optional=True, default='R'),
-            ColumnDefinition('CPC_DEFVAL', String(17), optional=True),
+            ColumnDefinition('CPC_DEFVAL', String(248), optional=True),
             ColumnDefinition('CPC_CORR', Boolean(), optional=True, default='Y'),
             ColumnDefinition('CPC_OBTIP', Number(5), optional=True, default='0'),
             ColumnDefinition('CPC_DESCR2', String(256), optional=True, default=''),
             ColumnDefinition('CPC_ENDIAN', EndianessColumn(), optional=True, default='B'),
             ])
 
 
+class CDFTable(TableDefinition):
+    """The cdf.dat table in SCOS
+
+    Command definition
+    """
+    def __init__(self):
+        super().__init__('cdf', [
+            ColumnDefinition('CDF_CNAME', String(8), optional=False, is_key=True),
+            ColumnDefinition('CDF_ELTYPE', CommandElementTypeColumn(), optional=False),
+            ColumnDefinition('CDF_DESCR', String(24), optional=True),
+            ColumnDefinition('CDF_ELLEN', Number(4), optional=False),
+            ColumnDefinition('CDF_BIT', Number(4), optional=False),
+            ColumnDefinition('CDF_GRPSIZE', Number(2), optional=True, default='0'),
+            ColumnDefinition('CDF_PNAME', String(8), optional=True),
+            ColumnDefinition('CDF_INTER', CommandValueRepresentationColumn(),
+                             optional=True, default='R'),
+            ColumnDefinition('CDF_VALUE', String(248), optional=True),
+            ColumnDefinition('CDF_TMID', String(8), optional=True),
+            ])
+
+
 class PTVTable(TableDefinition):
     """The ptv.dat table in SCOS
 
     Commands pre-transmission validation"""
     def __init__(self):
         super().__init__('ptv', [
             ColumnDefinition('PTV_CNAME', String(8), optional=False, is_key=True),
             ColumnDefinition('PTV_PARNAM', String(8), optional=False, is_key=True),
             ColumnDefinition('PTV_INTER', OutputViewColumn(), optional=True, default='R'),
             ColumnDefinition('PTV_VAL', String(17), optional=False),
             ])
 
 
+class CSFTable(TableDefinition):
+    """The csf.dat table in SCOS
+
+    Command sequence characteristics"""
+    def __init__(self):
+        super().__init__('csf', [
+            ColumnDefinition('CSF_NAME', String(8), optional=False, is_key=True),
+            ColumnDefinition('CSF_DESC', String(24), optional=False),
+            ColumnDefinition('CSF_DESC2', String(64), optional=True),
+            ColumnDefinition('CSF_IFTT', TimeTagTypeColumn(), optional=True, default='N'),
+            ColumnDefinition('CSF_NFPARS', Number(3), optional=True),
+            ColumnDefinition('CSF_ELEMS', Number(5), optional=True),
+            ColumnDefinition('CSF_CRITICAL', Boolean(), optional=True, default='N'),
+            ColumnDefinition('CSF_PLAN', PlannableBySourceColumn(), optional=True, default='N'),
+            ColumnDefinition('CSF_EXEC', StandaloneExecutionColumn(), optional=True, default='Y'),
+            ColumnDefinition('CSF_SUBSYS', Number(3), optional=True),
+            ColumnDefinition('CSF_GENTIME', String(17), optional=True),
+            ColumnDefinition('CSF_DOCNAME', String(32), optional=True),
+            ColumnDefinition('CSF_ISSUE', String(10), optional=True),
+            ColumnDefinition('CSF_DATE', String(17), optional=True),
+            ColumnDefinition('CSF_DEFSET', String(8), optional=True),
+            ColumnDefinition('CSF_SUBSCHEDID', Number(5), optional=True),
+            ])
+
+
+class CSSTable(TableDefinition):
+    """The css.dat table in SCOS
+
+    Command sequence definitions"""
+    def __init__(self):
+        super().__init__('css', [
+            ColumnDefinition('CSS_SQNAME', String(8), optional=False, is_key=True),
+            ColumnDefinition('CSS_COMM', String(32), optional=True),
+            ColumnDefinition('CSS_ENTRY', Number(5), optional=False),
+            ColumnDefinition('CSS_TYPE', SequenceElementTypeColumn(), optional=False),
+            ColumnDefinition('CSS_ELEMID', String(8), optional=True),
+            ColumnDefinition('CSS_NPARS', Number(3), optional=False),
+            ColumnDefinition('CSS_MANDISP', Boolean(), optional=True, default='N'),
+            ColumnDefinition('CSS_RELTYPE', ReleaseTimeTypeColumn(), optional=True, default='R'),
+            ColumnDefinition('CSS_RELTIME', String(12), optional=True),
+            ColumnDefinition('CSS_EXTIME', String(17), optional=True),
+            ColumnDefinition('CSS_PREVREL', ReleaseTimeTypeColumn(), optional=True, default='R'),
+            ColumnDefinition('CSS_GROUP', RelativePositionColumn(), optional=True),
+            ColumnDefinition('CSS_BLOCK', RelativePositionColumn(), optional=True),
+            ColumnDefinition('CSS_ILSCOPE', CommandSequenceInterlockColumn(), optional=True),
+            ColumnDefinition('CSS_ILSTAGE', CommandVerificationColumn(), optional=True),
+            ColumnDefinition('CSS_DYNPTV', Boolean(), optional=True, default='N'),
+            ColumnDefinition('CSS_STATPTV', Boolean(), optional=True, default='N'),
+            ColumnDefinition('CSS_CEV', Boolean(), optional=True, default='N'),
+            ])
+
+
+class SDFTable(TableDefinition):
+    """The sdf.dat table in SCOS
+
+    Command sequence element parameters"""
+    def __init__(self):
+        super().__init__('sdf', [
+            ColumnDefinition('SDF_SQNAME', String(8), optional=False, is_key=True),
+            ColumnDefinition('SDF_ENTRY', Number(5), optional=False, is_key=True),
+            ColumnDefinition('SDF_ELEMID', String(8), optional=False),
+            ColumnDefinition('SDF_POS', Number(4), optional=False, is_key=True),
+            ColumnDefinition('SDF_PNAME', String(8), optional=False, is_key=True),
+            ColumnDefinition('SDF_FTYPE', ValueEditableColumn(), optional=True, default='E'),
+            ColumnDefinition('SDF_VTYPE', ValueSourceColumn(), optional=False),
+            ColumnDefinition('SDF_VALUE', String(248), optional=True),
+            ColumnDefinition('SDF_VALSET', String(8), optional=True),
+            ColumnDefinition('SDF_REPPOS', Number(4), optional=True),
+            ])
+
+
+class CSPTable(TableDefinition):
+    """The csp.dat table in SCOS
+
+    Command sequence formal parameters"""
+    def __init__(self):
+        super().__init__('csp', [
+            ColumnDefinition('CSP_SQNAME', String(8), optional=False, is_key=True),
+            ColumnDefinition('CSP_FPQNAME', String(8), optional=False, is_key=True),
+            ColumnDefinition('CSP_FPNUM', Number(8), optional=False),
+            ColumnDefinition('CSP_DESCR', String(23), optional=True),
+            ColumnDefinition('CSP_PTC', Number(2), optional=False),
+            ColumnDefinition('CSP_PFC', Number(5), optional=False),
+            ColumnDefinition('CSP_DISPFMT', CommandInputFormatColumn(),
+                             optional=True, default='R'),
+            ColumnDefinition('CSP_RADIX', RadixColumn(), optional=True, default='D'),
+            ColumnDefinition('CSP_TYPE', FormatParameterTypeColumn(), optional=False),
+            ColumnDefinition('CSP_VTYPE', OutputViewColumn(), optional=True),
+            ColumnDefinition('CSP_DEFVAL', String(248), optional=True),
+            ColumnDefinition('CSP_CATEG', CommandCategoryColumn(),
+                             optional=True, default='N'),
+            ColumnDefinition('CSP_PRFREF', String(10), optional=True),
+            ColumnDefinition('CSP_CCAREF', String(10), optional=True),
+            ColumnDefinition('CSP_PAFREF', String(10), optional=True),
+            ColumnDefinition('CSP_UNIT', String(4), optional=True),
+            ])
+
+
+class PSTTable(TableDefinition):
+    """The pst.dat table in SCOS
+
+    Command/Sequence parameter sets"""
+    def __init__(self):
+        super().__init__('pst', [
+            ColumnDefinition('PST_NAME', String(8), optional=False, is_key=True),
+            ColumnDefinition('PST_DESCR', String(24), optional=True),
+            ])
+
+
+class PSVTable(TableDefinition):
+    """The psv.dat table in SCOS
+
+    Command/sequence parameter value sets"""
+    def __init__(self):
+        super().__init__('psv', [
+            ColumnDefinition('PSV_NAME', String(8), optional=False),
+            ColumnDefinition('PSV_PVSID', String(8), optional=False, is_key=True),
+            ColumnDefinition('PSV_DESCR', String(24), optional=True),
+            ])
+
+
+class CCATable(TableDefinition):
+    """The cca.dat table in SCOS
+
+    Command/Sequence Parameter (De-)calibration curves"""
+    def __init__(self):
+        super().__init__('cca', [
+            ColumnDefinition('CCA_NUMBR', String(10), optional=False, is_key=True),
+            ColumnDefinition('CCA_DESCR', String(24), optional=True),
+            ColumnDefinition('CCA_ENGFMT', NumericFormatTypeColumn(),
+                             optional=True, default='R'),
+            ColumnDefinition('CCA_RAWFMT', NumericFormatTypeColumn(),
+                             optional=True, default='U'),
+            ColumnDefinition('CCA_RADIX', RadixColumn(), optional=True, default='D'),
+            ColumnDefinition('CCA_UNIT', String(4), optional=True),
+            ColumnDefinition('CCA_NCURVE', Number(3), optional=True),
+            ])
+
+
+class CCSTable(TableDefinition):
+    """The ccs.dat table in SCOS
+
+    Command/Sequence Parameter (De-)calibration curve definitions"""
+    def __init__(self):
+        super().__init__('ccs', [
+            ColumnDefinition('CCS_NUMBR', String(10), optional=False, is_key=True),
+            ColumnDefinition('CCS_XVALS', String(248), optional=False, is_key=True),
+            ColumnDefinition('CCS_YVALS', String(248), optional=False, is_key=True),
+            ])
+
+
+class PAFTable(TableDefinition):
+    """The paf.dat table in SCOS
+
+    Command/Sequence Parameter Textual (De-)calibration"""
+    def __init__(self):
+        super().__init__('paf', [
+            ColumnDefinition('PAF_NUMBR', String(10), optional=False, is_key=True),
+            ColumnDefinition('PAF_DESCR', String(24), optional=True),
+            ColumnDefinition('PAF_RAWFMT', NumericFormatTypeColumn(),
+                             optional=True, default='U'),
+            ColumnDefinition('PAF_NALIAS', Number(3), optional=True),
+            ])
+
+
+class PASTable(TableDefinition):
+    """The pas.dat table in SCOS
+
+    Command/Sequence Parameter Textual (De-)calibration definition"""
+    def __init__(self):
+        super().__init__('pas', [
+            ColumnDefinition('PAS_NUMBR', String(10), optional=False, is_key=True),
+            ColumnDefinition('PAS_ALTXT', String(248), optional=False, is_key=True),
+            ColumnDefinition('PAS_ALVAL', String(248), optional=False, is_key=True),
+            ])
+
+
+class PRFTable(TableDefinition):
+    """The prf.dat table in SCOS
+
+    Command/Sequence Parameter range sets"""
+    def __init__(self):
+        super().__init__('prf', [
+            ColumnDefinition('PRF_NUMBR', String(10), optional=False, is_key=True),
+            ColumnDefinition('PRF_DESCR', String(24), optional=True),
+            ColumnDefinition('PRF_INTER', OutputViewColumn(), optional=True, default='R'),
+            ColumnDefinition('PRF_DSPFMT', CommandInputFormatColumn(),
+                             optional=True, default='R'),
+            ColumnDefinition('PRF_RADIX', RadixColumn(), optional=True, default='D'),
+            ColumnDefinition('PRF_NRANGE', Number(3), optional=True),
+            ColumnDefinition('PRF_UNIT', String(4), optional=True),
+            ])
+
+
+class PRVTable(TableDefinition):
+    """The prv.dat table in SCOS
+
+    Command/Sequence Parameter range values"""
+    def __init__(self):
+        super().__init__('prv', [
+            ColumnDefinition('PRV_NUMBR', String(10), optional=False, is_key=True),
+            ColumnDefinition('PRV_MINVAL', String(248), optional=False, is_key=True),
+            ColumnDefinition('PRV_MAXVAL', String(248), optional=True),
+            ])
+
+
 class SCOS:
     """An SCOS-2000 database instance
 
     This is your main entry point for the use of SCOS-2000 databases.
 
     To merge this SCOS-2000 database with another database (for example if
     you have an instrument’s database but also a separate database for the
@@ -526,33 +757,34 @@
             # TODO 'ppc': Table(self, PPCTable()).parse(),
             'tcp': Table(self, TCPTable()).parse(),
             'pcpc': Table(self, PCPCTable()).parse(),
             'pcdf': Table(self, PCDFTable()).parse(),
             'ccf': Table(self, CCFTable()).parse(),
             'dst': Table(self, DSTTable()).parse(),
             'cpc': Table(self, CPCTable()).parse(),
-            # TODO 'cdf': Table(self, CDFTable()).parse(),
+            'cdf': Table(self, CDFTable()).parse(),
             'ptv': Table(self, PTVTable()).parse(),
-            # TODO 'csf': Table(self, CSFTable()).parse(),
-            # TODO 'css': Table(self, CSSTable()).parse(),
-            # TODO 'csp': Table(self, CSPTable()).parse(),
+            'csf': Table(self, CSFTable()).parse(),
+            'css': Table(self, CSSTable()).parse(),
+            'sdf': Table(self, SDFTable()).parse(),
+            'csp': Table(self, CSPTable()).parse(),
             # TODO 'cvs': Table(self, CVSTable()).parse(),
             # TODO 'cve': Table(self, CVETable()).parse(),
             # TODO 'cvp': Table(self, CVPTable()).parse(),
-            # TODO 'pst': Table(self, PSTTable()).parse(),
-            # TODO 'psv': Table(self, PSVTable()).parse(),
+            'pst': Table(self, PSTTable()).parse(),
+            'psv': Table(self, PSVTable()).parse(),
             # TODO 'cps': Table(self, CPSTable()).parse(),
             # TODO 'pvs': Table(self, PVSTable()).parse(),
             # TODO 'psm': Table(self, PSMTable()).parse(),
-            # TODO 'cca': Table(self, CCATable()).parse(),
-            # TODO 'ccs': Table(self, CCSTable()).parse(),
-            # TODO 'paf': Table(self, PAFTable()).parse(),
-            # TODO 'pas': Table(self, PASTable()).parse(),
-            # TODO 'prf': Table(self, PRFTable()).parse(),
-            # TODO 'prv': Table(self, PRVTable()).parse(),
+            'cca': Table(self, CCATable()).parse(),
+            'ccs': Table(self, CCSTable()).parse(),
+            'paf': Table(self, PAFTable()).parse(),
+            'pas': Table(self, PASTable()).parse(),
+            'prf': Table(self, PRFTable()).parse(),
+            'prv': Table(self, PRVTable()).parse(),
             }
 
         self.synthetics = {}
         """The ``synthetics`` dictionary contains the definitions for all
         synthetic parameters. The key is the parameter's name, the value an
         instance of ``SyntheticParameterDefinition``."""
         self.synthetics_in_spid = {}
```

### Comparing `pyscos2000-0.1.0/pyscos2000/shared.py` & `pyscos2000-0.2.0/pyscos2000/shared.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/pyscos2000/synthetic.py` & `pyscos2000-0.2.0/pyscos2000/synthetic.py`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/pyscos2000.egg-info/SOURCES.txt` & `pyscos2000-0.2.0/pyscos2000.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyscos2000-0.1.0/setup.cfg` & `pyscos2000-0.2.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [metadata]
 name = pyscos2000
 version = attr: pyscos2000.version.__version__
 author = Robert Labudda
 author_email = robert.labudda@irf.se
 url = https://gitlab.irf.se/irf/pyscos2000
 description = Python SCOS-2000 parsing and checking
+long_description = file:README.md
+long_description_content_type = text/markdown
 license = MIT
 license_files = 
 	LICENSE
 keywords = 
 	SCOS-2000
 	ESA
 classifiers =
```

### Comparing `pyscos2000-0.1.0/tests/test_capcalib.py` & `pyscos2000-0.2.0/tests/test_capcalib.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,14 @@
 
 
 class CAPCalibTest(unittest.TestCase):
     def setUp(self):
         self.scos = SCOS(Path(__file__).parent / 'capcalib')
         self.scos.check()
 
-    def test_canary(self):
-        self.assertFalse(True)
-
     def test_simple1(self):
         """Test simple interpolation"""
         packet = TestablePacket(self.scos, 15,
                                 [('PCF01', b'\x05')])
         self.assertEqual(packet['PCF01'].raw, 5)
         self.assertEqual(packet['PCF01'].eng, 2.5)
```

