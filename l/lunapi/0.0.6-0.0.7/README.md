# Comparing `tmp/lunapi-0.0.6-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/lunapi-0.0.7-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,10 @@
-Zip file size: 10328745 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 18:38 lunapi.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 18:38 lunapi/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 18:38 lunapi-0.0.6.dist-info/
--rw-r--r--  2.0 unx     9418 b- defN 24-Apr-26 18:38 lunapi/lunapi0.cpp
--rwxr-xr-x  2.0 unx 27284288 b- defN 24-Apr-26 18:38 lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx    44647 b- defN 24-Apr-26 18:38 lunapi/lunapi1.py
--rw-r--r--  2.0 unx      352 b- defN 24-Apr-26 18:38 lunapi/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 18:38 lunapi-0.0.6.dist-info/licenses/
--rw-rw-r--  2.0 unx     1350 b- defN 24-Apr-26 18:38 lunapi-0.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx      734 b- defN 24-Apr-26 18:38 lunapi-0.0.6.dist-info/RECORD
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-26 18:38 lunapi-0.0.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx      165 b- defN 24-Apr-26 18:38 lunapi-0.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx    35149 b- defN 24-Apr-26 18:38 lunapi-0.0.6.dist-info/licenses/LICENSE
-13 files, 27376103 bytes uncompressed, 10327057 bytes compressed:  62.3%
+Zip file size: 6866696 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      630 b- defN 24-May-02 00:12 lunapi-0.0.7.dist-info/RECORD
+-rw-rw-r--  2.0 unx      118 b- defN 24-May-02 00:12 lunapi-0.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     1350 b- defN 24-May-02 00:12 lunapi-0.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx    35149 b- defN 24-May-02 00:12 lunapi-0.0.7.dist-info/licenses/LICENSE
+-rw-r--r--  2.0 unx      352 b- defN 24-May-02 00:12 lunapi/__init__.py
+-rw-r--r--  2.0 unx    48099 b- defN 24-May-02 00:12 lunapi/lunapi1.py
+-rwxr-xr-x  2.0 unx 15117024 b- defN 24-May-02 00:12 lunapi/lunapi0.pypy39-pp73-darwin.so
+-rw-r--r--  2.0 unx     9947 b- defN 24-May-02 00:12 lunapi/lunapi0.cpp
+8 files, 15212669 bytes uncompressed, 6865634 bytes compressed:  54.9%
```

## zipnote {}

```diff
@@ -1,40 +1,25 @@
-Filename: lunapi.libs/
+Filename: lunapi-0.0.7.dist-info/RECORD
 Comment: 
 
-Filename: lunapi/
+Filename: lunapi-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: lunapi-0.0.6.dist-info/
+Filename: lunapi-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: lunapi/lunapi0.cpp
-Comment: 
-
-Filename: lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
-Comment: 
-
-Filename: lunapi/lunapi1.py
+Filename: lunapi-0.0.7.dist-info/licenses/LICENSE
 Comment: 
 
 Filename: lunapi/__init__.py
 Comment: 
 
-Filename: lunapi-0.0.6.dist-info/licenses/
-Comment: 
-
-Filename: lunapi-0.0.6.dist-info/METADATA
-Comment: 
-
-Filename: lunapi-0.0.6.dist-info/RECORD
-Comment: 
-
-Filename: lunapi-0.0.6.dist-info/entry_points.txt
+Filename: lunapi/lunapi1.py
 Comment: 
 
-Filename: lunapi-0.0.6.dist-info/WHEEL
+Filename: lunapi/lunapi0.pypy39-pp73-darwin.so
 Comment: 
 
-Filename: lunapi-0.0.6.dist-info/licenses/LICENSE
+Filename: lunapi/lunapi0.cpp
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## lunapi/lunapi0.cpp

