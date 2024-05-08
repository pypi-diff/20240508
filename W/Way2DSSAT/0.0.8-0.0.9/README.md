# Comparing `tmp/way2dssat-0.0.8.tar.gz` & `tmp/way2dssat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "way2dssat-0.0.8.tar", last modified: Tue May  7 05:25:19 2024, max compression
+gzip compressed data, was "way2dssat-0.0.9.tar", last modified: Wed May  8 00:15:40 2024, max compression
```

## Comparing `way2dssat-0.0.8.tar` & `way2dssat-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 05:25:19.619156 way2dssat-0.0.8/
--rw-rw-rw-   0        0        0      667 2024-05-07 05:25:19.611140 way2dssat-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       67 2024-04-28 03:48:31.000000 way2dssat-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 05:25:19.449614 way2dssat-0.0.8/Way2DSSAT/
--rw-rw-rw-   0        0        0     4017 2024-05-07 04:46:41.000000 way2dssat-0.0.8/Way2DSSAT/WTH.py
--rw-rw-rw-   0        0        0       92 2024-05-07 04:55:05.000000 way2dssat-0.0.8/Way2DSSAT/__init__.py
--rw-rw-rw-   0        0        0     6928 2024-05-07 04:34:08.000000 way2dssat-0.0.8/Way2DSSAT/gssurgo2soil.py
--rw-rw-rw-   0        0        0     6687 2024-05-07 04:51:57.000000 way2dssat-0.0.8/Way2DSSAT/xfiles.py
-drwxrwxrwx   0        0        0        0 2024-05-07 05:25:19.611140 way2dssat-0.0.8/Way2DSSAT.egg-info/
--rw-rw-rw-   0        0        0      667 2024-05-07 05:25:19.000000 way2dssat-0.0.8/Way2DSSAT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-07 05:25:19.000000 way2dssat-0.0.8/Way2DSSAT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 05:25:19.000000 way2dssat-0.0.8/Way2DSSAT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-07 05:25:19.000000 way2dssat-0.0.8/Way2DSSAT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-07 05:25:19.000000 way2dssat-0.0.8/Way2DSSAT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      698 2024-05-07 05:24:25.000000 way2dssat-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 05:25:19.620358 way2dssat-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      481 2024-05-07 03:15:22.000000 way2dssat-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 00:15:40.456619 way2dssat-0.0.9/
+-rw-rw-rw-   0        0        0     4604 2024-05-08 00:15:40.444473 way2dssat-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4006 2024-05-08 00:11:32.000000 way2dssat-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 00:15:40.284681 way2dssat-0.0.9/Way2DSSAT/
+-rw-rw-rw-   0        0        0     4072 2024-05-08 00:11:56.000000 way2dssat-0.0.9/Way2DSSAT/WTH.py
+-rw-rw-rw-   0        0        0      246 2024-05-08 00:11:50.000000 way2dssat-0.0.9/Way2DSSAT/__init__.py
+-rw-rw-rw-   0        0        0     7604 2024-05-08 00:11:55.000000 way2dssat-0.0.9/Way2DSSAT/gssurgo2soil.py
+-rw-rw-rw-   0        0        0     6183 2024-05-08 00:11:54.000000 way2dssat-0.0.9/Way2DSSAT/xfiles.py
+drwxrwxrwx   0        0        0        0 2024-05-08 00:15:40.444473 way2dssat-0.0.9/Way2DSSAT.egg-info/
+-rw-rw-rw-   0        0        0     4604 2024-05-08 00:15:40.000000 way2dssat-0.0.9/Way2DSSAT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-08 00:15:40.000000 way2dssat-0.0.9/Way2DSSAT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 00:15:40.000000 way2dssat-0.0.9/Way2DSSAT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 00:15:40.000000 way2dssat-0.0.9/Way2DSSAT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 00:15:40.000000 way2dssat-0.0.9/Way2DSSAT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2024-05-08 00:11:48.000000 way2dssat-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 00:15:40.456619 way2dssat-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      481 2024-05-07 03:15:22.000000 way2dssat-0.0.9/setup.py
```

### Comparing `way2dssat-0.0.8/Way2DSSAT/WTH.py` & `way2dssat-0.0.9/Way2DSSAT/WTH.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,68 @@
-'''
+"""
 Creates .WTH file from weather data file 
 
 Input
 -----
-    path: path to csv
+path: path to csv
 
-    the csv must contain following columns
-    - 'SRAD','Tmax','Tmin','Rain','timedate' 
-    - 'timedate' in format = '%m/%d/%Y'/%Y'
+the csv must contain following columns
+- 'SRAD','Tmax','Tmin','Rain','timedate' 
+- 'timedate' in format = '%m/%d/%Y'/%Y'
 
-    stname(optional)
-    ------
-        name of the station
-        first 4 alphabets will be used as output file name
+stname(optional)
+
+    name of the station
+    first 4 alphabets will be used as output file name
+
+latitude
 
-    latitude
-    --------
-        of format = 123.456 
-
-    longitude
-    ---------
-        of format = +-123.456
-    elevation
-    ---------
+    of format = 123.456 
 
+longitude
+
+    of format = +-123.456
+elevation
 
 Output
 ------
     weather file stored as ABCD.WTH
-
-
-'''
+"""
 def WTH(path,stname = 'ABCd',latitude= 34.583,longitude= -103.200,elevation= 1348):
-    '''
-    Creates .WTH file from weather data file 
-
-    Input
-    -----
-        path: path to csv
+    """Creates .WTH file from weather data file. 
 
