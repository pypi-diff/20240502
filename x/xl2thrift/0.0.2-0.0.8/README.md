# Comparing `tmp/xl2thrift-0.0.2.tar.gz` & `tmp/xl2thrift-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xl2thrift-0.0.2.tar", last modified: Tue Apr 23 13:13:54 2024, max compression
+gzip compressed data, was "xl2thrift-0.0.8.tar", last modified: Thu May  2 18:16:36 2024, max compression
```

## Comparing `xl2thrift-0.0.2.tar` & `xl2thrift-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:13:54.385543 xl2thrift-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-23 13:13:54.385543 xl2thrift-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:13:54.385543 xl2thrift-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:13:54.381543 xl2thrift-0.0.2/xl2thrift/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/xl2thrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/xl2thrift/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-04-23 13:13:51.000000 xl2thrift-0.0.2/xl2thrift/thriftExcelTools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:13:54.381543 xl2thrift-0.0.2/xl2thrift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 13:13:54.000000 xl2thrift-0.0.2/xl2thrift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:16:36.855014 xl2thrift-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-02 18:16:36.851014 xl2thrift-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:16:36.855014 xl2thrift-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:16:36.851014 xl2thrift-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/tests/test_usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:16:36.851014 xl2thrift-0.0.8/xl2thrift/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/xl2thrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/xl2thrift/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/xl2thrift/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/xl2thrift/mutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/xl2thrift/mutate_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16564 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/xl2thrift/thriftExcelTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/xl2thrift/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-02 18:16:33.000000 xl2thrift-0.0.8/xl2thrift/validate_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:16:36.851014 xl2thrift-0.0.8/xl2thrift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-02 18:16:36.000000 xl2thrift-0.0.8/xl2thrift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-02 18:16:36.000000 xl2thrift-0.0.8/xl2thrift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:16:36.000000 xl2thrift-0.0.8/xl2thrift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-02 18:16:36.000000 xl2thrift-0.0.8/xl2thrift.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:16:36.000000 xl2thrift-0.0.8/xl2thrift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 18:16:36.000000 xl2thrift-0.0.8/xl2thrift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 18:16:36.000000 xl2thrift-0.0.8/xl2thrift.egg-info/top_level.txt
```

### Comparing `xl2thrift-0.0.2/LICENSE` & `xl2thrift-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xl2thrift-0.0.2/PKG-INFO` & `xl2thrift-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl2thrift
-Version: 0.0.2
+Version: 0.0.8
 Summary: Converts xlsx files into thrift files that can be deserialized in many programming languages
 Home-page: http://github.com/ohthepain/xl2thrift
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: thrift config
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xl2thrift-0.0.2/README.rst` & `xl2thrift-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `xl2thrift-0.0.2/setup.py` & `xl2thrift-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='xl2thrift',
-      version='0.0.2',
+      version='0.0.8',
       description='Converts xlsx files into thrift files that can be deserialized in many programming languages',
       long_description='Uses thrift-generated python reflection classes to match spreadsheet data with your thrift file. You can then load the resulting blob in any language supported by thrift.',
       long_description_content_type='text/x-rst',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
@@ -22,11 +22,13 @@
             'thrift',
             'argparse',
             'datetime',
       ],
       entry_points = {
         'console_scripts': [
           'xl2thrift=xl2thrift.command_line:main',
+          'mutate=xl2thrift.mutate_cmd:mutateThriftBlob',
+          'validate=xl2thrift.validate_cmd:validateThriftBlob',
         ],
       },
       zip_safe=False)
```

### Comparing `xl2thrift-0.0.2/xl2thrift/thriftExcelTools.py` & `xl2thrift-0.0.8/xl2thrift/thriftExcelTools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import sys, os
 import importlib
-import argparse
 import datetime
+import glob
 
 import thrift
 from thrift.transport import TTransport
 from thrift.Thrift import TType
 from openpyxl import Workbook
 from openpyxl import load_workbook
 import openpyxl
 
+from .exceptions import EnumException, ThriftGeneratedModuleException, FileNotFoundException
+
 def Log(s):