```diff
@@ -23,33 +23,34 @@
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h> 
 #include <pybind11/eigen.h>
 
 #include "luna.h"
 
 namespace py = pybind11;
+
 using namespace pybind11::literals;
 
 PYBIND11_MODULE(lunapi0, m) {
-
+  
   m.doc() = "LunaAPI: Python bindings for the Luna C/C++ library";
   
   m.def( "inaugurate",
 	 &lunapi_t::inaugurate,
 	 py::return_value_policy::reference ,
 	 "Start/return a reference to the Luna engine" );
-
+  
   m.def( "retire",
 	 &lunapi_t::retire,	 
 	 "Retire an extant Luna engine" );
-
+  
   m.def( "cmdfile" ,
 	 &lunapi_t::cmdfile ,
 	 "Load a Luna script from a file" );    
-
+  
   m.def( "version" ,
 	 &lunapi_t::version ,
 	 "Version of Luna" );
   
   //
   // lunapi_t engine class
   //
@@ -61,148 +62,158 @@
 	  "Load a sample list from a file" )
     .def( "build_sample_list" ,
 	  &lunapi_t::build_sample_list,
 	  "Load a sample list from a file" )
     .def( "get_sample_list" ,
           &lunapi_t::sample_list,
           "Return the loaded sample list" )
-
+    
     .def( "insert_inst" , &lunapi_t::insert_inst )
     .def( "nobs" , &lunapi_t::nobs )
     .def( "clear" , &lunapi_t::clear )
-
+    
     .def( "silence", &lunapi_t::silence )
     .def( "is_silenced" , &lunapi_t::is_silenced )
 
     .def( "flush" , &lunapi_t::flush )
-
+    
     .def( "reset" , &lunapi_t::reset )
     
+    .def( "include" ,
+	  &lunapi_t::includefile ,
+	  "Include a @parameter-file" )
+
+    .def( "aliases" ,
+	  &lunapi_t::aliases ,
+	  "Return table of signal & annotation aliases/mappings" )
+    
     .def("opt",py::overload_cast<const std::string &,const std::string &>(&lunapi_t::var),
-		"Set an option value" )
-
+	 "Set an option value" )
+    
     .def("get_opt",py::overload_cast<const std::string &>(&lunapi_t::var,py::const_ ),
 	 "Show an option value" )
     .def("get_opts",py::overload_cast<const std::vector<std::string> &>(&lunapi_t::vars,py::const_),
 	 "Show multiple option values" )
     .def("get_all_opts",py::overload_cast<>(&lunapi_t::vars,py::const_),
 	 "Show all option values" )
     
-    .def("clear_opt",&lunapi_t::dropvar,
-	 "Clear an option" )
     .def("clear_opts",&lunapi_t::dropvars,
 	 "Clear options" )
     .def("clear_all_opts",&lunapi_t::dropallvars,
 	 "Clear all options" )
-
+    
     .def("clear_ivars",&lunapi_t::clear_ivars,
 	 "Clear all individual-variables")
-
+    
     .def( "inst" ,
 	  py::overload_cast<int>
 	  (&lunapi_t::inst,py::const_),
 	  "Return a lunapi-instance object from a sample list" )
-
+    
     .def( "inst" ,
 	  py::overload_cast<const std::string&>
 	  (&lunapi_t::inst,py::const_),
 	  "Generate an empty lunapi-instance" )
-
+    
     .def( "inst" ,
 	  py::overload_cast<const std::string&,const std::string &>
 	  (&lunapi_t::inst,py::const_),
 	  "Generate an lunapi-instance with attached EDF" )
-
+    
     .def( "inst" ,
 	  py::overload_cast<const std::string&,const std::string &,const std::string&>
 	  (&lunapi_t::inst,py::const_),
 	  "Generate an lunapi-instance with attached EDF & annotation" )
-
+    
     .def( "inst" ,
 	  py::overload_cast<const std::string&,const std::string &,const std::set<std::string>&>
 	  (&lunapi_t::inst,py::const_),
 	  "Generate an lunapi-instance with attached EDF & annotations" )
-
+    
     .def( "get_n" , &lunapi_t::get_n)
     .def( "get_id" , &lunapi_t::get_id)
     .def( "get_edf" , &lunapi_t::get_edf)
     .def( "get_annot" , &lunapi_t::get_annot)
-
+    
     .def( "import_db" ,
 	  py::overload_cast<const std::string &>(&lunapi_t::import_db) )
     .def( "import_db_subset" ,
 	  py::overload_cast<const std::string &,const std::set<std::string> &>(&lunapi_t::import_db) )
-
+    
+    .def("desc",&lunapi_t::desc,
+	 "Table of basic descripives for all individuals" )
     .def("eval",&lunapi_t::eval,
 	 "Evaluate a Luna command sequence given an attached EDF" ) 
-  
+    
     .def("commands",&lunapi_t::commands,
-       "List commands resulting from a prior eval()" )
-
+	 "List commands resulting from a prior eval()" )
+    
     .def("strata",&lunapi_t::strata,
 	 "List command/strata tuples resulting from a prior eval()" )
-
+    
     .def("vars",&lunapi_t::variables,
 	 "List variables (columns) from a table (defined by a command/strat pair) from a prior eval()")
-
+    
     .def("table",py::overload_cast<const std::string &,const std::string &>(&lunapi_t::results,py::const_) ,
 	 "Return a result table (defined by a command/strata pair) from a prior eval()" )
-
+    
     .def("tables",py::overload_cast<>(&lunapi_t::results,py::const_) ,
 	 "Return a result table (defined by a command/strata pair) from a prior eval()" );
-
+  
   //
   // lunapi_inst_t : individual instance (EDF/annotation pair)
   //
-
+  
   py::class_<lunapi_inst_t, std::shared_ptr<lunapi_inst_t> >(m, "inst")
-
+    
     // .def(py::init<const std::string &>(),
     // 	 py::arg( "id" ) = "id1" )
-
+    
     .def( "attach_edf", &lunapi_inst_t::attach_edf,
 	  "Attach an EDF" ,
 	  "edffile"_a )
     .def( "attach_annot",&lunapi_inst_t::attach_annot,
 	  "Attach an annotation file to the current EDF" ,
 	  "annotfile"_a )
-
+    
     
     .def( "refresh", &lunapi_inst_t::refresh,
 	  "Reattach the current EDF")
     .def( "drop", &lunapi_inst_t::drop,
 	  "Drop the current EDF" )
     
+    .def( "desc" , &lunapi_inst_t::desc,
+	  "Return basic descriptive information" )
     .def( "channels", &lunapi_inst_t::channels,
 	  "Return a list of channel labels" )
     .def( "chs", &lunapi_inst_t::channels,
 	  "Return a list of channel labels" )
     .def( "has_channels", &lunapi_inst_t::has_channels,
 	  "Return boolean for whether channels exist (with aliasing)" )
     .def( "has", &lunapi_inst_t::has_channels,
 	  "Return boolean for whether channels exist (with aliasing)" )
 
-
+    
     
     .def( "annots", &lunapi_inst_t::annots,
 	  "Return a list of all annotations class labels" )
     .def( "fetch_annots", &lunapi_inst_t::fetch_annots,
 	  "Return a list of intervals for selected annotations" )
     .def( "fetch_full_annots", &lunapi_inst_t::fetch_full_annots,
 	  "Return a list of intervals and meta-data for selected annotations" )
-
+    
     .def( "has_annots" , &lunapi_inst_t::has_annots,
 	  "Return boolean for whether annotations exist (with aliasing)" )
-
+    
     .def( "has_staging" , &lunapi_inst_t::has_staging,
 	  "Return boolean for whether valid staging annotations exist" )
     
     .def( "stat" , &lunapi_inst_t::status,
 	  "Return a dict of key details on the current EDF" )
-
+    
     .def( "e2i" , &lunapi_inst_t::epochs2intervals ,
 	  "Convert epoch numbers to interval tuples" ,
 	  "e"_a )
     .def( "s2i" , &lunapi_inst_t::seconds2intervals ,
 	  "Convert second (start/stop tuples) to interval tuples" ,
 	  "s"_a )
     
@@ -220,53 +231,53 @@
 	  "Insert a signal" ,
 	  "label"_a , "data"_a , "sr"_a )
     .def( "update_signal" , &lunapi_inst_t::update_signal,
 	  "Update a signal" , "label"_a , "data"_a )
     .def( "insert_annot" , &lunapi_inst_t::insert_annotation,
 	  "Insert an annotation" ,
 	  "label"_a , "intervals"_a , "durcol2"_a = false ) 
-
+    
     .def("ivar",py::overload_cast<const std::string &,const std::string &>(&lunapi_inst_t::ivar),
 	 "Set an individual-variable")
     .def("get_ivar",py::overload_cast<const std::string &>(&lunapi_inst_t::ivar,py::const_),
 	 "Return an individual-variable")
     .def("ivars", &lunapi_inst_t::ivars,
 	 "Return all individual-variables")
     .def("clear_ivar",&lunapi_inst_t::clear_ivar,
 	 "Clear individual-variables")
-
+    .def("clear_selected_ivar",&lunapi_inst_t::clear_selected_ivar,
+	 "Clear selected individual-variables")
+    
+    
     .def("eval",&lunapi_inst_t::eval,
 	 "Evaluate Luna commands" )
-
+    
     .def("proc",&lunapi_inst_t::eval_return_data,
 	 "Similar to eval(), but returns all data tables" )
-
+    
     .def("commands",&lunapi_inst_t::commands,
 	 "List commands resulting from a prior eval()" )
     .def("strata",&lunapi_inst_t::strata,
 	 "List command/strata tuples resulting from a prior eval()" )
     .def("vars",&lunapi_inst_t::variables,
 	 "List variables (columns) from a table (defined by a command/strat pair) from a prior eval()")
     .def("table",py::overload_cast<const std::string &,const std::string &>(&lunapi_inst_t::results,py::const_) ,
 	 "Return a result table (defined by a command/strata pair) from a prior eval()" )
     .def("tables",py::overload_cast<>(&lunapi_inst_t::results,py::const_) ,
 	 "Return a result table (defined by a command/strata pair) from a prior eval()" )
-        
+    
     .def("__repr__",
 	 [](const lunapi_inst_t & a)
 	 {
 	   std::string s = "<lunapi-instance id:" + a.get_id();
 	   const std::string f1 = a.get_edf_file();
 	   const std::string f2 = a.get_annot_files();
 	   if ( f1 != "" ) s += " edf:" + f1;
 	   if ( f2 != "" ) s += " annot:" + f2;
 	   s += ">";
 	   return s;
 	 }
 	 );
-  
-
-
-  
+ 
   
 }
```

