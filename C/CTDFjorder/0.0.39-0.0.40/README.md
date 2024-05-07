# Comparing `tmp/ctdfjorder-0.0.39.tar.gz` & `tmp/ctdfjorder-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdfjorder-0.0.39.tar", last modified: Sat May  4 07:32:29 2024, max compression
+gzip compressed data, was "ctdfjorder-0.0.40.tar", last modified: Tue May  7 22:11:45 2024, max compression
```

## Comparing `ctdfjorder-0.0.39.tar` & `ctdfjorder-0.0.40.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:32:29.462232 ctdfjorder-0.0.39/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:32:29.458232 ctdfjorder-0.0.39/CTDFjorder/
--rw-r--r--   0 runner    (1001) docker     (127)    59203 2024-05-04 07:32:25.000000 ctdfjorder-0.0.39/CTDFjorder/CTDFjorder.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 07:32:25.000000 ctdfjorder-0.0.39/CTDFjorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:32:29.462232 ctdfjorder-0.0.39/CTDFjorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 07:32:29.000000 ctdfjorder-0.0.39/CTDFjorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 07:32:29.000000 ctdfjorder-0.0.39/CTDFjorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:32:29.000000 ctdfjorder-0.0.39/CTDFjorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 07:32:29.000000 ctdfjorder-0.0.39/CTDFjorder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 07:32:29.000000 ctdfjorder-0.0.39/CTDFjorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 07:32:29.000000 ctdfjorder-0.0.39/CTDFjorder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-04 07:32:29.462232 ctdfjorder-0.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 07:32:25.000000 ctdfjorder-0.0.39/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:32:29.462232 ctdfjorder-0.0.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-04 07:32:25.000000 ctdfjorder-0.0.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:11:45.204559 ctdfjorder-0.0.40/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:11:45.200559 ctdfjorder-0.0.40/CTDFjorder/
+-rw-r--r--   0 runner    (1001) docker     (127)    62118 2024-05-07 22:11:40.000000 ctdfjorder-0.0.40/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 22:11:40.000000 ctdfjorder-0.0.40/CTDFjorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:11:45.204559 ctdfjorder-0.0.40/CTDFjorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 22:11:45.204559 ctdfjorder-0.0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-07 22:11:40.000000 ctdfjorder-0.0.40/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:11:45.204559 ctdfjorder-0.0.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 22:11:40.000000 ctdfjorder-0.0.40/setup.py
```

### Comparing `ctdfjorder-0.0.39/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.40/CTDFjorder/CTDFjorder.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     """
     _ctd_array = pandas.DataFrame()
     _rsk = None
     _filename = None
     _calculator = None
     _cwd = None
-    _cached_master_sheet = None
+    _cached_master_sheet = pandas.DataFrame()
     master_sheet_path = "FjordPhyto MASTER SHEET.xlsx"
     _NO_SAMPLES_ERROR = "No samples in file."
     _NO_LOCATION_ERROR = "No location could be found."
     _DENSITY_CALCULATION_ERROR = "Could not calculate density on this dataset."
     _SALINITYABS_CALCULATION_ERROR = "Could not calculate density on this dataset."
     _DATA_CLEANING_ERROR = "No data remains after data cleaning, reverting to previous CTD"
     _REMOVE_NEGATIVES_ERROR = "No data remains after removing non-positive samples."
@@ -163,14 +163,22 @@
                 case 'salinityabs':
                     self._ctd_array = self.Utility.remove_rows_with_negative_salinityabs(self._ctd_array)
                 case 'density':
                     self._ctd_array = self.Utility.remove_rows_with_negative_density(self._ctd_array)
         if self.Utility.no_values_in_object(self._ctd_array):
             raise CTDError(self._filename, self._REMOVE_NEGATIVES_ERROR)
 
+    def remove_duplicate_depths(self):
+        """
+        Removes depths within 0.1 meters of each other.
+        """
+        if self.Utility.no_values_in_object(self._ctd_array):
+            raise CTDError(self._filename, self._NO_SAMPLES_ERROR)
+        self._ctd_array = self.Utility.remove_duplicate_depths(self._ctd_array.copy())
+
     def clean(self, feature, method='salinitydiff'):
         """
         Applies complex data cleaning methods to the specified feature based on the selected method.
         Currently supports cleaning practical salinity using the 'salinitydiff' method.
 
         Parameters
         ----------