-	if args.verbose:
+	verbose = globals()['verbose']
+	if verbose:
 	 	print(s)
 
 def stringToName(s):
 	name = s.split("--", 1)[0].strip().replace(" ", "")
 	return name[0].lower() + name[1:]
 
 class SheetColumnEntry:
 	title = None
 	attributeName = None
 	columnNum = 0
 	def __init__(self, cnum, topcell):
 		self.title = topcell
 		self.attributeName = stringToName(topcell)
 		self.columnNum = cnum
-		#self.dump()
-	def dump(self):
-		Log("SheetColumnEntry for column %d has attributeName %s (%s)" % (self.columnNum, self.attributeName, self.title))
+	# 	self.dump()
+	# def dump(self):
+	# 	if globals()['verbose']:
+	# 		print("SheetColumnEntry for column %d has attributeName %s (%s)" % (self.columnNum, self.attributeName, self.title))
 
 class SheetInfo:
 	title = None
 	tablename = None
 	columnInfo = None
 	numcolumns = 0
 	def __init__(self, sheet):
@@ -53,23 +57,25 @@
 					c += 1
 			checkdupes = {}
 			for c in self.columnInfo:
 				columnInfo = self.columnInfo[c]
 				if columnInfo.attributeName in checkdupes:
 					print('WARNING: Sheet <%s> has duplicate columns for <%s>' % (sheet.title, columnInfo.attributeName))
 				checkdupes[columnInfo.attributeName] = 1
+		self.dump()
 
 	def dump(self):
-		print("++++++++++++++++++++++++++++++")
-		print(("SheetInfo (%s) -> table %s" % (self.title, self.tablename)))
-		for c in range(1,len(self.columnInfo) + 1):
-			columnInfo = self.columnInfo[c]
-			if columnInfo != None:
-				print(("	column %d: column %d attribute name %s" % (c, columnInfo.columnNum, columnInfo.attributeName)))
-		print("++++++++++++++++++++++++++++++")
+		if (globals()['verbose']):
+			print("++++++++++++++++++++++++++++++")
+			print(("SheetInfo (%s) -> table %s" % (self.title, self.tablename)))
+			for c in range(1,len(self.columnInfo) + 1):
+				columnInfo = self.columnInfo[c]
+				if columnInfo != None:
+					print(("	column %d: cattribute name %s" % (c, columnInfo.attributeName)))
+			print("++++++++++++++++++++++++++++++")
 
 # type info for a field in the Data class
 # if it's a container type then it's "of" value type.
 class TypeEntry:
 	type = None
 	name = None
 	mapIndexType = None
@@ -101,48 +107,41 @@
 					self.valueType = spec[3][0]
 				else:
 					self.valueType = spec[3][1][0]
 					# this constructs the object
 					#new_object = self.valueType()
 			elif self.containerType == TType.STRUCT:
 				self.valueType = spec[3][0]
-			#self.dump()
+			self.dump()
 	def dump(self):
-		print(("TypeEntry: %s in Data[%d], self.valueType %s" % (self.name, self.fieldNum, self.valueType)))
+		if (globals()['verbose']):
+			print(("TypeEntry: %s in Data[%d], self.valueType %s" % (self.name, self.fieldNum, self.valueType)))
 
 def makeTypeEntries(Data):
 	typeEntries = {}
 	for spec in Data.thrift_spec:
 		typeEntry = TypeEntry(spec)
 		if typeEntry != None:
 			typeEntries[typeEntry.name] = typeEntry
 	return typeEntries
 
-def old_countActiveColumns(sheet):
-	count = 0
-	for col in range(1, 100):
-		value = sheet.cell(1, col).value
-		#print('countActiveColumns - value %s' %(value))
-		if value != None:
-			#print('countActiveColumns - %d columns' %(col-1))
-			return col-1
-
 def	countActiveColumns(sheet):
 	count = 0
 	# note max_row = 1 here
 	#row = sheet[1]
 	for row in sheet.iter_rows(min_row=1, min_col=1, max_row=1, max_col=1000):
 		for cell in row:
 			##print('countActiveColumns - content %s' %(cell.value))
 			if cell.value == None:
 				##print('countActiveColumns - count %s' %(count))
 				return count
 			count += 1
 
 def getRowObject(sheetInfo, row, columnFieldSpec):