## lunapi/lunapi1.py

```diff
@@ -1,11 +1,11 @@
 """lunapi1 module provides a high-level convenience wrapper around lunapi0 module functions."""
 
 # Luna Python wrapper
-# v0.0.6, 26-Apr-2024
+# v0.0.7, 1-May-2024
 
 import lunapi.lunapi0 as _luna
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import cm
 from IPython.core import display as ICD
@@ -13,15 +13,15 @@
 
 # resource set for Docker container version
 class resources:
    POPS_PATH = '/build/nsrr/common/resources/pops/'
    POPS_LIB = 's2'
    MODEL_PATH = '/build/luna-models/'
 
-lp_version = "v0.0.6"
+lp_version = "v0.0.7"
    
 # C++ singleton class (engine & sample list)
 # lunapi_t      --> luna
 
 # one observation
 # lunapi_inst_T --> inst
 
@@ -178,54 +178,83 @@
       
       
    #------------------------------------------------------------------------
    def flush(self):
       """Internal command, to flush the output buffer"""
       proj.eng.flush()
 
+   # --------------------------------------------------------------------------------
+   def include( self, f ):
+      """Include options/variables from a @parameter-file"""
+      return proj.eng.include( f )
+
+
    #------------------------------------------------------------------------
-   def var(self,key=None,value=None):
-      """Set or return a project-level argument/option"""
-      if key == None:
+   def aliases( self ):
+      """Return a table of signal/annotation aliases"""
+      t = pd.DataFrame( proj.eng.aliases() )      
+      t.index = t.index + 1
+      if len( t ) == 0: return t
+      t.columns = ["Type", "Preferred", "Case-insensitive, sanitized alias" ]
+      with pd.option_context('display.max_rows', None,):   
+         display(t)
+
+   #------------------------------------------------------------------------
+   def var(self , key=None , value=None):
+      """Set or get project-level options(s)/variables(s)"""
+      return self.vars( key, value )
+
+   #------------------------------------------------------------------------
+   def vars(self , key=None , value=None):
+      """Set or get project-level options(s)/variables(s)"""
+
+      # return all vars?
+      if key is None:
          return proj.eng.get_all_opts()
-      if value == None:
-         if type(key) is not list: key = [ key ]
-         return proj.eng.get_opt( key )
-      else:         
-         proj.eng.opt( key, str( value ) )
-
-   #------------------------------------------------------------------------                                                                                                                                                            
-   def varmap(self,d):
-      """Sets project-level arguments/options"""
-      if isinstance(d, dict):
-         for k, v in d.items():
-            self.var(k,v)
+
+      # return one or more vars?
+      if value is None:
          
-   #------------------------------------------------------------------------
-   def vars(self):
-      """Return a dictionary of all project-level variables"""
-      return proj.eng.get_all_opts()
+         # return 1?
+         if type( key ) is str:
+            return proj.eng.get_opt( key )
+
+         # return some?
+         if type( key ) is list:
+            return proj.eng.get_opts( key )
+
+      # set from a dict
+      if isinstance(key, dict):
+         for k, v in key.items():
+            self.vars(k,v)
+         return
 
-   
+      # set a single pair
+      proj.eng.opt( key, str( value ) )
+
+            
    #------------------------------------------------------------------------
-   def clear_var(self,key):
-      """Clear a project-level option/variable"""
-      proj.eng.clear_opt(key)
+#   def clear_var(self,key):
+#      """Clear project-level option(s)/variable(s)"""
+#      self.clear_vars(key)
 
    #------------------------------------------------------------------------
-   def clear_vars(self,key):
-      """Clear a project-level option/variable"""
+   def clear_vars(self,key = None ):
+      """Clear project-level option(s)/variable(s)"""
+
+      # clear all
+      if key is None:
+         proj.eng.clear_all_opts()
+         return
+
+      # clear some/one
       if type(key) is not list: key = [ key ]
       proj.eng.clear_opts(key)
 
-   #------------------------------------------------------------------------
-   def clear_all_vars(self):
-      """Clear all project-level options/variables"""
-      proj.eng.clear_all_opts()
-
+      
    #------------------------------------------------------------------------   
    def clear_ivars(self):
       """Clear individual-level variables for all individuals"""
       proj.eng.clear_ivars()
 
    #------------------------------------------------------------------------
    def get_n(self,id):
@@ -254,53 +283,66 @@
       else:
          return proj.eng.get_annot(proj.eng.get_n(x))
 
 
    #------------------------------------------------------------------------      
    def import_db(self,f,s=None):
       """Import a destrat-style Luna output database"""
-      if s == None:
+      if s is None:
          return proj.eng.import_db(f)
       else:
          return proj.eng.import_db_subset(f,s)
 
    #------------------------------------------------------------------------      
-   def eval(self, cmdstr ):
+   def desc( self ):
+      """Returns table of descriptives for all sample-list individuals"""
+      silence_mode = self.is_silenced()
+      self.silence(True,False)
+      t = pd.DataFrame( proj.eng.desc() )
+      self.silence( silence_mode , False )
+      t.index = t.index + 1
+      if len( t ) == 0: return t
+      t.columns = ["ID","Gapped","Date","Start(hms)","Stop(hms)","Dur(hms)","Dur(s)","# sigs","# annots","Signals" ]
+      with pd.option_context('max_colwidth',None):
+         display(t)
+
+      
+   #------------------------------------------------------------------------      
+   def proc(self, cmdstr ):
       """Evaluates one or more Luna commands for all sample-list individuals"""
       r = proj.eng.eval(cmdstr)
       return tables( r )
 
    #------------------------------------------------------------------------ 
-   def silent_eval(self, cmdstr ):
+   def silent_proc(self, cmdstr ):
       """Silently evaluates one or more Luna commands for all sample-list individuals"""
       silence_mode = self.is_silenced()
       self.silence(True,False)
       r = proj.eng.eval(cmdstr)
       self.silence( silence_mode , False )
       return tables( r )
-   
-   
+      
    #------------------------------------------------------------------------   
    def commands( self ):
-      """Return a list of commands in the output set (following eval()"""
+      """Return a list of commands in the output set (following proc()"""
       t = pd.DataFrame( proj.eng.commands() )
       t.columns = ["Command"]
       return t
 
    #------------------------------------------------------------------------
    def empty_result_set( self ):
       return len( proj.eng.strata()  ) == 0
 
    #------------------------------------------------------------------------   
    def strata( self ):
       """Return a datraframe of command/strata pairs from the output set"""
       
       if self.empty_result_set(): return None
       t = pd.DataFrame( proj.eng.strata() )      
-      t.columns = ["Command","Stratum"]
+      t.columns = ["Command","Strata"]
       return t
 
    #------------------------------------------------------------------------
    def table( self, cmd , strata = 'BL' ):
       """Return a dataframe from the output set"""
       if self.empty_result_set(): return None
       r = proj.eng.table( cmd , strata )
@@ -328,91 +370,91 @@
              do_reref = False ,
              m = None , m1 = None , m2 = None,
              lights_off = '.' , lights_on = '.' ,
              ignore_obs = False, 
              args = '' ):
       """Run the POPS stager"""
 
-      if path == None: path = resources.POPS_PATH
-      if lib == None: lib = resources.POPS_LIB
+      if path is None: path = resources.POPS_PATH
+      if lib is None: lib = resources.POPS_LIB
       
       import os
       if not os.path.isdir( path ):         
          return 'could not open POPS resource path ' + path 
 
-      if s == None and s1 == None:
+      if s is None and s1 is None:
          print( 'must set s or s1 and s2 to EEGs' )
          return
 
-      if ( s1 == None ) != ( s2 == None ):
+      if ( s1 is None ) != ( s2 is None ):
          print( 'must set s or s1 and s2 to EEGs' )
          return
          
       # set options
       self.var( 'mpath' , path )
       self.var( 'lib' , lib )
       self.var( 'do_edger' , '1' if do_edger else '0' )
       self.var( 'do_reref' , '1' if do_reref else '0' )
       self.var( 'no_filter' , '1' if no_filter else '0' )
       self.var( 'LOFF' , lights_off )
       self.var( 'LON' , lights_on )
       
-      if s != None: self.var( 's' , s )
-      else: self.clear_var( 's' )
+      if s is not None: self.var( 's' , s )
+      else: self.clear_vars( 's' )
       
-      if m != None: self.var( 'm' , m )
-      else: self.clear_var( 'm' )
+      if m is not None: self.var( 'm' , m )
+      else: self.clear_vars( 'm' )
 
-      if s1 != None: self.var( 's1' , s1 )
-      else: self.clear_var( 's1' )
+      if s1 is not None: self.var( 's1' , s1 )
+      else: self.clear_vars( 's1' )
       
-      if s2 != None: self.var( 's2' , s2 )
-      else: self.clear_var( 's2' )
+      if s2 is not None: self.var( 's2' , s2 )
+      else: self.clear_vars( 's2' )
       
-      if m1 != None: self.var( 'm1' , m1 )
-      else: self.clear_var( 'm1' )
+      if m1 is not None: self.var( 'm1' , m1 )
+      else: self.clear_vars( 'm1' )
       
-      if m2 != None: self.var( 'm2' , m2 )
-      else: self.clear_var( 'm2' )
+      if m2 is not None: self.var( 'm2' , m2 )
+      else: self.clear_vars( 'm2' )
             
       # get either one- or two-channel mode Luna script from POPS folder
-      twoch = s1 != None and s2 != None;
+      twoch = s1 is not None and s2 is not None;
       if twoch: cmdstr = cmdfile( path + '/s2.ch2.txt' )
       else: cmdstr = cmdfile( path + '/s2.ch1.txt' )
 
       # swap in any additional options to POPS
       if ignore_obs is True:
          args = args + ' ignore-obs-staging';
          if do_edger is True:
             cmdstr = cmdstr.replace( 'EDGER' , 'EDGER all' )
       if args != '':
             cmdstr = cmdstr.replace( 'POPS' , 'POPS ' + args + ' ')
       
       # run the command
-      self.eval( cmdstr )
+      self.proc( cmdstr )
 
       # return of results
       return self.table( 'POPS' )
 
 
    # --------------------------------------------------------------------------------
    def predict_SUN2019( self, cen , th = '3' , path = None ):
       """Run SUN2019 prediction model for a project
 
       This assumes that ${age} will be set via a vars file, i.e.
 
-         proj.opt( 'vars' , 'ages.txt' )      
+         proj.var( 'vars' , 'ages.txt' )      
 
       """
-      if path == None: path = resources.MODEL_PATH
+      if path is None: path = resources.MODEL_PATH
       if type( cen ) is list: cen = ','.join( cen )
       self.var( 'cen' , cen )
       self.var( 'mpath' , path )
       self.var( 'th' , str(th) )
-      self.eval( cmdfile( resources.MODEL_PATH + '/m1-adult-age-luna.txt' ) )
+      self.proc( cmdfile( resources.MODEL_PATH + '/m1-adult-age-luna.txt' ) )
       return self.table( 'PREDICT' )
 
 
 
 
       
 
@@ -463,33 +505,66 @@
       # note: current kludge: problem is proj-wide
       #       so this will not play well w/ multiple EDFs
       # todo: implement inst-specific prob flag
       
       _proj = proj(False)
       _proj.reset();
 
-   #------------------------------------------------------------------------      
-   def ivar( self , key , value = None ):
-      """Set or get an individual-level variable"""
-      if value != None: self.edf.ivar( key , str(value) )
-      else: return self.edf.get_ivar( key )
-         
-   #------------------------------------------------------------------------                                                                                                                                                            
-   def ivarmap(self,d):
-      """Sets individual-level variables"""
-      if isinstance(d, dict):
-         for k, v in d.items():
-            self.ivar(k,v)
 
+   #------------------------------------------------------------------------
+   def clear_vars(self, keys = None ):
+      """Clear some or all individual-level variable(s)"""
+
+      # all
+      if keys is None:
+         self.edf.clear_ivar()
+         return
+
+      # one/some
+      if type( keys ) is not set: keys = set( keys )
+      self.edf.clear_selected_ivar( keys )
+      
+   #------------------------------------------------------------------------
+   def var( self , key = None , value = None ):
+      """Set or get individual-level variable(s)"""
+      return self.vars( key , value )
+   
    #------------------------------------------------------------------------      
-   def ivars( self ):
-      """Return all individual-level variables"""
-      return self.edf.ivars()
+   def vars( self , key = None , value = None ):
+      """Set or get individual-level variable(s)"""
+
+      # return all i-vars
+      if key is None:
+         return self.edf.ivars()
+
+      # return one i-var   
+      if value is None and type( key ) is str:
+         return self.edf.get_ivar( key )
+      
+      # set from a dict of key-value pairs
+      if isinstance(key, dict):
+         for k, v in key.items():
+            self.vars(k,v)
+         return
+
+      # set a single pair
+      self.edf.ivar( key , str(value) )
+               
 
    #------------------------------------------------------------------------      
+   def desc( self ):
+      """Returns of dataframe of current channels"""
+      t = pd.DataFrame( self.edf.desc() ).T
+      t.index =	t.index	+ 1
+      if len( t ) == 0: return t
+      t.columns = ["ID","Gapped","Date","Start(hms)","Stop(hms)","Dur(hms)","Dur(s)","# sigs","# annots","Signals" ]
+      with pd.option_context('display.max_colwidth',None):
+         display(t)
+   
+   #------------------------------------------------------------------------      
    def channels( self ):
       """Returns of dataframe of current channels"""
       t = pd.DataFrame( self.edf.channels() )
       if len( t ) == 0: return t
       t.columns = ["Channels"]
       return t
 
@@ -553,15 +628,15 @@
       return len( self.edf.strata()  ) == 0
 
    #------------------------------------------------------------------------
    def strata( self ):
       """Return a dataframe of command/strata pairs from the output set"""
       if ( self.empty_result_set() ): return None
       t = pd.DataFrame( self.edf.strata() )
-      t.columns = ["Command","Stratum"]
+      t.columns = ["Command","Strata"]
       return t
 
    #------------------------------------------------------------------------
    def table( self, cmd , strata = 'BL' ):
       """Return a dataframe for a given command/strata pair from the output set"""
       if ( self.empty_result_set() ): return None
       r = self.edf.table( cmd , strata )
@@ -575,46 +650,47 @@
       if ( self.empty_result_set() ): return None
       return self.edf.variables( cmd , strata )
 
 
    #------------------------------------------------------------------------
    def e2i( self, epochs ):
       """Helper function to convert epoch (1-based) to intervals"""
+      if type( epochs ) is not list: epochs = [ epochs ]
       return self.edf.e2i( epochs )
-   
+     
    # --------------------------------------------------------------------------------
    def s2i( self, secs ):
       """Helper function to convert seconds to intervals"""
       return self.edf.s2i( secs )
 
    # --------------------------------------------------------------------------------
    def data( self, chs , annots = None , time = False ):
       """Returns all data for certain channels and annotations"""
       if type( chs ) is not list: chs = [ chs ]
-      if annots != None:
+      if annots is not None:
          if type( annots ) is not list: annots = [ annots ]
-      if annots == None: annots = [ ]
+      if annots is None: annots = [ ]
       return self.edf.data( chs , annots , time )
 
    # --------------------------------------------------------------------------------
    def slice( self, intervals, chs , annots = None , time = False ):
       """Return signal/annotation data aggregated over a set of intervals"""
       if type( chs ) is not list: chs = [ chs ]
-      if annots != None:
+      if annots is not None:
          if type( annots ) is not list: annots = [ annots ]
-      if annots == None: annots = [ ]
+      if annots is None: annots = [ ]
       return self.edf.slice( intervals, chs , annots , time )
 
    # --------------------------------------------------------------------------------   
    def slices( self, intervals, chs , annots = None , time = False ):
       """Return a series of signal/annotation data objects for each requested interval"""
       if type( chs ) is not list: chs = [ chs ]
-      if annots != None:
+      if annots is not None:
          if type( annots ) is not list: annots = [ annots ]
-      if annots == None: annots = [ ]
+      if annots is None: annots = [ ]
       return self.edf.slices( intervals, chs , annots , time )
    
    # --------------------------------------------------------------------------------
    def insert_signal( self, label , data , sr ):
       """Insert a signal into an in-memory EDF"""
       return self.edf.insert_signal( label , data , sr )
 
@@ -650,15 +726,15 @@
 
    # --------------------------------------------------------------------------------
    def empty_freezer( self ):
       self.eval( 'CLEAN-FREEZER' )
       
    # --------------------------------------------------------------------------------
    def mask( self , f = None ):
-      if f == None: return
+      if f is None: return
       if type(f) is not list: f = [ f ]
       [ self.eval( 'MASK ' + _f ) for _f in f ]
       self.eval( 'RE' )   
 
    
    # --------------------------------------------------------------------------------
    def segments( self ):
@@ -677,15 +753,15 @@
       df = df[[ 'E', 'E1', 'LABEL', 'HMS', 'START','STOP','DUR' ]]
       #df = df.drop(columns = ['ID','TP','MID','INTERVAL'] )
       return df
       
    # --------------------------------------------------------------------------------
    def psd( self, ch, var = 'PSD' , minf = None, maxf = None, minp = None, maxp = None , xlines = None , ylines = None ):
       """Generates a PSD plot (from PSD or MTM)"""
-      if ch == None: return
+      if ch is None: return
       if type(ch) is not list: ch = [ ch ]
 
       if var == 'PSD':
          self.eval( 'PSD spectrum dB sig=' + ','.join(ch) )
          df = self.table( 'PSD' , 'CH_F' )
       else:
          self.eval( 'MTM tw=15 dB sig=' + ','.join(ch) )
@@ -695,15 +771,15 @@
            minf = minf , maxf = maxf , minp = minp , maxp = maxp ,
            xlines = xlines , ylines = ylines )
       
     
    # --------------------------------------------------------------------------------
    def spec( self, ch, var = 'PSD' , mine = None, maxe = None, minf = None, maxf = None , w = 0.025 ):
       """Generates a PSD spectrogram (from PSD or MTM)"""
-      if ch == None: return
+      if ch is None: return
       if type(ch) is not list: ch = [ ch ]
 
       if var == 'PSD':
          self.eval( 'PSD epoch-spectrum dB sig=' + ','.join(ch) )
          df = self.table( 'PSD' , 'CH_E_F' )
       else:
          self.eval( 'MTM epoch-spectra epoch epoch-output dB tw=15 sig=' + ','.join(ch) )
@@ -720,47 +796,47 @@
              do_reref = False ,
              m = None , m1 = None , m2 = None ,
              lights_off = '.' , lights_on = '.' ,
              ignore_obs = False, 
              args = '' ):
       """Run the POPS stager"""
 
-      if path == None: path = resources.POPS_PATH
-      if lib == None: lib = resources.POPS_LIB
+      if path is None: path = resources.POPS_PATH
+      if lib is None: lib = resources.POPS_LIB
       
       import os
       if not os.path.isdir( path ):         
          return 'could not open POPS resource path ' + path 
 
-      if s == None and s1 == None:
+      if s is None and s1 is None:
          print( 'must set s or s1 and s2 to EEGs' )
          return
 
-      if ( s1 == None ) != ( s2 == None ):
+      if ( s1 is None ) != ( s2 is None ):
          print( 'must set s or s1 and s2 to EEGs' )
          return
          
       # set options
-      self.ivar( 'mpath' , path )
-      self.ivar( 'lib' , lib )
-      self.ivar( 'do_edger' , '1' if do_edger else '0' )
-      self.ivar( 'do_reref' , '1' if do_reref else '0' )
-      self.ivar( 'no_filter' , '1' if no_filter else '0' )
-      self.ivar( 'LOFF' , lights_off )
-      self.ivar( 'LON' , lights_on )
-
-      if s != None: self.ivar( 's' , s )
-      if m != None: self.ivar( 'm' , m )
-      if s1 != None: self.ivar( 's1' , s1 )
-      if s2 != None: self.ivar( 's2' , s2 )
-      if m1 != None: self.ivar( 'm1' , m1 )
-      if m2 != None: self.ivar( 'm2' , m2 )
+      self.var( 'mpath' , path )
+      self.var( 'lib' , lib )
+      self.var( 'do_edger' , '1' if do_edger else '0' )
+      self.var( 'do_reref' , '1' if do_reref else '0' )
+      self.var( 'no_filter' , '1' if no_filter else '0' )
+      self.var( 'LOFF' , lights_off )
+      self.var( 'LON' , lights_on )
+
+      if s is not None: self.var( 's' , s )
+      if m is not None: self.var( 'm' , m )
+      if s1 is not None: self.var( 's1' , s1 )
+      if s2 is not None: self.var( 's2' , s2 )
+      if m1 is not None: self.var( 'm1' , m1 )
+      if m2 is not None: self.var( 'm2' , m2 )
       
       # get either one- or two-channel mode Luna script from POPS folder
-      twoch = s1 != None and s2 != None;
+      twoch = s1 is not None and s2 is not None;
       if twoch: cmdstr = cmdfile( path + '/s2.ch2.txt' )
       else: cmdstr = cmdfile( path + '/s2.ch1.txt' )
 
       # swap in any additional options to POPS
       if ignore_obs is True:
          args = args + ' ignore-obs-staging';
          if do_edger is True:
@@ -775,25 +851,25 @@
       # return of results
       return self.table( 'POPS' , 'E' )
 
 
    # --------------------------------------------------------------------------------
    def predict_SUN2019( self, cen , age = None , th = '3' , path = None ):
       """Run SUN2019 prediction model for a single individual"""
-      if path == None: path = resources.MODEL_PATH
+      if path is None: path = resources.MODEL_PATH
       if type( cen ) is list : cen = ','.join( cen )
       
-      # set ivars
-      if age == None:
-         print( 'need to set age ivar' )
+      # set i-vars
+      if age is None:
+         print( 'need to set age indiv-var' )
          return
-      self.ivar( 'age' , str(age) )
-      self.ivar( 'cen' , cen )
-      self.ivar( 'mpath' , path )
-      self.ivar( 'th' , str(th) )
+      self.var( 'age' , str(age) )
+      self.var( 'cen' , cen )
+      self.var( 'mpath' , path )
+      self.var( 'th' , str(th) )
       self.eval( cmdfile( resources.MODEL_PATH + '/m1-adult-age-luna.txt' ) )
       return self.table( 'PREDICT' )
 
    # --------------------------------------------------------------------------------   
    def stages(self):
       """Return of a list of stages"""   
       hyp = self.silent_proc( "STAGE" )
@@ -819,34 +895,34 @@
       res = self.edf.has_staging()
       _proj.silence( silence_mode , False )
       return res
 
    # --------------------------------------------------------------------------------
    def has_annots(self,anns):
       """Returns boolean for which annotations are present"""
-      if anns == None: return
+      if anns is None: return
       if type( anns ) is not list: anns = [ anns ]
       return self.edf.has_annots( anns )
 
    # --------------------------------------------------------------------------------
    def has_annot(self,anns):
       """Returns boolean for which annotations are present"""
       return self.has_annots(anns)
 
    # --------------------------------------------------------------------------------
    def has_channels(self,ch):
       """Return a boolean to indicate whether a given channel exists"""
-      if ch == None: return
+      if ch is None: return
       if type(ch) is not list: ch = [ ch ]
       return self.edf.has_channels( ch )
 
    # --------------------------------------------------------------------------------
    def has(self,ch):
       """Return a boolean to indicate whether a given channel exists"""
-      if ch == None: return
+      if ch is None: return
       if type(ch) is not list: ch = [ ch ]
       return self.edf.has_channels( ch )
 
    # --------------------------------------------------------------------------------                                                                  
    def spec(self,ch,mine = None , maxe = None , minf = None, maxf = None, w = 0.025 ):
       """PSD given channel 'ch'"""
       if type( ch ) is not str:
@@ -876,60 +952,104 @@
 
 # --------------------------------------------------------------------------------
 def cmdfile( f ):
    """load and parse a Luna command script from a file"""
 
    return _luna.cmdfile( f )
 
+
 # --------------------------------------------------------------------------------
 def strata( ts ):
    """Utility function to format tables"""
    r = [ ] 
    for cmd in ts:
       strata = ts[cmd].keys()
       for stratum in strata:
          r.append( ( cmd , strata ) )
       return r
 
    t = pd.DataFrame( self.edf.strata() )
-   t.columns = ["Command","Stratum"]
+   t.columns = ["Command","Strata"]
    return t
 
 # --------------------------------------------------------------------------------
 def table( ts, cmd , strata = 'BL' ):
    """Utility function to format tables"""
    r = ts[cmd][strata]
    t = pd.DataFrame( r[1] ).T
    t.columns = r[0]
    return t
 
 # --------------------------------------------------------------------------------
 def tables( ts ):
    """Utility function to format tables"""
    r = { }
-   for cmd in ts:
+   for cmd in ts.keys():
       strata = ts[cmd].keys()
       for stratum in strata:
          r[ cmd + ": " + stratum ] = _table2df( ts[cmd][stratum] ) 
-      return r
+   return r
 
 # --------------------------------------------------------------------------------
 def _table2df( r ):
    """Utility function to format tables"""
    t = pd.DataFrame( r[1] ).T
    t.columns = r[0]
    return t
 
 # --------------------------------------------------------------------------------
 def show( dfs ):
    """Utility function to format tables"""
    for title , df in dfs.items():
       print( _color.BOLD + _color.DARKCYAN + title + _color.END )
       ICD.display(df)
- 
+
+
+# --------------------------------------------------------------------------------
+def subset( df , ids = None , qry = None , vars = None  ):
+   """Utility function to subset table rows/columns"""
+
+   # subset rows (ID)
+   if ids is not None:
+      if type(ids) is not list: ids = [ ids ]
+      df = df[ df[ 'ID' ].isin( ids ) ]
+
+   # subset rows (factors/levels)
+   if type(qry) is str:
+      df = df.query( qry )
+	
+   # subset cols (vars)
+   if vars is not None:
+      if type(vars) is not list: vars = [ vars ]
+      vars.insert( 0, 'ID' )
+      df = df[ vars ]
+
+   return df
+
+# --------------------------------------------------------------------------------
+def concat( dfs , tlab , vars = None , add_index = None , ignore_index = True ):
+   """Utility function to extract and concatenate tables"""
+
+   # assume dict[k]['cmd: faclvl']->table
+   # and we want to concatenate over 'k'
+   # assume 'k' will be tracked in the tables (e.g. via TAG)
+
+   if add_index is not None:
+      for k in dfs.keys():
+         dfs[k][tlab][ [add_index] ] = k
+
+   if vars is not None:
+      if type(vars) is not list: vars = [ vars ]
+      dfs = pd.concat( [ dfs[ k ][ tlab ][ vars ] for k in dfs.keys() ] , ignore_index = ignore_index )
+   if vars is None:
+      dfs = pd.concat( [ dfs[ k ][ tlab ] for k in dfs.keys() ] , ignore_index = ignore_index )
+
+   return dfs
+
+
 # --------------------------------------------------------------------------------
 #
 # Helpers
 #
 # --------------------------------------------------------------------------------
 
 def version():
@@ -1032,15 +1152,15 @@
 # --------------------------------------------------------------------------------
 
 
 # --------------------------------------------------------------------------------
 def hypno( ss , e = None , xsize = 20 , ysize = 2 , title = None ):
     """Plot a hypnogram"""
     ssn = stgn( ss )
-    if e == None: e = np.arange(0, len(ssn), 1)
+    if e is None: e = np.arange(0, len(ssn), 1)
     e = e/120
     plt.figure(figsize=(xsize , ysize ))
     plt.plot( e , ssn , c = 'gray' , lw = 0.5 )
     plt.scatter( e , ssn , c = stgcol( ss ) , zorder=2.5 , s = 10 )
     plt.ylabel('Sleep stage')
     plt.xlabel('Time (hrs)')
     plt.ylim(-3.5, 2.5)
@@ -1075,56 +1195,56 @@
 
 
 
 # --------------------------------------------------------------------------------
 def psd(df , ch, var = 'PSD' , minf = None, maxf = None, minp = None, maxp = None , 
         xlines = None , ylines = None, dB = False ):
     """Returns a PSD plot from PSD or MTM epoch table (CH_F)"""
-    if ch == None: return
+    if ch is None: return
     if type( ch ) is not list: ch = [ ch ]
     if type( xlines ) is not list and xlines != None: xlines = [ xlines ]
     if type( ylines ) is not list and ylines != None: ylines = [ ylines ]
     df = df[ df['CH'].isin(ch) ]
     if len(df) == 0: return
     f = df['F'].to_numpy(dtype=float)
     p = df[var].to_numpy(dtype=float)
     if dB is True: p = 10*np.log10(p)
     cx = df['CH'].to_numpy(dtype=str)
-    if minp == None: minp = min(p)
-    if maxp == None: maxp = max(p)
-    if minf == None: minf = min(f)
-    if maxf == None: maxf = max(f)
+    if minp is None: minp = min(p)
+    if maxp is None: maxp = max(p)
+    if minf is None: minf = min(f)
+    if maxf is None: maxf = max(f)
     incl = np.zeros(len(df), dtype=bool)
     incl[ (f >= minf) & (f <= maxf) ] = True
     f = f[ incl ]
     p = p[ incl ]
     cx = cx[ incl ] 
     p[ p > maxp ] = maxp
     p[ p < minp ] = minp
     [ plt.plot(f[ cx == _ch ], p[ cx == _ch ] , label = _ch ) for _ch in ch ]
     plt.legend()
     plt.xlabel('Frequency (Hz)')
     plt.ylabel('Power (dB)')
-    if xlines != None: [plt.axvline(_x, linewidth=1, color='gray') for _x in xlines ]
-    if ylines != None: [plt.axhline(_y, linewidth=1, color='gray') for _y in ylines ]
+    if xlines is not None: [plt.axvline(_x, linewidth=1, color='gray') for _x in xlines ]
+    if ylines is not None: [plt.axhline(_y, linewidth=1, color='gray') for _y in ylines ]
     plt.show()
 
 
 # --------------------------------------------------------------------------------
 def spec(df , ch = None , var = 'PSD' , mine = None , maxe = None , minf = None, maxf = None, w = 0.025 ):
     """Returns a spectrogram from a PSD or MTM epoch table (CH_E_F)"""
-    if ch != None: df = df.loc[ df['CH'] == ch ]
+    if ch is not None: df = df.loc[ df['CH'] == ch ]
     if len(df) == 0: return
     x = df['E'].to_numpy(dtype=int)
     y = df['F'].to_numpy(dtype=float)
     z = df[ var ].to_numpy(dtype=float)
-    if mine == None: mine = min(x)
-    if maxe == None: maxe = max(x)
-    if minf == None: minf = min(y)
-    if maxf == None: maxf = max(y)
+    if mine is None: mine = min(x)
+    if maxe is None: maxe = max(x)
+    if minf is None: minf = min(y)
+    if maxf is None: maxf = max(y)
     incl = np.zeros(len(df), dtype=bool)
     incl[ (x >= mine) & (x <= maxe) & (y >= minf) & (y <= maxf) ] = True
     x = x[ incl ]
     y = y[ incl ]
     z = z[ incl ]
     z = winsorize( z , limits=[w, w] )
 
@@ -1156,35 +1276,35 @@
 def topo_heat(chs, z,  ths = None , th=0.05 ,
               topo = None , 
               lmts= None , sz=70, colormap = "bwr", title = "", 
               rimcolor="black", lab = "dB"):
     """Generate a channel-wise topoplot"""
 
     z = np.array(z)
-    if ths != None: ths = np.array(ths)
-    if topo == None: topo = default_xy()
+    if ths is not None: ths = np.array(ths)
+    if topo is None: topo = default_xy()
 
     xlim = [-0.6, 0.6]
     ylim = [-0.6, 0.6]
     rng = [np.min(z), np.max(z)]
 
-    if lmts == None : lmts = rng
+    if lmts is None : lmts = rng
     else: assert lmts[0] <= rng[0] <= lmts[1] and lmts[0] <= rng[1] <= lmts[1], "channel values are out of specified limits"
    
     assert len(set(topo['CH']).intersection(chs)) > 0, "no matching channels"
     
     chs = chs.apply(lambda x: x.upper())    
     topo = topo[topo['CH'].isin(chs)]
     topo["vals"] = np.nan
     topo["th_vals"] = np.nan
     topo["rims"] = 0.5
 
     for ix, ch in topo.iterrows():
         topo.loc[ix,'vals'] = z[chs == ch["CH"]]
-        if ths == None:
+        if ths is None:
            topo.loc[ix,'th_vals'] = 999;
         else:              
            topo.loc[ix,'th_vals'] = ths[chs == ch["CH"]] 
 
         if topo.loc[ix,'th_vals'] < th:
            topo.loc[ix,'rims'] = 1.5
```

## Comparing `lunapi-0.0.6.dist-info/METADATA` & `lunapi-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python interface to the Luna toolset for sleep signal analysis
 Keywords: Sleep,EEG,PSG,Luna,Signal processing
 Author-Email: Shaun Purcell <smpurcell@bwh.harvard.edu>, Senthil Palanivelu <spalanivelu@mgh.harvard.edu>, Nataliia Kozhemiako <nkozhemiako@bwh.harvard.edu>
 Maintainer-Email: Senthil Palanivelu <spalanivelu@mgh.harvard.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

## Comparing `lunapi-0.0.6.dist-info/licenses/LICENSE` & `lunapi-0.0.7.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