@@ -396,17 +404,16 @@
         if df_filtered['overturn'].any():
             plt.title(
                 f"{filename}\n Depth vs. Salinity and Density with LOESS Transform "
                 f"\n THIS IS AN UNSTABLE WATER COLUMN "
                 f"\n(Higher density fluid lies above lower density fluid)")
         else:
             plt.title(
-                f"{filename}\n Depth vs. Salinity and Density with LOESS Transform "
-                f"\n THIS IS AN UNSTABLE WATER COLUMN "
-                f"\n(Higher density fluid lies above lower density fluid)")
+                f"{filename}\n Depth vs. Salinity and Density with LOESS Transform ")
+
         ax1.grid(True)
         lines, labels = ax1.get_legend_handles_labels()
         ax2_legend = ax2.get_legend_handles_labels()
         ax1.legend(lines + ax2_legend[0], labels + ax2_legend[1], loc='lower center', bbox_to_anchor=(0.5, -0.15),
                    ncol=3)
         plot_path = os.path.join(self._cwd, f"plots/{filename}_salinity_density_depth_plot_dual_x_axes_line.png")
         plot_folder = os.path.join(self._cwd, "plots")
@@ -462,17 +469,16 @@
         if df_filtered['overturn'].any():
             plt.title(
                 f"{filename}\n Depth vs. Salinity and Density "
                 f"\n THIS IS AN UNSTABLE WATER COLUMN "
                 f"\n(Higher density fluid lies above lower density fluid)")
         else:
             plt.title(
-                f"{filename}\n Depth vs. Salinity and Density "
-                f"\n THIS IS AN UNSTABLE WATER COLUMN "
-                f"\n(Higher density fluid lies above lower density fluid)")
+                f"{filename}\n Depth vs. Salinity and Density ")
+
         ax1.grid(True)
         lines, labels = ax1.get_legend_handles_labels()
         ax2_legend = ax2.get_legend_handles_labels()
         ax1.legend(lines + ax2_legend[0], labels + ax2_legend[1], loc='upper center', bbox_to_anchor=(0.5, -0.15),
                    ncol=3)
         plot_path = os.path.join(self._cwd, f"plots/{filename}_salinity_density_depth_plot_dual_x_axes.png")
         plot_folder = os.path.join(self._cwd, "plots")
@@ -523,17 +529,15 @@
         if df_filtered['overturn'].any():
             plt.title(
                 f"{filename}\n Depth vs. Temperature \n "
                 f"THIS IS AN UNSTABLE WATER COLUMN \n"
                 f"(Higher density fluid lies above lower density fluid)")
         else:
             plt.title(
-                f"{filename}\n Depth vs. Temperature \n "
-                f"THIS IS AN UNSTABLE WATER COLUMN \n"
-                f"(Higher density fluid lies above lower density fluid)")
+                f"{filename}\n Depth vs. Temperature \n ")
         ax1.grid(True)
         lines, labels = ax1.get_legend_handles_labels()
         ax1.legend(lines, labels, loc='upper center', bbox_to_anchor=(0.5, -0.15), ncol=3)
         plot_path = os.path.join(self._cwd, f"plots/{filename}_temperature_depth_plot.png")
         plot_folder = os.path.join(self._cwd, "plots")
         if not (os.path.isdir(plot_folder)):
             os.mkdir(plot_folder)
@@ -631,20 +635,18 @@
                 try:
                     df_hour, df_minute = [int(df_time_str.split(':')[0]), int(df_time_str.split(':')[1])]
                 except:
                     return None
                 return abs((target_hour * 60 + target_minute) - (df_hour * 60 + df_minute))
 
             # Check if the master sheet is already cached
-            if CTD._cached_master_sheet is None:
+            if CTD._cached_master_sheet.empty:
                 # Load the master sheet and cache it
                 CTD._cached_master_sheet = pd.read_excel(master_sheet_path)
-
-            # Use the cached master sheet data
-            master_df = CTD._cached_master_sheet.copy()
+            master_df = CTD._cached_master_sheet
             # Get date and time components from the filename
             year, month, day, time = get_date_from_string(filename)
             if year is None:
                 return
             # Calculate absolute differences for each row in 'master_df'
             master_df['date_difference'] = master_df.apply(date_difference, args=(year, month, day), axis=1)
             master_df['time_difference'] = master_df['time_local'].apply(lambda x: time_difference(time, x))
@@ -876,14 +878,47 @@
             if 'density' in df.columns:
                 df = df[df['density'] >= 0].reset_index(drop=True)
             else:
                 return None
             if self.no_values_in_object(df):
                 return None
             return df.copy()