+	enums = globals()['enums']
 	if len(row) == 0 or row[0].value == None:
 		return
 	tablename = sheetInfo.tablename
 	typeEntry = typeEntries[tablename]
 	numcolumns = sheetInfo.numcolumns
 	if typeEntry.valueType == 'UTF8':
 		return row[0].value
@@ -155,16 +154,17 @@
 		for cell in row:
 			info = sheetInfo.columnInfo[column]
 			value = cell.value
 			if value != None:
 				enumClass = None
 				enumLookup = typeEntry.valueType.__name__ + '.' + info.attributeName
 				if enumLookup in enums:
-					enumClassName = enums[enumLookup]
-					enumClass = getattr(ConfigModule, enumClassName)
+					enumClass = getEnumClass(enumLookup)
+					# enumClassName = enums[enumLookup]
+					# enumClass = getattr(ConfigModule, enumClassName)
 
 				if column in columnFieldSpec:
 					containerType = columnFieldSpec[column][1]
 					if containerType == TType.STRUCT:
 						fieldType = columnFieldSpec[column][3][0]
 						if fieldType.__name__ == "DateTimeUTC":
 							msec = int((value - datetime.datetime(1970,1,1)).total_seconds()) * 1000
@@ -203,27 +203,31 @@
 							else:
 								value = value.split(',')
 								for v in value:
 									if v != v.strip():
 										print(("WARNING: the string '%s' has leading/trailing spaces" % (v)))
 
 				elif enumClass != None:
-					value = enumClass._NAMES_TO_VALUES[value]
+					try:
+						value = enumClass._NAMES_TO_VALUES[value]
+					except:
+						raise EnumException('ERROR: undefined enum value <%s>' % (value))
 			# get member for column
 			info = sheetInfo.columnInfo[column]
 			setattr(new_object, info.attributeName, value)
 			column += 1
 			if column > numcolumns:
 				break
 		new_object.validate()
 	return new_object
 
 def parseSheet(sheet):
 	sheetInfo = SheetInfo(sheet)
 	numcolumns = sheetInfo.numcolumns
+	enums = globals()['enums']
 	#sheetInfo.dump()
 	tablename = stringToName(sheet.title)
 	if not tablename in typeEntries:
 		Log('Ignore table <%s>' % (tablename))
 	if tablename in typeEntries:
 		Log("parseSheet " + sheet.title + " with tablename " + tablename)
 		typeEntry = typeEntries[tablename]
@@ -298,16 +302,17 @@
 								subValueType = fieldSpec[3][0]
 								valueStrings = attrvalue.split(',')
 								value = []
 								for v in valueStrings:
 									if subValueType == TType.I32:
 										enumLookup = typeEntry.valueType.__name__ + '.' + fieldSpec[2]
 										if enumLookup in enums:
-											enumClassName = enums[enumLookup]
-											enumClass = getattr(ConfigModule, enumClassName)
+											enumClass = getEnumClass(enumLookup)
+											# enumClassName = enums[enumLookup]
+											# enumClass = getattr(ConfigModule, enumClassName)
 											value.append(enumClass._NAMES_TO_VALUES[v])
 										else:
 											value.append(int(v))
 									elif subValueType == TType.DOUBLE:
 										value.append(float(v))
 									else:
 										value.append(v)
@@ -341,129 +346,135 @@
 			rownum += 1
 
 		if typeEntry.containerType == TType.STRUCT:
 			table = new_object
 			new_object.validate()
 
 def parseEnums(path):
-	with open(path) as myfile:
-		for line in myfile:
-			name, var = line.split("=")
-			enums[name.strip()] = var.strip()
+	try:
+		with open(path) as myfile:
+			for line in myfile:
+				name, var = line.split("=")
+				enums[name.strip()] = var.strip()
+	except:
+		raise FileNotFoundException('Enums file <%s> not found' % (path))
+	return enums
+
+def getEnumClass(enumLookup):
+	ConfigModule = globals()['ConfigModule']
+	enumClassName = enums[enumLookup]
+	enumClass = getattr(ConfigModule, enumClassName)
+	return enumClass
 
 def parseWorkbook(workbook):
 	for sheet in workbook:
 		parseSheet(sheet)
 
 def parseFile(path):
 	Log('========== Workbook %s ============' % (path))
 	workbook = load_workbook(path, read_only = True, data_only = True)
 	parseWorkbook(workbook)
 