+    Parameters
+    ----------
+    path: string path to csv.
         the csv must contain following columns
         - 'SRAD','Tmax','Tmin','Rain','timedate' 
-        - 'timedate' in format = '%m/%d/%Y'/%Y'
+        - 'timedate' in format = '%m/%d/%Y'
+
+    stname(optional): string
+        name of the station first 4 alphabets will be 
+        used as output file name.
+
+    latitude : float.
+        of format = 123.456 .
+        
+    longitude : float
+        of format = +-123.456 .
 
-        stname(optional)
-        ------
-            name of the station
-            first 4 alphabets will be used as output file name
-
-        latitude
-        --------
-
-        longitude
-        ---------
-
-        elevation
-        ---------
-        Output
-        ------
-            weather file stored as f'{stname[0:4]}{yy}01.WTH'  for eg: ABCD2301.WTH      
-    '''
+    elevation : float.
+    
+    Output
+    ------
+    writes .WTH file to cwd as f'{stname[0:4]}{yy}01.WTH'  for eg: ABCD2301.WTH.
+    
+    Returns
+    -------
+    weather file stored as f'{stname[0:4]}{yy}01.WTH'  for eg: ABCD2301.WTH.
+    
+    String : name of weather station
+    """
     #Import Modules 
     import pandas
     df = pandas.read_csv(path)
     
     # Converting  the date column into desired format 
     
     df['timedate'] = pandas.to_datetime(df['TS'], format = '%m/%d/%Y')
```

### Comparing `way2dssat-0.0.8/Way2DSSAT/gssurgo2soil.py` & `way2dssat-0.0.9/Way2DSSAT/gssurgo2soil.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,74 @@
-"""
-Converts gSSURGO format into DSSAT .SOL format.
+"""Converts gSSURGO format into DSSAT .SOL format.
     
-Inputs
-------
-path: string
-    path to your .csv file containing the data from gSSURGO. Must have the following columns(and other related depths)
-    WC15Bar_DCP_0to5
-    WC3rdbar_DCP_0to5
-    Clay_DCP_0to5
-    Silt_DCP_0to5
-    pHwater_DCP_0to5
-    CEC_DCP_0to5
-    Db3rdbar_DCP_0to5
-    Ksat_DCP_0to5
-    OrgMatter_DCP_0to5
-    MUKEY_DCP_0to5          
-Output
-------
-    SG.SOL file in cwd
-
-    a py dictionary of format:
-        dictionary = {MUKEY :{depth:SH2O}}
-
-    a list of all the Mukeys
-
-Example
--------
-    path = 'Username/pathtothecsv'
-    A,B = ssurgo2soil(path)          
+Arguments
+
+path -- string
+path to your .csv file containing the data from gSSURGO. Must have the following columns(and other related depths)
+WC15Bar_DCP_0to5
+WC3rdbar_DCP_0to5
+Clay_DCP_0to5
+Silt_DCP_0to5
+pHwater_DCP_0to5
+CEC_DCP_0to5
+Db3rdbar_DCP_0to5
+Ksat_DCP_0to5
+OrgMatter_DCP_0to5
+MUKEY_DCP_0to5          
+
+Return --
+
+SG.SOL file in cwd
+
+a py dictionary of format
+dictionary = {MUKEY :{depth:SH2O}}
+
+a list of all the Mukeys
+
+Example --
+
+path = 'Username/pathtothecsv'
+A,B = ssurgo2soil(path)          
 """
 
-def SOL(path):      
+def SOL(path):
+    """Converts gSSURGO format into DSSAT .SOL format.
+
+    Parameters
+    ----------
+    path : string
+        path to your .csv file containing the data from gSSURGO. Must have the following columns(and other related depths)
+        WC15Bar_DCP_0to5
+        WC3rdbar_DCP_0to5
+        Clay_DCP_0to5
+        Silt_DCP_0to5
+        pHwater_DCP_0to5
+        CEC_DCP_0to5
+        Db3rdbar_DCP_0to5
+        Ksat_DCP_0to5
+        OrgMatter_DCP_0to5
+        MUKEY_DCP_0to5          
+
+    Output
+    ------
+    Creates a SG.SOL file in cwd.
+    
+    Returns
+    -------
+    A : Dictionary of format.
+        A = {MUKEY :{depth:SH2O}}.
+
+    B : List of all the Mukeys.
+
+    Example
+    -------
+    path = 'Username/pathtothecsv'.
+    
+    A,B = ssurgo2soil(path).
+    """
     import pandas
     import math
     #Reading csv  
     df_soil = pandas.read_csv(path)
     #Returns list of columns not required with specific keyword
     # data from ssurgo contains columns suchas pct_Silt** which aren't required
     # Removing those columns form the dataframe
```

### Comparing `way2dssat-0.0.8/Way2DSSAT/xfiles.py` & `way2dssat-0.0.9/Way2DSSAT/xfiles.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,86 +1,85 @@
-'''
-    Function to create DSSAT X file from a template X file
+"""Function to create DSSAT X file from a template X file.
 
-    input
-    -----
-        path: path to the template file
-            Example template 
-            https://github.com/ManavjotSingh97/Way2DSSAT/blob/main/Seasonl/KSMR6301.SNX
-
-        init_cond:
-            dictinary of initial key as depth and value as SDUL  
-            for example dict = 'GSS2733104': {5: 0.2, 15: 0.2, 30: 0.2, 60: 0.2, 
-                                                        100: 0.338, 200: 0.308} 
-        site_name:
-            string of site name less than 120 char
-
-        station:
-            string of max 8 character eg: UFGA8201 or ABCD(default)
-
-        soil:
-            soil name, (not the .SOL file name) for eg: GSS2733103(default)
-        crop:
-            two character for eg: SB(default)
+input
+-----
+path: path to the template file
+    Example template 
+    https://github.com/ManavjotSingh97/Way2DSSAT/blob/main/Seasonl/KSMR6301.SNX
+
+init_cond:
+    dictinary of initial key as depth and value as SDUL  
+    for example dict = 'GSS2733104': {5: 0.2, 15: 0.2, 30: 0.2, 60: 0.2, 
+                                                100: 0.338, 200: 0.308} 
+site_name:
+    string of site name less than 120 char
+
+station:
+    string of max 8 character eg: UFGA8201 or ABCD(default)
+
+soil:
+    soil name, (not the .SOL file name) for eg: GSS2733103(default)
+crop:
+    two character for eg: SB(default)
+
+cultivar:
+    full cultivar name, for eg: NE0006 NECPHA4 2014 (default)
+
+planting_date:
+    planting date in format yydoy , for eg: 24145
+
+Returns
+-------
+    xfile .SNX in cwd
+
+Example
+-------
+    path = 'C:path/to/the/template'
+    init_cond = {5: 0.2, 15: 0.2, 30: 0.2, 60: 0.2, 100: 0.338, 200: 0.308}
+    Xfile()
 
-        cultivar:
-            full cultivar name, for eg: NE0006 NECPHA4 2014 (default)
+    """
 