+        def remove_duplicate_depths(self, df):
+            """
+            Removes rows from the given DataFrame where the 'depth' value is within 0.1 meters of another depth value,
+            prioritizes depths with lower timestamps.
+
+            Parameters
+            ----------
+            df: DataFrame
+                The DataFrame to process.
+
+            Returns
+            -------
+            DataFrame
+                The updated DataFrame with rows containing duplicate depths removed.
+            """
+            if self.no_values_in_object(df):
+                return None
+            if 'depth_00' in df.columns and 'timestamp' in df.columns:
+                # Sort by timestamp to ensure earlier records are prioritized
+                df = df.sort_values(by='timestamp')
+                # Round the depth values to the nearest 0.1 meters
+                df['rounded_depth'] = df['depth_00'].round(decimals=1)
+                # Drop duplicates based on the rounded depth values
+                df = df.drop_duplicates(subset='rounded_depth', keep='first')
+                # Reset index after removing duplicates
+                df = df.reset_index(drop=True)
+                # Remove the temporary 'rounded_depth' column
+                df.drop(columns=['rounded_depth'], inplace=True)
+            else:
+                return None
+            if self.no_values_in_object(df):
+                return None
+            return df.copy()
             
             
 class Calculate:
     """
     Calculate
     ----------
 
@@ -938,15 +973,15 @@
                 SA.isna() | CT.isna() | p.isna()
         )
         in_funnel[condition] = False
 
         return in_funnel
 
     @staticmethod
-    def calculate_and_drop_salinity_spikes(df):
+    def calculate_and_drop_salinity_spikes_slow(df):
         """
         Calculates and removes salinity spikes from the CTD data based on predefined thresholds for acceptable
         changes in salinity with depth.
 
         Parameters
         ----------
         df : DataFrame
@@ -975,15 +1010,15 @@
         # Check if there is enough depth range to calculate
         min_depth = df['depth_00'].min()
         max_depth = df['depth_00'].max()
         if min_depth == max_depth:
             print("Insufficient depth range to calculate.")
             return df
 
-        def recursively_drop(df, depth_range, acceptable_delta, i):
+        def recursively_drop(df, acceptable_delta, depth_range, i):
             try:
                 num_points = int((max_depth - min_depth) / depth_range)  # Calculate number of points
             except:
                 print("Error in calculating number of points.")
                 return df
             ranges = np.linspace(min_depth, max_depth, num=num_points)
 
@@ -998,14 +1033,49 @@
             return filtered_groups
 
         for i, deltas in enumerate(acceptable_delta_salinity_per_depth):
             df = recursively_drop(df, deltas[0], deltas[1], i)
         return df
 
     @staticmethod