-def ensureDir(file_path):
-    directory = os.path.dirname(file_path)
-    if not os.path.exists(directory):
-        os.makedirs(directory)
-		
 def usage():
 	print('--gen_py should point to your thrift-generated python source folder')
 	print('    i.e, the folder generated by `thrift --gen py <thriftfile>')
 	print('--namespace is the namespace in your thrift file')
 	print('--class_name is the class in your thrift file that contains all the data')
 	print('--verbose for more output')
 	print('--enums coming soon')
 
 # Globals
 typeEntries = {}
 Data = {}
 enums = {}
 args = {}
 
-def convertXlsx():
-
-	parser = argparse.ArgumentParser(description='Excel converter')
-	parser.add_argument('--namespace', help='namespace from thrift file', required=True)
-	parser.add_argument('--thrift_protocol', choices=('TCompactProtocol', 'TJSONProtocol', 'TBinaryProtocol'), default='TJSONProtocol', required=True)
-	parser.add_argument('--gen_py', default='', help="location of thrift-generated python source folder (thrift --gen py <thriftfile>)", required=True)
-	parser.add_argument('--output', default='config.bin', required=False, help="where to save output")
-	parser.add_argument('--class_name', default='Data', help="name of the class (without namespace) in your thrift file that contains all the data")
-	parser.add_argument('--verbose', action='store_true', help="show detailed output")
-	parser.add_argument('--enums', action='store_true', help="name of text file that stores a list of enums (coming soon)")
-	parser.add_argument('--release', action='store_true', help='do not process folders ending with Debug')
-
-	try:
-		globals()['args'] = parser.parse_args()
-	except IOError as msg:
-		parser.error(str(msg))
-		usage()
-
-	Log('Hi from convertXlsx: Loading <%s> from: <%s>' % (args.namespace, args.gen_py))
-
-	sys.path.append('%s' % (args.gen_py))
+def list_matching_files(glob_patterns):
+    matched_files = []
+    for pattern in glob_patterns.split():
+        matched_files.extend(glob.glob(pattern))
+    return matched_files
+
+def convertXlsxToThrift(patterns, namespace, thrift_protocol, gen_py, class_name='Data', output='config.bin', enums_path=None, release=False, verbose=False):
+	globals()['verbose'] = verbose
+	sys.path.append(gen_py)
 	ConfigModule = {}
 	try:
-		ConfigModule = importlib.import_module('%s.ttypes' % (args.namespace))
+		ConfigModule = importlib.import_module('%s.ttypes' % (namespace))
 	except:
-		print('Failed to load thrift-generated module (%s.ttypes)' % (args.namespace))
-		print('Check that the namespace in your thrift file matches the --namespace arg (%s)' % (args.namespace))
-		print('and that the --gen_py arg (%s) points to the correct folder' % (args.gen_py))
-		exit()
+		print('Failed to load thrift-generated module (%s.ttypes)' % (namespace))
+		print('Check that the namespace in your thrift file matches the --namespace arg (%s)' % (namespace))
+		print('and that the --gen_py arg (%s) points to the correct folder' % (gen_py))
+		raise ThriftGeneratedModuleException('Failed to load thrift-generated module in <%s> called (%s.ttypes)' % (gen_py, namespace))
 
+	sys.path.remove(gen_py)
 	Log(ConfigModule)
+	globals()['ConfigModule'] = ConfigModule
 
 	try:
-		dataClass = getattr(ConfigModule, args.class_name)
+		dataClass = getattr(ConfigModule, class_name)
 	except:
-		print('Failed create an instance of class (%s) specified in the --class_name arg' % (args.class_name))
 		print('Please make sure that your --class_name arg refers to the correct class in your thrift file (and in the source code in --gen_py)')