-        planting_date:
-            planting date in format yydoy , for eg: 24145
+def Xfile(path,init_cond,site_name = '-99',station = 'ABCD',soil = 'GSS2733103',
+          crop = 'SB',cultivar = 'NE0006 NECPHA4 2014',planting_date = '24145'):
+    """Function to create DSSAT X file from a template X file.
 
-    Output
-    ------
-        xfile .SNX in cwd
+    Parameters
+    ----------
 
-    Example
-    -------
-        path = 'C:path/to/the/template'
-        init_cond = {5: 0.2, 15: 0.2, 30: 0.2, 60: 0.2, 100: 0.338, 200: 0.308}
-        Xfile()
+    path: path to the template file.
+        Example template 
+        https://github.com/ManavjotSingh97/Way2DSSAT/blob/main/Seasonl/KSMR6301.SNX
 
-'''
-    
-def Xfile(path,init_cond,site_name = '-99',station = 'ABCD',soil = 'GSS2733103',
-          crop = 'SB',cultivar = 'NE0006 NECPHA4 2014',planting_date = '24145'):
-    '''
-        Function to create DSSAT X file from a template X file
-        
-        input
-        -----
-            path: path to the template file
-                Example template 
-                https://github.com/ManavjotSingh97/Way2DSSAT/blob/main/Seasonl/KSMR6301.SNX
-            
-            init_cond:
-                dictinary of initial key as depth and value as SDUL  
-                for example dict = 'GSS2733104': {5: 0.2, 15: 0.2, 30: 0.2, 60: 0.2, 
-                                                            100: 0.338, 200: 0.308} 
-            site_name:
-                string of site name less than 120 char
-            
-            station:
-                string of max 8 character eg: UFGA8201 or ABCD(default)
-            
-            soil:
-                soil name, (not the .SOL file name) for eg: GSS2733103(default)
-            crop:
-                two character for eg: SB(default)
-            
-            cultivar:
-                full cultivar name, for eg: NE0006 NECPHA4 2014 (default)
-            
-            planting_date:
-                planting date in format yydoy , for eg: 24145
-            
-        Output
-        ------
-            xfile .SNX in cwd
-            
-    '''
+    init_cond:
+        dictinary of initial key as depth and value as SDUL.  
+        for example dict = 'GSS2733104': {5: 0.2, 15: 0.2, 30: 0.2, 60: 0.2} 
+
+    site_name:
+        string of site name less than 120 char.
+
+    station:
+        string of max 8 character eg: UFGA8201 or ABCD(default).
+
+    soil:
+        soil name, (not the .SOL file name) for eg: GSS2733103(default).
+
+    crop:
+        two character for eg: SB(default).
+
+    cultivar:
+        full cultivar name, for eg: NE0006 NECPHA4 2014 (default).
+
+    planting_date:
+        planting date in format yydoy , for eg: 24145.
+
+    Output
+    -------
+        Writes xfile of format .SNX in cwd.
+    """
     #Variables that can be changed
 
     #geting the year part from planting_date variable
     yy=planting_date[0:2]
     crop = crop.upper()
     
     #Checking error in input
```

### Comparing `way2dssat-0.0.8/pyproject.toml` & `way2dssat-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0","pandas"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = [ "pandas"]
 name = "Way2DSSAT"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Manavjot", email="manavjotsingh97@gmail.com" },
 ]
 description = "Package to handle input DSSAT files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