+    def calculate_and_drop_salinity_spikes(df):
+        if df.empty:
+            return None
+
+        df['depth_00'] = pd.to_numeric(df['depth_00'], errors='coerce')
+        df['salinity_00'] = pd.to_numeric(df['salinity_00'], errors='coerce')
+        df = df.dropna(subset=['depth_00', 'salinity_00'])
+
+        min_depth = df['depth_00'].min()
+        max_depth = df['depth_00'].max()
+        if min_depth == max_depth:
+            print("Insufficient depth range to calculate.")
+            return df
+
+        acceptable_delta_salinity_per_depth = [
+            (0.0005, 0.001),
+            (0.005, 0.01),
+            (0.05, 0.1),
+            (0.5, 1),
+            (1, 2),
+
+        ]
+
+        for acceptable_delta, depth_range in acceptable_delta_salinity_per_depth:
+            num_points = int((max_depth - min_depth) / depth_range)
+            bins = np.linspace(min_depth, max_depth, num=num_points)
+            indices = np.digitize(df['depth_00'], bins)
+
+            # Group by indices and filter
+            grouped = df.groupby(indices)
+            df = grouped.filter(lambda x: abs(x['salinity_00'].max() - x['salinity_00'].min()) <= acceptable_delta)
+
+        return df
+
+    @staticmethod
     def calculate_overturns(ctd_array):
         """
         Calculates density overturns in the CTD data where denser water lies above lighter water with density
         difference of at least 0.05 kg/m³, which may indicate mixing or other dynamic processes.
 
         Parameters
         ----------
@@ -1258,22 +1328,25 @@
         self.message = message
         super().__init__(self.message)
 
 
 def run_default(plot=False):
     _reset_file_environment()
     CTD.master_sheet_path = os.path.join(_get_cwd(), "FjordPhyto MASTER SHEET.xlsx")
+    CTD._cached_master_sheet = pandas.read_excel(CTD.master_sheet_path)
     rsk_files_list = get_rsk_filenames_in_dir(_get_cwd())
     for file in rsk_files_list:
         try:
             my_data = CTD(file)
             my_data.add_filename_to_table()
             my_data.save_to_csv("output.csv")
             my_data.add_location_to_table()
+            my_data.remove_upcasts()
             my_data.remove_non_positive_samples()
+            my_data.remove_duplicate_depths()
             my_data.clean("practicalsalinity", 'salinitydiff')
             my_data.add_absolute_salinity()
             my_data.add_density()
             my_data.add_overturns()
             my_data.add_mld(1)
             my_data.add_mld(5)
             my_data.save_to_csv("outputclean.csv")
@@ -1284,14 +1357,15 @@
         except Exception as e:
             print(f"Error processing file: '{file}' {e}")
             continue
 
 
 def merge_all_in_folder():
     CTD.master_sheet_path = os.path.join(_get_cwd(), "FjordPhyto MASTER SHEET.xlsx")
+    CTD._cached_master_sheet = pandas.read_excel(CTD.master_sheet_path)
     rsk_files_list = get_rsk_filenames_in_dir(_get_cwd())
     for file in rsk_files_list:
         try:
             my_data = CTD(file)
             my_data.add_filename_to_table()
             my_data.add_location_to_table()
             my_data.save_to_csv("output.csv")
@@ -1327,16 +1401,17 @@
 
 
 def _get_filename(filepath):
     return '_'.join(filepath.split("/")[-1].split("_")[0:3]).split('.rsk')[0]
 
 def _reset_file_environment():
     CTD.master_sheet_path = os.path.join(_get_cwd(), "FjordPhyto MASTER SHEET.xlsx")
+    CTD._cached_master_sheet = pandas.read_excel(CTD.master_sheet_path)
     output_file_csv = "output.csv"
-    output_file_csv_clean = "output_clean.csv"
+    output_file_csv_clean = "outputclean.csv"
     output_plots_dir = "plots"
     cwd = _get_cwd()
     CTD.master_sheet_path = os.path.join(cwd, CTD.master_sheet_path)
     output_file_csv = os.path.join(cwd, output_file_csv)
     output_file_csv_clean = os.path.join(cwd, output_file_csv_clean)
     if cwd is None:
         raise CTDError("", "Couldn't get working directory.")
@@ -1372,14 +1447,15 @@
         file_path = sys.argv[2]
         try:
             ctd = CTD(file_path)
             ctd.add_filename_to_table()
             ctd.save_to_csv("output.csv")
             ctd.add_location_to_table()
             ctd.remove_non_positive_samples()
+            ctd.remove_upcasts()
             ctd.clean("practicalsalinity", 'salinitydiff')
             ctd.add_absolute_salinity()
             ctd.add_density()
             ctd.add_overturns()
             ctd.add_mld(0)
             ctd.add_mld(10)
             ctd.save_to_csv("outputclean.csv")
@@ -1408,8 +1484,9 @@
         print("  default                 Run the default processing pipeline")
         print("  defaultplotall          Run the default processing pipeline and create plots")
         print("CWD:")
         print(_get_cwd())
         sys.exit(1)
 
 if __name__ == "__main__":
+    run_default(True)
     main()
```

### Comparing `ctdfjorder-0.0.39/CTDFjorder.egg-info/PKG-INFO` & `ctdfjorder-0.0.40/CTDFjorder.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.39
+Version: 0.0.40
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
@@ -24,28 +24,33 @@
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: setuptools
 
 # CTDFjorder
 
 CTDFjorder is a Python package for processing and analyzing CTD (Conductivity, Temperature, Depth) data.
 Documentation: [Read the docs](https://nikothomas.github.io/CTDFjorder/CTDFjorder/CTDFjorder.html)
+GUI Wrapper: [ctdfjorder-lite](https://github.com/nikothomas/ctdfjorder-lite)
 
 ## Features
 
 - Read RSK files and extract CTD data
 - Process CTD data, including removing non-positive samples and cleaning data
 - Calculate derived quantities such as absolute salinity, density, and overturns
 - Determine mixed layer depth (MLD) using different methods
 - Generate plots for visualizing CTD profiles and derived quantities
 - Command-line interface (CLI) for easy processing and merging of RSK files
 
 ## Installation
-
-To install CTDFjorder, you can use pip:
-
+It's recommended that you create a new environment just for CTDFjorder. This can be done in conda with the following
+command.
+```shell
+conda create --name ctdfjorder -c conda-forge python=3.11
+conda activate ctdfjorder
+```
+To install CTDFjorder you can use pip:
 ```shell
 pip install ctdfjorder
 ```
 
 ## Usage
 
 CTDFjorder provides a command-line interface (CLI) for processing and analyzing CTD data. Here are the available commands:
@@ -124,15 +129,15 @@
     except Exception as e:
         print(f"Error processing file: '{file}' {e}")
         continue
 ```
 
 ## Contributing
 
-Contributions to CTDFjorder are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com).
+Contributions to CTDFjorder are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/nikothomas/CTDFjorder).
 
 ## License
 
 CTDFjorder is released under the MIT License.
 
 ## Acknowledgments
```

### Comparing `ctdfjorder-0.0.39/PKG-INFO` & `ctdfjorder-0.0.40/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.39
+Version: 0.0.40
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
@@ -24,28 +24,33 @@
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: setuptools
 
 # CTDFjorder
 
 CTDFjorder is a Python package for processing and analyzing CTD (Conductivity, Temperature, Depth) data.
 Documentation: [Read the docs](https://nikothomas.github.io/CTDFjorder/CTDFjorder/CTDFjorder.html)
+GUI Wrapper: [ctdfjorder-lite](https://github.com/nikothomas/ctdfjorder-lite)
 
 ## Features
 
 - Read RSK files and extract CTD data
 - Process CTD data, including removing non-positive samples and cleaning data
 - Calculate derived quantities such as absolute salinity, density, and overturns
 - Determine mixed layer depth (MLD) using different methods
 - Generate plots for visualizing CTD profiles and derived quantities
 - Command-line interface (CLI) for easy processing and merging of RSK files
 
 ## Installation
-
-To install CTDFjorder, you can use pip:
-
+It's recommended that you create a new environment just for CTDFjorder. This can be done in conda with the following
+command.
+```shell
+conda create --name ctdfjorder -c conda-forge python=3.11
+conda activate ctdfjorder
+```
+To install CTDFjorder you can use pip:
 ```shell
 pip install ctdfjorder
 ```
 
 ## Usage
 
 CTDFjorder provides a command-line interface (CLI) for processing and analyzing CTD data. Here are the available commands:
@@ -124,15 +129,15 @@
     except Exception as e:
         print(f"Error processing file: '{file}' {e}")
         continue
 ```
 
 ## Contributing
 
-Contributions to CTDFjorder are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com).
+Contributions to CTDFjorder are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/nikothomas/CTDFjorder).
 
 ## License
 
 CTDFjorder is released under the MIT License.
 
 ## Acknowledgments
```

### Comparing `ctdfjorder-0.0.39/README.md` & `ctdfjorder-0.0.40/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # CTDFjorder
 
 CTDFjorder is a Python package for processing and analyzing CTD (Conductivity, Temperature, Depth) data.
 Documentation: [Read the docs](https://nikothomas.github.io/CTDFjorder/CTDFjorder/CTDFjorder.html)
+GUI Wrapper: [ctdfjorder-lite](https://github.com/nikothomas/ctdfjorder-lite)
 
 ## Features
 
 - Read RSK files and extract CTD data
 - Process CTD data, including removing non-positive samples and cleaning data
 - Calculate derived quantities such as absolute salinity, density, and overturns
 - Determine mixed layer depth (MLD) using different methods
 - Generate plots for visualizing CTD profiles and derived quantities
 - Command-line interface (CLI) for easy processing and merging of RSK files
 
 ## Installation
-
-To install CTDFjorder, you can use pip:
-
+It's recommended that you create a new environment just for CTDFjorder. This can be done in conda with the following
+command.
+```shell
+conda create --name ctdfjorder -c conda-forge python=3.11
+conda activate ctdfjorder
+```
+To install CTDFjorder you can use pip:
 ```shell
 pip install ctdfjorder
 ```
 
 ## Usage
 
 CTDFjorder provides a command-line interface (CLI) for processing and analyzing CTD data. Here are the available commands:
@@ -98,15 +103,15 @@
     except Exception as e:
         print(f"Error processing file: '{file}' {e}")
         continue
 ```
 
 ## Contributing
 
-Contributions to CTDFjorder are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com).
+Contributions to CTDFjorder are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/nikothomas/CTDFjorder).
 
 ## License
 
 CTDFjorder is released under the MIT License.
 
 ## Acknowledgments
```

### Comparing `ctdfjorder-0.0.39/setup.py` & `ctdfjorder-0.0.40/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CTDFjorder",
-    version="0.0.39",
+    version="0.0.40",
     author="Nikolas Yanek-Chrones",
     author_email="nikojb1001@gmail.com",
     description="A package for processing and analyzing CTD data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nikothomas/CTDFjorder",
     project_urls={
```