-		exit()
+		raise FileNotFoundException('Failed create an instance of class (%s) specified in the --class_name arg' % (class_name))
 
 	globals()['Data'] = dataClass()
 	Data = globals()['Data']
 
 	sheetInfo = None
 
-	if args.enums:
-		globals()['enums'] = parseEnums(enums)
+	if enums_path:
+		globals()['enums'] = parseEnums(enums_path)
 	globals()['typeEntries'] = makeTypeEntries(Data)
 
-	for root, dirs, files in os.walk("."):
-		for file_ in files:
-			if file_[:2] != "~$" and file_[:2] != "--" and file_.lower().endswith(".xlsx"):
-				if not file_.lower().endswith("!.xlsx"):
-					parseFile(os.path.join(root, file_))
-
-
-	for root, dirs, files in os.walk("."):
-		for file_ in files:
-			if file_[:2] != "~$" and file_[:2] != "--" and file_.lower().endswith(".xlsx"):
-				if not args.release and file_.endswith('!.xlsx'):
-					print(('Including debug workbook %s' % (file_)))
-					parseFile(os.path.join(root, file_))
+	filenames = list_matching_files(patterns)
+	for path in filenames:
+		file_ = os.path.basename(path)
+		if file_[:2] != "~$" and file_[:2] != "--" and file_.lower().endswith(".xlsx"):
+			if not file_.lower().endswith("!.xlsx"):
+				parseFile(path)
+
+	# Debug sheets are added last so that they can overwrite 
+	for path in filenames:
+		file_ = os.path.basename(path)
+		if file_[:2] != "~$" and file_[:2] != "--" and file_.lower().endswith(".xlsx"):
+			if not release and file_.endswith('!.xlsx'):
+				parseFile(path)
+
+	# for pattern in patterns:
+	# 	for path in glob.glob(pattern, recursive=True):
+	# 		file_ = os.path.basename(path)
+	# 		if file_[:2] != "~$" and file_[:2] != "--" and file_.lower().endswith(".xlsx"):
+	# 			if not file_.lower().endswith("!.xlsx"):
+	# 				parseFile(path)
+
+	# Debug sheets are added last so that they can overwrite 
+	# for pattern in patterns:
+	# 	for path in glob.glob(pattern, recursive=True):
+	# 		file_ = os.path.basename(path)
+	# 		if file_[:2] != "~$" and file_[:2] != "--" and file_.lower().endswith(".xlsx"):
+	# 			if not release and file_.endswith('!.xlsx'):
+	# 				parseFile(path)
 
 	transport = TTransport.TMemoryBuffer()
-	ThriftProtocol = getattr(importlib.import_module("thrift.protocol.%s" % (args.thrift_protocol)), args.thrift_protocol)
+	ThriftProtocol = getattr(importlib.import_module("thrift.protocol.%s" % (thrift_protocol)), thrift_protocol)
 	protocol = ThriftProtocol(transport)
 	Data.schemaVersionId = 1
 	Data.write(protocol)
 
 	# Write output file
-	configPath = args.output
+	configPath = output
 	buf = transport.getvalue()
 	with open(configPath, 'wb') as f:
 		f.write(buf)
 
 	# Read and validate
 	buf = None
 
 	with open(configPath, 'rb') as f:
 		buf = f.read()
 
 	transport = TTransport.TMemoryBuffer(buf)
 	protocol = ThriftProtocol(transport)
 	Data = None
-	Data = ConfigModule.ConfigData()
+	Data = dataClass()
 	Data.read(protocol)
-	Data.validate()
-
-if __name__ == '__main__':
-    convertXlsx()
+	return Data.validate()
```

### Comparing `xl2thrift-0.0.2/xl2thrift.egg-info/PKG-INFO` & `xl2thrift-0.0.8/xl2thrift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl2thrift
-Version: 0.0.2
+Version: 0.0.8
 Summary: Converts xlsx files into thrift files that can be deserialized in many programming languages
 Home-page: http://github.com/ohthepain/xl2thrift
 Author: Paul Wilkinson
 Author-email: paul@thisco.co
 License: MIT
 Keywords: thrift config
 Classifier: Development Status :: 3 - Alpha
```

