# Comparing `tmp/scintillometry-1.0.4.tar.gz` & `tmp/scintillometry-1.0.5.tar.gz`

## Comparing `scintillometry-1.0.4.tar` & `scintillometry-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/__init__.py
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/__init__.py
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/constants.py
--rw-r--r--   0        0        0    25114 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/constructions.py
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/derivations.py
--rw-r--r--   0        0        0    15739 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/iterations.py
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/transects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/metrics/__init__.py
--rwxr-xr-x   0        0        0    38541 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/metrics/calculations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/visuals/__init__.py
--rw-r--r--   0        0        0    31290 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/visuals/plotting.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/wrangler/__init__.py
--rw-r--r--   0        0        0    34241 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/wrangler/data_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0    27735 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/conftest.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_backend_constants.py
--rw-r--r--   0        0        0    28637 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_backend_constructions.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_backend_derivations.py
--rw-r--r--   0        0        0    12604 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_backend_iterations.py
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_backend_transects.py
--rw-r--r--   0        0        0    44917 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_metrics_calculations.py
--rw-r--r--   0        0        0    31368 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_visuals_plotting.py
--rw-r--r--   0        0        0    48525 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_wrangler_data_parser.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_data/test_data_v7_empty.mat
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_data/test_data_v7_results.mat
--rw-r--r--   0        0        0    10813 2020-02-02 00:00:00.000000 scintillometry-1.0.4/LICENSE
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 scintillometry-1.0.4/README.md
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 scintillometry-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    22589 2020-02-02 00:00:00.000000 scintillometry-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/__init__.py
+-rw-r--r--   0        0        0    13668 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/backend/__init__.py
+-rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/backend/constants.py
+-rw-r--r--   0        0        0    25113 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/backend/constructions.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/backend/deprecations.py
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/backend/derivations.py
+-rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/backend/iterations.py
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/backend/transects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/metrics/__init__.py
+-rwxr-xr-x   0        0        0    41883 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/metrics/calculations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/visuals/__init__.py
+-rw-r--r--   0        0        0    34520 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/visuals/plotting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/wrangler/__init__.py
+-rw-r--r--   0        0        0    34108 2020-02-02 00:00:00.000000 scintillometry-1.0.5/src/scintillometry/wrangler/data_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/__init__.py
+-rw-r--r--   0        0        0    28296 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/conftest.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_backend_constants.py
+-rw-r--r--   0        0        0    28637 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_backend_constructions.py
+-rw-r--r--   0        0        0    21589 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_backend_deprecations.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_backend_derivations.py
+-rw-r--r--   0        0        0    12637 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_backend_iterations.py
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_backend_transects.py
+-rw-r--r--   0        0        0    49439 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_metrics_calculations.py
+-rw-r--r--   0        0        0    33811 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_visuals_plotting.py
+-rw-r--r--   0        0        0    48521 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_wrangler_data_parser.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_data/test_data_v7_empty.mat
+-rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 scintillometry-1.0.5/tests/test_data/test_data_v7_results.mat
+-rw-r--r--   0        0        0    10813 2020-02-02 00:00:00.000000 scintillometry-1.0.5/LICENSE
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 scintillometry-1.0.5/README.md
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 scintillometry-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 scintillometry-1.0.5/PKG-INFO
```

### Comparing `scintillometry-1.0.4/src/scintillometry/main.py` & `scintillometry-1.0.5/src/scintillometry/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
                                     Default 850 nm.
     --beam-error <int>          Transmitter beam wavelength error, nm.
                                     Default 20 nm.
 """
 
 import argparse
 
-import scintillometry.metrics.calculations as MetricsCalculations
-import scintillometry.wrangler.data_parser as DataParser
+import scintillometry.metrics.calculations as calculations
+import scintillometry.wrangler.data_parser as data_parser
 
 
 def user_argumentation():
     """Parses user arguments when run as main.
 
     Required arguments:
         -i, --input <path>      Path to raw BLS450 data.
@@ -294,29 +294,29 @@
             would require `file_path = "./path/to/file_"`. Default None.
 
     Returns:
         dict: Parsed and labelled datasets for scintillometry
         measurements, weather observations, and topography.
     """
 
-    data_parser = DataParser.WranglerParsing()
+    parser = data_parser.WranglerParsing()
 
     # Parse BLS, weather, and topographical data
-    datasets = data_parser.wrangle_data(
+    datasets = parser.wrangle_data(
         bls_path=kwargs["input"],
         transect_path=kwargs["transect_path"],
         calibrate=kwargs["calibration"],
         station_id=kwargs["station_id"],
         tzone=kwargs["timezone"],
         weather_source="zamg",
     )
 
     # Parse vertical measurements
     if kwargs["profile_prefix"]:
-        datasets["vertical"] = data_parser.vertical.parse_vertical(
+        datasets["vertical"] = parser.vertical.parse_vertical(
             file_path=kwargs["profile_prefix"],
             source="hatpro",
             levels=None,
             tzone=kwargs["timezone"],
         )
 
     return datasets
@@ -356,19 +356,19 @@
 
     Returns:
         dict: Passes input datasets. If a path to eddy covariance data
         is provided, adds the key "eddy" containing the parsed eddy
         covariance data.
     """
 
-    metrics_class = MetricsCalculations.MetricsWorkflow()
-    data_parser = DataParser.WranglerParsing()
+    metrics_class = calculations.MetricsWorkflow()
+    parser = data_parser.WranglerParsing()
     metrics_data = metrics_class.calculate_standard_metrics(data=datasets, **kwargs)
     if kwargs["eddy_path"]:
-        eddy_frame = data_parser.eddy.parse_eddy_covariance(
+        eddy_frame = parser.eddy.parse_eddy_covariance(
             file_path=kwargs["eddy_path"], tzone=kwargs["timezone"], source="innflux"
         )
         metrics_data["eddy"] = eddy_frame
         metrics_class.compare_eddy(
             own_data=metrics_data["iteration"],
             ext_data=eddy_frame,
             source="innflux",
@@ -378,15 +378,15 @@
     return metrics_data
 
 
 def main():
     """Parses command line arguments and executes analysis.
 
     Converts command line arguments into kwargs. Imports and parses
-    scintillomter, weather, and transect data. If the appropriate
+    scintillometer, weather, and transect data. If the appropriate
     arguments are specified:
 
         - Parses vertical measurements
         - Calculates sensible heat fluxes
         - Compares calculated fluxes to external data.
 
     The majority of kwarg expansions should occur in this module. Do not
```

### Comparing `scintillometry-1.0.4/src/scintillometry/backend/constants.py` & `scintillometry-1.0.5/src/scintillometry/backend/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,14 @@
     Attributes:
         alpha11 (dict): |Cn2| measurement coefficients |a_11| for each
             BLS type, [|m^(7/3)|].
         alpha12 (dict): |Cn2| measurement coefficients |a_12| for each
             BLS type.
         lamda (float): BLS wavelength, |lamda| [nm].
         lamda_error (float): BLS wavelength error, [nm].
-        m1_opt (float): Needed for |A_T| and |A_q|, from Owens (1967).
-            [#owens1967]_
-        m2_opt (float): Needed for |A_T| and |A_q|, from Owens (1967).
-            [#owens1967]_
 
         at_opt (float): |A_T| coefficient for 880 nm & typical
             atmospheric conditions, from Ward et al. (2013).
             [#ward2013]_
         aq_opt (float): |A_q| coefficient for 880 nm & typical
             atmospheric conditions, Ward et al. (2013). [#ward2013]_
 
@@ -56,15 +52,15 @@
         g (float): Gravitational acceleration [|ms^-2|].
         k (float): von Kármán's constant.
         kelvin (float): 0°C in kelvins.
         latent_vapour (float): Latent heat of vapourisation at
             20°C [|Jkg^-1|].
         r_dry (float): Specific gas constant for dry air,
             |R_dry| [|JK^-1| |kg^-1|].
-        r_vapour (float): Specific gas contstant for water vapour,
+        r_vapour (float): Specific gas constant for water vapour,
             |R_v| [|JK^-1| |kg^-1|].
         ratio_rmm (float): Ratio of molecular masses of water vapour and
             dry air i.e. ratio of gas constants |epsilon|.
         ref_pressure (int): Reference pressure (not SLP), |P_b| [Pa].
         rho (float): Density of air at STP, |rho| [|kgm^-3|].
 
     """
@@ -145,15 +141,15 @@
         This method should therefore only be used on pre-processed data
         as a *convenience*. By default, converts to pascals.
 
         Args:
             pressure (Union[pd.DataFrame, pd.Series]): Pressure
                 measurements |P| in pascals [Pa], hectopascals [hPa], or
                 bars [bar].
-            base (bool): If True, converts to pascals [Pa]. Otherwise
+            base (bool): If True, converts to pascals [Pa]. Otherwise,
                 converts to hectopascals [hPa]. Default True.
 
         Returns:
             Union[pd.DataFrame, pd.Series]: Pressure measurements |P| in
             either pascals [Pa] or hectopascals [hPa].
         """
 
@@ -182,20 +178,20 @@
         This method handles 0 and NaN values, but only converts
         correctly for temperature values in these intervals:
 
         - T [K] > 130 K
         - T [°C] < 130 °C
 
         This method should therefore only be used on pre-processed data
-        as a *convenience*. By default converts to kelvins.
+        as a *convenience*. By default, converts to kelvins.
 
         Args:
             temperature (Union[pd.DataFrame, pd.Series]): Temperature
                 measurements |T| in kelvins [K] or Celsius [°C].
-            base (bool): If True, converts to kelvins [K]. Otherwise
+            base (bool): If True, converts to kelvins [K]. Otherwise,
                 converts to Celsius [°C]. Default True.
 
         Returns:
             Union[pd.DataFrame, pd.Series]: Temperature measurements |T|
             in either kelvins [K] or Celsius [°C].
         """
```

### Comparing `scintillometry-1.0.4/src/scintillometry/backend/constructions.py` & `scintillometry-1.0.5/src/scintillometry/backend/constructions.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         Returns:
             pd.DataFrame: Derived vertical measurements for mixing
             ratio, |r| [|kgkg^-1|].
         """
 
         # (wv_pressure * self.r_dry) / (d_pressure * self.r_vapour)
         m_ratio = (wv_pressure.multiply(self.constants.r_dry)).divide(
-            (d_pressure).multiply(self.constants.r_vapour)
+            d_pressure.multiply(self.constants.r_vapour)
         )
 
         return m_ratio
 
     def get_virtual_temperature(self, temperature, mixing_ratio):
         """Derive virtual temperature from vertical measurements.
 
@@ -232,15 +232,15 @@
             station_pressure (pd.DataFrame): Vertical measurements,
                 pressure relative to station elevation, |P_z| [Pa].
             virtual_temperature (pd.DataFrame): Vertical measurements,
                 virtual temperature, |T_v| [K].
             elevation (float): Station elevation, |z_stn| [m].
 
         Returns:
-            pd.DataDrame: Derived vertical measurements for mean
+            pd.DataFrame: Derived vertical measurements for mean
             sea-level pressure, |P_MSL| [Pa].
         """
 
         # station_pressure * np.exp(
         #     elevation / (virtual_temperature * (self.r_dry / np.abs(self.g)))
         # )
         alpha = self.constants.r_dry / np.abs(self.constants.g)
@@ -491,15 +491,15 @@
 
         Calculates |dy/dx| at each value of independent variable x for
         each time step t(n): e.g. an input dataframe of temperatures |T|
         for heights |z| with time index t, returns a dataframe of
         :math:`\\partial T/\\partial z` for heights |z| with time
         index t.
 
-        By default the gradient is calculated using a 1-D
+        By default, the gradient is calculated using a 1-D
         centred-differencing scheme for non-uniform meshes, since
         vertical measurements are rarely made at uniform intervals.
 
         Args:
             data (pd.DataFrame): Vertical measurements for a single
                 variable.
             method (str): Finite differencing method. Supports "uneven"
```

### Comparing `scintillometry-1.0.4/src/scintillometry/backend/derivations.py` & `scintillometry-1.0.5/src/scintillometry/backend/derivations.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.4/src/scintillometry/backend/iterations.py` & `scintillometry-1.0.5/src/scintillometry/backend/iterations.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,14 +325,16 @@
             dataframe (pd.DataFrame): Parsed, localised dataframe row
                 containing at least |CT2|, wind speed, air density,
                 and temperature.
             zm_bls (float): Effective height of scintillometer.
             stable_flag (bool): Stability conditions. If true, assumes
                 stable conditions, otherwise assumes unstable
                 conditions.
+            most_coeffs (list): MOST coefficients for unstable and
+                stable conditions.
 
         Returns:
             pd.DataFrame: Dataframe with additional columns for Obukhov
             lengths, sensible heat fluxes, frictional velocity, and
             temperature scale.
         """
```

### Comparing `scintillometry-1.0.4/src/scintillometry/backend/transects.py` & `scintillometry-1.0.5/src/scintillometry/backend/transects.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,24 +81,24 @@
         """Gets b-value for an implemented stability condition.
 
         Args:
             stability_name (str): Name of stability condition.
 
         Returns:
             float: Constant "b" accounting for height dependence of
-                |Cn2|. Values of "b" are from Hartogenesis et al.
+                |Cn2|. Values of "b" are from Hartogensis et al.
                 (2003) [#hartogensis2003]_, and Kleissl et al.
                 (2008) [#kleissl2008]_.
 
         Raises:
             NotImplementedError: <stability_name> is not an implemented
                 stability condition.
         """
 
-        # Hartogenesis et al. (2003), Kleissl et al. (2008).
+        # Hartogensis et al. (2003), Kleissl et al. (2008).
         stability_dict = {"stable": -2 / 3, "unstable": -4 / 3}
 
         if not stability_name:
             b_value = 1
         elif stability_name.lower() in stability_dict:
             b_value = stability_dict[stability_name]
         else:
@@ -164,17 +164,17 @@
     def get_all_path_heights(self, path_transect):
         """Calculates effective & mean path heights in all conditions.
 
         Args:
             path_transect (pd.DataFrame): Parsed path transect data.
 
         Returns:
-            dict[tuple[np.floating, np.floating]]: Effective and mean
-            path heights of transect |z_eff| and |z_mean| [m], with each
-            stability condition as key.
+            dict[str, tuple[np.floating, np.floating]]: Effective and
+            mean path heights of transect |z_eff| and |z_mean| [m], with
+            each stability condition as key.
         """
 
         path_heights_dict = {}
         for stability in ["stable", "unstable", None]:
             path_heights = self.get_path_heights(
                 transect_data=path_transect, stability_condition=stability
             )
```

### Comparing `scintillometry-1.0.4/src/scintillometry/metrics/calculations.py` & `scintillometry-1.0.5/src/scintillometry/metrics/calculations.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 =====
 
 Calculates metrics from datasets.
 """
 
 import kneed
 import pandas as pd
+from sklearn.linear_model import LinearRegression
 
-from scintillometry.backend.iterations import IterationMost
 from scintillometry.backend.constants import AtmosConstants
 from scintillometry.backend.constructions import ProfileConstructor
 from scintillometry.backend.derivations import DeriveScintillometer
+from scintillometry.backend.iterations import IterationMost
 from scintillometry.backend.transects import TransectParameters
 from scintillometry.visuals.plotting import FigurePlotter
+from scintillometry.backend.deprecations import Decorators
 
 
 class MetricsTopography:
     """Calculate metrics for topographical data.
 
     Attributes:
         transect (TransectParameters): Inherited methods for calculating
@@ -51,16 +53,17 @@
         Select the stability conditions using ``--r, --regime <str>``.
 
         Args:
             transect (pd.DataFrame): Parsed path transect data.
             regime (str): Target stability condition. Default None.
 
         Returns:
-            dict[float, float]: Tuples of effective and mean path height
-            |z_eff| and |z_mean| [m], with stability conditions as keys.
+            dict[str, tuple[np.floating, np.floating]]: Tuples of
+            effective and mean path height |z_eff| and |z_mean| [m],
+            with stability conditions as keys.
         """
 
         z_params = self.transect.get_all_path_heights(path_transect=transect)
 
         self.transect.print_path_heights(
             z_eff=z_params[str(regime)][0],
             z_mean=z_params[str(regime)][1],
@@ -101,15 +104,14 @@
         comparison between the computed flux and the flux recorded by
         the scintillometer, and saves the figure to disk.
 
         Warning: this will overwrite existing values for |CT2| in
         <interpolated_data>.
 
         Args:
-            user_args (argparse.Namespace): Namespace of user arguments.
             interpolated_data (pd.DataFrame): Dataframe containing
                 parsed and localised weather and scintillometer data
                 with matching temporal resolution.
             z_eff (np.floating): Effective path height, z_eff| [m].
             beam_wavelength (int): Transmitter beam wavelength, nm.
                 Default 880 nm.
             beam_error (int): Transmitter beam error, nm. Default 20 nm.
@@ -171,15 +173,15 @@
 
         Returns:
             dict: If the input dictionary contained a dictionary under
             the key "vertical" measurements, the dictionary under
             "vertical" is updated with vertical data for water vapour
             pressure, air pressure, mixing ratio, virtual temperature,
             mean sea-level pressure, and potential temperature.
-            Otherwise the dictionary is returned unmodified.
+            Otherwise, the dictionary is returned unmodified.
         """
 
         if "vertical" in data:
             data["vertical"] = self.construction.get_vertical_variables(
                 vertical_data=data["vertical"], meteo_data=data["weather"]
             )
 
@@ -212,14 +214,49 @@
         if not series_match.empty:
             match_time = series_match.dropna().index[0]
         else:
             match_time = None
 
         return match_time
 
+    def get_regression(self, x_data, y_data, intercept=True):
+        """Performs regression on labelled data.
+
+        Args:
+            x_data (pd.Series): Labelled explanatory data.
+            y_data (pd.Series): Labelled response data.
+            intercept (bool): If True, calculate intercept (e.g. data is
+            not centred). Default True.
+
+        Returns:
+            dict: Contains the fitted estimator for regression data, the
+            coefficient of determination |R^2|, and predicted values for
+            a fitted regression line.
+        """
+
+        scatter_frame = pd.merge(
+            x_data, y_data, left_index=True, right_index=True, sort=True
+        )
+        scatter_frame = scatter_frame.dropna(axis=0)
+        x_fit_data = scatter_frame.iloc[:, 0].values.reshape(-1, 1)
+        y_fit_data = scatter_frame.iloc[:, 1].values.reshape(-1, 1)
+
+        linear_regressor = LinearRegression(fit_intercept=intercept)
+        estimator = linear_regressor.fit(x_fit_data, y_fit_data)
+        score = estimator.score(x_fit_data, y_fit_data)
+        predictions = linear_regressor.predict(x_fit_data)
+
+        regression = {
+            "fit": estimator,
+            "score": score,
+            "regression_line": predictions,
+        }
+
+        return regression
+
     def get_elbow_point(self, series, min_index=None, max_index=None):
         """Calculate elbow point using Kneedle algorithm.
 
         Only supports convex curves. Noisier curves may have several
         elbow points, in which case the function selects the smallest
         acceptable index.
 
@@ -243,18 +280,18 @@
             if not min_index:
                 min_index = series.index[0]
             indices = series.index[
                 (series.index >= min_index) & (series.index <= max_index)
             ]
         if series[indices[-1]] < series[indices[0]]:
             curve_direction = "decreasing"
-            online_param = "true"
+            online_param = True
         else:
             curve_direction = "increasing"
-            online_param = "true"
+            online_param = True
         knee = kneed.KneeLocator(
             series[indices],
             indices,
             S=1.5,
             curve="convex",
             online=online_param,
             direction=curve_direction,
@@ -357,19 +394,19 @@
             local_time (pd.Timestamp): Local time of switch between
                 stability conditions.
             bl_height (float): Boundary layer height, [m]. Default None.
             location (str): Location of data collection. Default empty
                 string.
 
         Returns:
-            tuple[plt.Figure, plt.Axes, plt.Figure, plt.Axes]: Vertical
-            profiles of lapse rates on a single axis, and vertical
-            profiles of parcel temperatures on a single axis. If a
-            boundary layer height is provided, vertical lines denoting
-            its height are added to the figures.
+            list[tuple[plt.Figure, plt.Axes]]: Vertical profiles of
+            lapse rates on a single axis, and vertical profiles of
+            parcel temperatures on a single axis. If a boundary layer
+            height is provided, vertical lines denoting its height are
+            added to the figures.
         """
 
         lapse_rates = {
             "environmental_lapse_rate": vertical_data["environmental_lapse_rate"],
             "moist_adiabatic_lapse_rate": vertical_data["moist_adiabatic_lapse_rate"],
         }
         round_time = self.get_nearest_time_index(
@@ -408,15 +445,15 @@
         )
         self.plotting.save_figure(
             figure=fig_parcel,
             timestamp=round_time,
             suffix=f"{round_time.strftime('%H%M')}_parcel_temperatures",
         )
 
-        return fig_lapse, axes_lapse, fig_parcel, axes_parcel
+        return [(fig_lapse, axes_lapse), (fig_parcel, axes_parcel)]
 
     def get_switch_time_vertical(self, data, method="static", ri_crit=0.25):
         """Gets local time of switch between stability conditions.
 
         Pass one of the following to the <method> argument:
 
         - **eddy**: eddy covariance (NotImplemented)
@@ -577,18 +614,18 @@
             local_time (pd.Timestamp): Local time of switch between
                 stability conditions.
             location (str): Location of data collection. Default empty
                 string.
             bl_height (int): Boundary layer height. Default None.
 
         Returns:
-            tuple[plt.Figure, plt.Axes]: Vertical profile of potential
-            temperature. If the gradient potential temperature is also
-            provided, the two vertical profiles are placed side-by-side
-            in separate subplots.
+            list[tuple[plt.Figure, plt.Axes]]: Vertical profile of
+            potential temperature. If the gradient potential temperature
+            is also provided, the two vertical profiles are placed
+            side-by-side in separate subplots.
         """
 
         round_time = self.get_nearest_time_index(
             data=data["potential_temperature"], time_stamp=local_time
         )
         mil_time = round_time.strftime("%H%M")
 
@@ -630,15 +667,15 @@
             )
             self.plotting.save_figure(
                 figure=fig_grad,
                 timestamp=local_time,
                 suffix=f"{mil_time}_gradient_potential_temperature_2km",
             )
 
-        return fig, ax
+        return [(fig, ax)]
 
     def calculate_switch_time(
         self, datasets, method="sun", switch_time=None, location=""
     ):
         """Calculates and plots local time of switch in stability.
 
         Optionally uses vertical measurements in a dictionary under
@@ -699,17 +736,17 @@
         location="",
     ):
         """Compute sensible heat fluxes with MOST through iteration.
 
         Trades speed from vectorisation for more accurate convergence.
 
         Args:
-            z_parameters (dict[float, float]): Tuples of effective and
-                mean path height |z_eff| and |z_mean| [m], with
-                stability conditions as keys.
+            z_parameters (dict[str, tuple[float, float]): Tuples of
+                effective and mean path height |z_eff| and |z_mean| [m],
+                with stability conditions as keys.
             datasets (dict): Contains parsed, tz-aware dataframes, with
                 at least |CT2|, wind speed, air density, and
                 temperature.
             most_id (str): MOST coefficients for unstable and stable
                 conditions. Default "an1988".
             algorithm (str): Method to calculate switch time.
                 Default "sun".
@@ -769,50 +806,70 @@
             time_id (pd.Timestamp): Start time of scintillometer data
                 collection.
             regime (str): Stability condition. Default None.
             location (str): Location of data collection. Default empty
             string.
 
         Returns:
-            tuple[plt.Figure, plt.Axes]: Time series comparing sensible
-            heat fluxes under free convection to on-board software.
+            list[tuple[plt.Figure, plt.Axes]]: Time series comparing
+            sensible heat fluxes under free convection to on-board
+            software.
         """
 
         fig_convection, ax_convection = self.plotting.plot_convection(
             dataframe=derived_data, stability=regime, site=location
         )
         self.plotting.save_figure(
             figure=fig_convection, timestamp=time_id, suffix="free_convection"
         )
+        derived_plots = [(fig_convection, ax_convection)]
 
-        return fig_convection, ax_convection
+        return derived_plots
 
-    def plot_iterated_metrics(self, iterated_data, time_stamp, site_location=""):
-        """Plot and save time series and comparison of iterated fluxes.
+    @Decorators.deprecated_argument(
+        stage="pending", version="1.0.5", site_location="location"
+    )
+    def plot_iterated_metrics(self, iterated_data, time_stamp, location=""):
+        """Plots and saves iterated SHF, comparison to free convection.
+
+        .. todo::
+            ST-126: Deprecate the argument `site_location` for
+                `location`.
 
         Args:
-            user_args (argparse.Namespace): Namespace of user arguments.
-            derived_data (pd.DataFrame): Interpolated tz-aware dataframe
-                with columns for sensible heat fluxes calculated with
-                MOST and for free convection.
-            time_id (pd.Timestamp): Start time of scintillometer data
-                collection.
-            site_location (str): Name of scintillometer location.
+            iterated_data (pd.DataFrame): TZ-aware with columns for
+                sensible heat fluxes calculated for free convection
+                |H_free|, and by MOST |H|.
+            time_stamp (pd.Timestamp): Local time of data collection.
+            location (str): Location of data collection. Default empty
+                string.
 
         Returns:
-            tuple[plt.Figure, plt.Axes, plt.Figure, plt.Axes]: Time
-            series of sensible heat flux calculated through MOST, and a
-            comparison to sensible heat flux under free convection.
+            list[tuple[plt.Figure, plt.Axes]]: Time series of sensible
+            heat flux calculated through MOST, and a comparison to
+            sensible heat flux under free convection.
         """
 
-        plots = self.plotting.plot_iterated_fluxes(
-            iteration_data=iterated_data, time_id=time_stamp, location=site_location
+        shf_plot = self.plotting.plot_generic(iterated_data, "shf", site=location)
+        self.plotting.save_figure(
+            figure=shf_plot[0], timestamp=time_stamp, suffix="shf"
         )
 
-        return plots
+        comparison_plot = self.plotting.plot_comparison(
+            df_01=iterated_data,
+            df_02=iterated_data,
+            keys=["H_free", "shf"],
+            labels=["Free Convection", "Iteration"],
+            site=location,
+        )
+        self.plotting.save_figure(
+            figure=comparison_plot[0], timestamp=time_stamp, suffix="shf_comp"
+        )
+
+        return [shf_plot, comparison_plot]
 
 
 class MetricsWorkflow(MetricsFlux, MetricsTopography):
     """Standard workflow for metrics."""
 
     def __init__(self):
         super().__init__()
@@ -832,15 +889,15 @@
         """Calculates and plots metrics from wrangled data.
 
         This wrapper function:
 
         - Calculates effective path heights for all stability
           conditions.
         - Derives |CT2| and sensible heat flux for free convection.
-        - Estimates the time where stability conditions change.
+        - Estimates the time when stability conditions change.
         - Calculates sensible heat flux using MOST.
         - Plots time series comparing sensible heat flux for free
           convection |H_free| to on-board software, time series of
           sensible heat flux calculated with MOST |H|, and a comparison
           to sensible heat flux for free convection.
         - Saves plots to disk.
 
@@ -916,104 +973,142 @@
             switch_time=switch_time,
             location=location,
         )
 
         self.plot_iterated_metrics(
             iterated_data=iterated_dataframe,
             time_stamp=data_timestamp,
-            site_location=location,
+            location=location,
         )
 
         data["derivation"] = derived_dataframe
         data["iteration"] = iterated_dataframe
 
         return data
 
     def compare_innflux(self, own_data, innflux_data, location=""):
-        """Compares SHF and Obukhov lengths to InnFLUX measurements.
+        """Compares SHF and Obukhov lengths to innFLUX measurements.
 
         This wrapper function:
 
         - Plots time series comparing Obukhov lengths and sensible heat
           fluxes between an input dataframe and innFLUX measurements.
         - Saves plots to disk.
 
         If this function is imported as a package, mock user arguments
         with an argparse.Namespace object.
 
         Args:
-            arguments (argparse.Namespace): User arguments.
             own_data (pd.DataFrame): Labelled data for SHF and Obukhov
                 length.
             innflux_data (pd.DataFrame): Eddy covariance data from
                 innFLUX.
             location (str): Location of data collection. Default empty
                 string.
 
         Returns:
-            tuple[plt.Figure, plt.Axes, plt.Figure, plt.Axes]: Time
-            series comparing Obukhov length and sensible heat flux to
-            innFlux measurements.
+            list[tuple[plt.Figure, plt.Axes]]: Time series comparing
+            Obukhov length and sensible heat flux to innFLUX
+            measurements.
         """
 
         data_timestamp = own_data.index[0]
-        fig_obukhov, ax_obukhov = self.plotting.plot_innflux(
+        obukhov_plot = self.plotting.plot_innflux(
             iter_data=own_data,
             innflux_data=innflux_data,
             name="obukhov",
             site=location,
         )
         self.plotting.save_figure(
-            figure=fig_obukhov, timestamp=data_timestamp, suffix="innflux_obukhov"
+            figure=obukhov_plot[0], timestamp=data_timestamp, suffix="innflux_obukhov"
+        )
+        obukhov_regression = self.get_regression(
+            x_data=own_data["obukhov"], y_data=innflux_data["obukhov"], intercept=True
+        )
+        obukhov_regression_plot = self.plotting.plot_scatter(
+            x_data=own_data["obukhov"],
+            y_data=innflux_data["obukhov"],
+            sources=["MOST Iteration", "innFLUX"],
+            name="obukhov",
+            score=obukhov_regression["score"],
+            regression_line=obukhov_regression["regression_line"],
+            site=location,
+        )
+        self.plotting.save_figure(
+            figure=obukhov_regression_plot[0],
+            timestamp=data_timestamp,
+            suffix="innflux_obukhov_regression",
         )
-        fig_shf, ax_shf = self.plotting.plot_innflux(
+
+        shf_plot = self.plotting.plot_innflux(
             iter_data=own_data,
             innflux_data=innflux_data,
             name="shf",
             site=location,
         )
         self.plotting.save_figure(
-            figure=fig_shf, timestamp=data_timestamp, suffix="innflux_shf"
+            figure=shf_plot[0], timestamp=data_timestamp, suffix="innflux_shf"
+        )
+        shf_regression = self.get_regression(
+            x_data=own_data["obukhov"], y_data=innflux_data["obukhov"], intercept=True
+        )
+        shf_regression_plot = self.plotting.plot_scatter(
+            x_data=own_data["shf"],
+            y_data=innflux_data["shf"],
+            sources=["MOST Iteration", "innFLUX"],
+            name="shf",
+            score=shf_regression["score"],
+            regression_line=shf_regression["regression_line"],
+            site=location,
+        )
+        self.plotting.save_figure(
+            figure=shf_regression_plot[0],
+            timestamp=data_timestamp,
+            suffix="innflux_shf_regression",
         )
 
-        return fig_obukhov, ax_obukhov, fig_shf, ax_shf
+        plots = [obukhov_plot, shf_plot, obukhov_regression_plot, shf_regression_plot]
+
+        return plots
 
     def compare_eddy(self, own_data, ext_data, source="innflux", location=""):
         """Compares data to an external source of eddy covariance data.
 
         Plots and saves time series comparing Obukhov lengths and
         sensible heat fluxes between an input dataframe and external
         eddy covariance measurements.
 
         If this function is imported as a package, mock user arguments
         with an argparse.Namespace object.
 
         Args:
-            arguments (argparse.Namespace): User arguments.
             own_data (pd.DataFrame): Labelled data.
             ext_data (pd.DataFrame): Eddy covariance data from an
                 external source.
+            source (str): Data source of vertical measurements.
+                Currently supports processed innFLUX data.
+                Default "innflux".
             location (str): Location of data collection. Default empty
                 string.
 
         Returns:
-            tuple[plt.Figure, plt.Axes, plt.Figure, plt.Axes]: Time
-            series comparing Obukhov length and sensible heat flux to
-            innFlux measurements.
+            list[tuple[plt.Figure, plt.Axes]]: Time series comparing
+            Obukhov length and sensible heat flux to innFLUX
+            measurements.
 
         Raises:
             NotImplementedError: <source> measurements are not
                 supported. Use "innflux".
 
         """
 
         if source.lower() == "innflux":
-            fig_obukhov, ax_obukhov, fig_shf, ax_shf = self.compare_innflux(
+            eddy_plots = self.compare_innflux(
                 own_data=own_data, innflux_data=ext_data, location=location
             )
         else:
             error_msg = (
                 f"{source.title()} measurements are not supported. Use 'innflux'."
             )
             raise NotImplementedError(error_msg)
 
-        return fig_obukhov, ax_obukhov, fig_shf, ax_shf
+        return eddy_plots
```

### Comparing `scintillometry-1.0.4/src/scintillometry/visuals/plotting.py` & `scintillometry-1.0.5/src/scintillometry/visuals/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 import math
 import os
 import re
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
+from scintillometry.backend.deprecations import Decorators
 
 
 class FigureFormat:
     """Regulates plot annotations and formatting."""
 
     def __init__(self):
         super().__init__()
@@ -87,16 +89,16 @@
             plt.ylabel(y_label)
 
     def get_site_name(self, site_name, dataframe=None):
         """Gets name of site from user string or dataframe metadata.
 
         Args:
             site_name (str): Location of data collection.
-            dataframe (pd.DataFrame): Any collected dataset. Default
-                None.
+            dataframe (pd.DataFrame or pd.Series): Any collected
+                dataset. Default None.
 
         Returns:
             str: Location of data collection. Returns empty string if no
             user argument or metadata was found.
         """
 
         if site_name:
@@ -189,15 +191,16 @@
 
         return label
 
     def get_date_and_timezone(self, data):
         """Return first time index and timezone.
 
         Args:
-            data (pd.DataFrame): TZ-aware dataframe with DatetimeIndex.
+            data (pd.DataFrame or pd.Series): TZ-aware dataframe with
+                DatetimeIndex.
 
         Returns:
             dict[str, datetime.tzinfo]: Date formatted as
             "DD Month YYYY", and timezone object.
         """
 
         date = data.index[0].strftime("%d %B %Y")
@@ -223,15 +226,15 @@
             location = ""  # Otherwise None interpreted literally in f-strings
         else:
             location = f" at {location}"
 
         if not isinstance(timestamp, str):
             timestamp = timestamp.strftime("%d %B %Y")
 
-        title_string = "".join((f"{title}{location},\n{timestamp}"))
+        title_string = f"{title}{location},\n{timestamp}"
         plt.title(title_string, fontweight="bold")
         plt.legend(loc="upper left")
 
         return title_string
 
     def merge_label_with_unit(self, label):
         """Merges variable name with its unit if applicable.
@@ -258,15 +261,15 @@
     def merge_multiple_labels(self, labels):
         """Merges multiple labels into a single formatted string.
 
         Args:
             labels (list[str]): Labels, which may contain duplicates.
 
         Returns:
-            str: A formatted, puncutated string with no duplicates.
+            str: A formatted, punctuated string with no duplicates.
         """
 
         unique_text = list(dict.fromkeys(labels))
         if len(unique_text) < 2:
             merged = f"{unique_text[0]}"
         elif len(unique_text) == 2:
             merged = " and ".join(unique_text)
@@ -280,17 +283,17 @@
 
         Args:
             ax (plt.Axes): Plot's axes.
             timezone (datetime.tzinfo): Local timezone of data.
             name (str): Name or abbreviation of dependent variable.
 
         Returns:
-            plt.Axes: Plot axes with labels for local time on the x axis
-            and for the dependent variable with units on the y axis.
-            Ticks on the x axis are formatted at hourly intervals.
+            plt.Axes: Plot axes with labels for local time on the x-axis
+            and for the dependent variable with units on the y-axis.
+            Ticks on the x-axis are formatted at hourly intervals.
         """
 
         x_label = f"Time, {timezone.zone}"
         label_text = self.label_selector(dependent=name)
         y_label = self.merge_label_with_unit(label=label_text)
 
         plt.xlabel(x_label)
@@ -576,27 +579,42 @@
             title=title_string, timestamp=plot_tzone["date"], location=site_label
         )
         axes = plt.gca()
         self.set_xy_labels(ax=axes, timezone=plot_tzone["tzone"], name=keys[1])
 
         return figure, axes
 
+    @Decorators.deprecated(
+        stage="pending",
+        reason="Superseded by MetricsFlux.plot_iterated_metrics.",
+        version="1.0.5",
+    )
     def plot_iterated_fluxes(self, iteration_data, time_id, location=""):
         """Plots and saves iterated SHF, comparison to free convection.
 
+        .. note:: Pending deprecation in a future patch release. Use
+            :func:`MetricsFlux.plot_iterated_metrics()
+            <scintillometry.metrics.calculations.MetricsFlux.plot_iterated_metrics>`
+            instead.
+
+        .. todo::
+            ST-126: Deprecate FigurePlotter.plot_iterated_fluxes in
+                favour of plot_iterated_metrics.
+
         Args:
             iteration_data (pd.DataFrame): TZ-aware with sensible heat
                 fluxes calculated for free convection |H_free|, and
                 MOST |H|.
             time_id (pd.Timestamp): Local time of data collection.
             location (str): Location of data collection. Default empty
                 string.
 
         Returns:
-            tuple[plt.Figure, plt.Figure]: Time series and comparison.
+            list[tuple[plt.Figure, plt.Axes]]: Time series and
+            comparison.
         """
 
         fig_shf, ax_shf = self.plot_generic(iteration_data, "shf", site=location)
         fig_shf = plt.gcf()
         self.save_figure(figure=fig_shf, timestamp=time_id, suffix="shf")
 
         fig_comp, ax_comp = self.plot_comparison(
@@ -605,15 +623,15 @@
             keys=["H_free", "shf"],
             labels=["Free Convection", "Iteration"],
             site=location,
         )
         fig_comp = plt.gcf()
         self.save_figure(figure=fig_comp, timestamp=time_id, suffix="shf_comp")
 
-        return fig_shf, ax_shf, fig_comp, ax_comp
+        return [(fig_shf, ax_shf), (fig_comp, ax_comp)]
 
     def plot_innflux(self, iter_data, innflux_data, name="obukhov", site=""):
         """Plots comparison between scintillometer and InnFLUX data.
 
         Args:
             iter_data (pd.DataFrame): Iterated data from scintillometer.
             innflux_data (pd.DataFrame): InnFLUX data.
@@ -650,27 +668,90 @@
             title=title_string, timestamp=iter_tzone["date"], location=site_label
         )
         axes = plt.gca()
         self.set_xy_labels(ax=axes, timezone=iter_tzone["tzone"], name=name)
 
         return figure, axes
 
+    def plot_scatter(
+        self, x_data, y_data, name, sources, score=None, regression_line=None, site=""
+    ):
+        """Plots scatter between two datasets with a regression line.
+
+        Args:
+            x_data (pd.Series): Labelled explanatory data.
+            y_data (pd.Series): Labelled response data.
+            name (str): Name of variable.
+            sources (list[str, str]): Names of data sources formatted
+                as: [<Explanatory Source>, <Response Source>].
+            score (float): Coefficient of determination |R^2|.
+                Default None.
+            regression_line (np.ndarray): Values for regression line.
+                Default None.
+            site (str): Location of data collection. Default empty
+                string.
+
+        Returns:
+            tuple[plt.Figure, plt.Axes]: Regression plot of explanatory
+            and response data, with fitted regression line and
+            regression score.
+        """
+
+        figure = plt.figure(figsize=(8, 8))
+        date = self.get_date_and_timezone(data=x_data)["date"]
+        scatter_frame = pd.merge(
+            x_data, y_data, left_index=True, right_index=True, sort=True
+        )
+
+        scatter_frame = scatter_frame.dropna(axis=0)  # drop mismatched index
+        x_fit_data = scatter_frame.iloc[:, 0].values.reshape(-1, 1)
+        y_fit_data = scatter_frame.iloc[:, 1].values.reshape(-1, 1)
+        plt.scatter(x_fit_data, y_fit_data, marker=".", color="gray")
+
+        if regression_line is not None:
+            plt.plot(
+                x_fit_data, regression_line, color="black", label="Line of Best Fit"
+            )
+
+        axes = plt.gca()
+        if score is not None:
+            plt.text(
+                0.05,
+                0.9,
+                f"R$^{2}$= {score:.5f}",
+                horizontalalignment="left",
+                verticalalignment="bottom",
+                transform=axes.transAxes,
+            )
+        variable_name = self.label_selector(name)
+        sources_string = f"{sources[0]} and {sources[1]}"
+        title_string = f"{variable_name[0]} Regression Between\n{sources_string}"
+        site_label = self.get_site_name(site_name=site, dataframe=x_data)
+        self.title_plot(title=title_string, timestamp=date, location=site_label)
+        x_label = self.merge_label_with_unit(label=variable_name)
+        y_label = self.merge_label_with_unit(label=variable_name)
+        plt.xlabel(f"{x_label} ({sources[0]})")
+        plt.ylabel(f"{y_label} ({sources[1]})")
+
+        return figure, axes
+
     def plot_vertical_profile(
         self, vertical_data, time_idx, name, site="", y_lim=None, **kwargs
     ):
         """Plots vertical profile of variable.
 
         Args:
-            vertical_data (dict[pd.DataFrame]): Contains time series of
-                vertical profiles.
+            vertical_data (dict[str, pd.DataFrame]): Contains time
+                series of vertical measurements.
             time_idx (pd.Timestamp): The local time for which to plot a
                 vertical profile.
             name (str): Name of dependent variable, must be key in
                 <vertical_data>.
-            site (str): Location of data collection. Default empty string.
+            site (str): Location of data collection. Default empty
+                string.
             y_lim (float): Y-axis limit. Default None.
 
         Keyword Args:
             hlines (dict): Name and y-axis value for which to plot a
                 horizontal line.
             vlines (dict): Name and x-axis value for which to plot a
                 vertical line.
@@ -714,16 +795,16 @@
 
         title = f"Vertical Profile of {variable_name[0]}"
         site_label = self.get_site_name(site_name=site, dataframe=vertical_data[name])
         if not site_label:
             location = ",\n"
         else:
             location = f"\nat {site_label}, "
-        time_idx = time_idx.strftime("%H:%M")
-        time_label = f"{time_data['date']} {time_idx} {time_data['tzone']}"
+        time_string = time_idx.strftime("%H:%M")
+        time_label = f"{time_data['date']} {time_string} {time_data['tzone']}"
         title_string = f"{title}{location}{time_label}"
         plt.title(title_string, fontweight="bold")
         axes = plt.gca()
         if kwargs:
             self.parse_formatting_kwargs(axis=axes, **kwargs)
 
         return figure, axes
@@ -745,50 +826,47 @@
                 vertical lines.
 
         Returns:
             tuple[plt.Figure, plt.Axes]: Figure and axis of vertical
             profiles.
         """
 
-        key_number = len(keys)
+        key_length = len(keys)
         figure, axes = plt.subplots(
-            nrows=1, ncols=key_number, sharey=False, figsize=(4 * key_number, 8)
+            nrows=1, ncols=key_length, sharey=False, figsize=(4 * key_length, 8)
         )
         subplot_labels = []
-        for i in range(key_number):
+        for i in range(key_length):
             vertical_profile = dataset[keys[i]].loc[[time_index]]
-            time_data = self.get_date_and_timezone(
-                data=dataset[keys[i]].loc[[time_index]]
-            )
             axes[i].plot(
                 vertical_profile.values[0],
                 vertical_profile.columns,
                 color="black",
                 label=keys[i],
             )
             label = self.label_selector(dependent=keys[i])
             subplot_labels.append(label[0])
             x_label = self.merge_label_with_unit(label=label)
             axes[i].set_xlabel(x_label)
             axes[i].set_ylim(bottom=0)
 
             if kwargs:
                 self.parse_formatting_kwargs(axis=axes[i], **kwargs)
-
         axes[0].set_ylabel("Height [m]")
 
         title_name = self.merge_multiple_labels(labels=subplot_labels)
         title = f"Vertical Profiles of {title_name}"
         site_label = self.get_site_name(site_name=site, dataframe=dataset[keys[0]])
         if not site_label:
             location = ",\n"
         else:
             location = f"\nat {site_label}, "
-        time_index = time_index.strftime("%H:%M")
-        time_label = f"{time_data['date']} {time_index} {time_data['tzone']}"
+        time_data = self.get_date_and_timezone(data=dataset[keys[-1]].loc[[time_index]])
+        time_string = time_index.strftime("%H:%M")
+        time_label = f"{time_data['date']} {time_string} {time_data['tzone']}"
         title_string = f"{title}{location}{time_label}"
         figure.suptitle(title_string, fontweight="bold")
 
         return figure, axes
 
     def plot_merged_profiles(self, dataset, time_index, site="", y_lim=None, **kwargs):
         """Plots vertical profiles on the same axis.
@@ -811,23 +889,20 @@
 
         Returns:
             tuple[plt.Figure, plt.Axes]: Figure and axis of vertical
             profiles.
         """
 
         keys = list(dataset)
-        key_number = len(keys)
+        key_length = len(keys)
         figure = plt.figure(figsize=(8, 8))
         subplot_labels = []
         xlims = []
-        for i in range(key_number):
+        for i in range(key_length):
             vertical_profile = dataset[keys[i]].loc[[time_index]]
-            time_data = self.get_date_and_timezone(
-                data=dataset[keys[i]].loc[[time_index]]
-            )
             line_label = self.label_selector(dependent=keys[i])
             plt.plot(
                 vertical_profile.values[0],
                 vertical_profile.columns,
                 label=line_label[0],
             )
             subplot_labels.append(line_label[0])
@@ -835,14 +910,15 @@
             if y_lim:
                 heights = vertical_profile.columns[vertical_profile.columns <= y_lim]
                 xlim_max = math.ceil(max(vertical_profile[heights].values[0]))
                 xlims.append(xlim_max)
                 if xlim_max > 1:
                     xlim_min = math.floor(min(vertical_profile[heights].values[0]))
                     xlims.append(xlim_min)
+        line_label = self.label_selector(dependent=keys[-1])
         x_label = self.merge_label_with_unit(label=line_label)
         plt.xlabel(x_label)
         plt.ylabel("Height [m]")
         if not y_lim:
             plt.ylim(bottom=0)
         else:
             plt.ylim(0, y_lim)
@@ -852,16 +928,17 @@
         plt.legend()
 
         site_label = self.get_site_name(site_name=site, dataframe=dataset[keys[0]])
         if not site_label:
             location = ",\n"
         else:
             location = f"\nat {site_label}, "
-        time_index = time_index.strftime("%H:%M")
-        time_label = f"{time_data['date']} {time_index} {time_data['tzone']}"
+        time_data = self.get_date_and_timezone(data=dataset[keys[-1]].loc[[time_index]])
+        time_string = time_index.strftime("%H:%M")
+        time_label = f"{time_data['date']} {time_string} {time_data['tzone']}"
         title_name = self.merge_multiple_labels(labels=subplot_labels)
         title = f"Vertical Profiles of {title_name}"
         title_string = f"{title}{location}{time_label}"
         plt.title(title_string, fontweight="bold")
 
         axes = plt.gca()
         if kwargs:
```

### Comparing `scintillometry-1.0.4/src/scintillometry/wrangler/data_parser.py` & `scintillometry-1.0.5/src/scintillometry/wrangler/data_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         """Parses timestamp with mixed ISO-8601 duration and date.
 
         Uses integer properties of bool to act as index for partition.
 
         Args:
             x (str): Timestamp containing ISO-8601 duration and date,
                 i.e. "<ISO-8601 duration>/<ISO-8601 date>".
-            date (bool): If True, returns date. Otherwise returns
+            date (bool): If True, returns date. Otherwise, returns
                 duration. Default True.
 
         Returns:
             str: ISO-8601 string representing either a duration or a
             date.
         """
 
@@ -159,18 +159,17 @@
     def parse_mnd_lines(self, line_list):
         """Parses data and variable names from a list of .mnd lines.
 
         Args:
             line_list (list): Lines read from .mnd file in FORMAT-1.
 
         Returns:
-            dict[list, list, str, list]: Contains a list of lines of
-            parsed BLS data, an ordered list of variable names, the file
-            timestamp, and any additional header parameters in the file
-            header.
+            dict: Contains a list of lines of parsed BLS data, an
+            ordered list of variable names, the file timestamp, and any
+            additional header parameters in the file header.
 
         Raises:
             Warning: The input file does not follow FORMAT-1.
         """
 
         if line_list[0][:8] != "FORMAT-1":
             raise Warning("The input file does not follow FORMAT-1.")
@@ -247,15 +246,16 @@
 
         return data
 
     def parse_scintillometer(self, file_path, timezone="CET", calibration=None):
         """Parses .mnd files into dataframes.
 
         Args:
-            filename (str): Path to a raw .mnd data file using FORMAT-1.
+            file_path (str): Path to a raw .mnd data file using
+                FORMAT-1.
             timezone (str): Local timezone during the scintillometer's
                 operation. Default "CET".
             calibration (list): Contains the incorrect and correct path
                 lengths, [m]. Format as [incorrect, correct].
                 Default None.
 
         Returns:
@@ -676,19 +676,15 @@
 
         Raises:
             NotImplementedError: <source> measurements are not
                 supported. Use "innflux".
         """
 
         if source.lower() == "innflux":
-            eddy_data = self.parse_innflux(
-                file_name=file_path,
-                timezone=tzone,
-                headers=None,
-            )
+            eddy_data = self.parse_innflux(file_name=file_path, timezone=tzone)
         else:
             error_msg = (
                 f"{source.title()} measurements are not supported. Use 'innflux'."
             )
             raise NotImplementedError(error_msg)
 
         return eddy_data
@@ -802,16 +798,16 @@
                 measurement period. Default "CET".
             scan_heights (list[int]): Heights of HATPRO measurement
                 levels, |z_scan| [m]. Default None.
             elevation (float): Station elevation, |z_stn| [m].
                 Default 612.0.
 
         Returns:
-            dict[pd.DataFrame, pd.DataFrame]: Vertical measurements from
-            HATPRO for temperature |T| [K], and absolute humidity
+            dict[str, pd.DataFrame]: Vertical measurements from HATPRO
+            for temperature |T| [K], and absolute humidity
             |rho_v| [|gm^-3|].
         """
 
         humidity_path = f"{file_prefix}humidity.csv"
         temperature_path = f"{file_prefix}temp.csv"
 
         scan_levels = self.construct_hatpro_levels(levels=scan_heights)
@@ -824,17 +820,15 @@
         temperature_data = self.load_hatpro(
             file_name=temperature_path,
             levels=scan_levels,
             tzone=timezone,
             station_elevation=elevation,
         )
 
-        data = {}
-        data["humidity"] = humidity_data
-        data["temperature"] = temperature_data
+        data = {"humidity": humidity_data, "temperature": temperature_data}
 
         return data
 
     def parse_vertical(
         self,
         file_path,
         source="hatpro",
```

### Comparing `scintillometry-1.0.4/tests/conftest.py` & `scintillometry-1.0.5/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -223,15 +223,15 @@
                 test_frame = dataframe.tz_localize(arg_timezone)
             else:
                 test_frame = dataframe.tz_localize("UTC")
         assert ptypes.is_datetime64_any_dtype(test_frame.index)
         self.check_timezone(dataframe=test_frame, tzone=arg_timezone)
 
     def index_not_equal(self, index_01: pd.Index, index_02: pd.Index):
-        """Check that two indices are not equal."""
+        """Check if two indices are not equal."""
 
         with pytest.raises(AssertionError, match="Index are different"):
             assert pd.testing.assert_index_equal(
                 left=index_01, right=index_02, check_names=False
             )
 
     @pytest.mark.dependency(name="TestBoilerplate::test_assert_index_not_equal")
@@ -334,14 +334,29 @@
     """Stops figure being saved to disk."""
 
     patcher = patch.object(scintillometry.visuals.plotting.FigurePlotter, "save_figure")
     mock_exists = patcher.start()
     mock_exists.return_value = None
 
 
+# Mock random data
+@pytest.fixture(name="conftest_generate_series", scope="function", autouse=False)
+def fixture_conftest_generate_series():
+    """Generates Series with random data and DatetimeIndex"""
+
+    rng = np.random.default_rng()
+    test_timestamp = pd.Timestamp("03 June 2020 05:20", tz="CET")
+    test_index = pd.date_range(start=test_timestamp, periods=100, freq="T")
+    assert ptypes.is_datetime64_any_dtype(test_index)
+    test_data = rng.random(size=len(test_index))
+    assert isinstance(test_data, np.ndarray)
+
+    yield test_data, test_index
+
+
 # Mock scintillometer data
 @pytest.fixture(name="conftest_mnd_lines", scope="function", autouse=False)
 def fixture_conftest_mock_mnd_lines():
     """Constructs mock list output from reading .mnd string object."""
 
     file_header = ["FORMAT-1.1", "2020-06-03T03:23:00Z", "BLS450", "2 5\n"]
     ascii_header = ["Station Code:     Test", "Software:         SRun 1.49"]
```

### Comparing `scintillometry-1.0.4/tests/test_backend_constants.py` & `scintillometry-1.0.5/tests/test_backend_constants.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.4/tests/test_backend_constructions.py` & `scintillometry-1.0.5/tests/test_backend_constructions.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.4/tests/test_backend_derivations.py` & `scintillometry-1.0.5/tests/test_backend_derivations.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.4/tests/test_backend_iterations.py` & `scintillometry-1.0.5/tests/test_backend_iterations.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,27 +132,27 @@
         assert all(isinstance(coeffs, tuple) for coeffs in compare_coeffs)
         for coeffs in compare_coeffs:
             assert all(isinstance(coeff, float) for coeff in coeffs)
         assert compare_coeffs == self.test_coeffs
 
     @pytest.mark.dependency(name="TestBackendIterationMost::test_similarity_function")
     @pytest.mark.parametrize("arg_obukhov", [(-100, False), (0, True), (100, True)])
-    def test_similarity_function(self, arg_obukhov):
+    def test_similarity_function(self, arg_obukhov: tuple):
         """Compute similarity function."""
 
         test_f_ct2 = self.test_class.similarity_function(
             obukhov=arg_obukhov[0], z=10, coeffs=self.test_coeffs, stable=arg_obukhov[1]
         )
 
         assert isinstance(test_f_ct2, float)
         assert test_f_ct2 > 0
 
     @pytest.mark.dependency(name="TestBackendIterationMost::test_calc_theta_star")
     @pytest.mark.parametrize("arg_params", [(1.9e-04, 5.6, True), (2e-03, 3.6, False)])
-    def test_calc_theta_star(self, arg_params):
+    def test_calc_theta_star(self, arg_params: tuple):
         """Calculate temperature scale."""
 
         test_theta = self.test_class.calc_theta_star(
             ct2=arg_params[0], f_ct2=arg_params[1], z=10, stable=arg_params[2]
         )
 
         assert isinstance(test_theta, mpmath.mpf)
@@ -178,15 +178,15 @@
 
     @pytest.mark.dependency(name="TestBackendIterationMost::test_calc_obukhov_length")
     @pytest.mark.parametrize("arg_theta", [0.05, -0.05])
     def test_calc_obukhov_length(self, arg_theta):
         """Calculate Obukhov length."""
 
         compare_lob = self.test_class.calc_obukhov_length(
-            temp=295, u_star=0.2, theta_star=mpmath.mpmathify(arg_theta)
+            temp=np.float64(295.0), u_star=0.2, theta_star=mpmath.mpmathify(arg_theta)
         )
         assert isinstance(compare_lob, mpmath.mpf)
         assert (compare_lob < 0) == (arg_theta < 0)  # obukhov and theta have same sign
 
     @pytest.mark.dependency(name="TestBackendIterationMost::test_check_signs")
     @pytest.mark.filterwarnings("error")
     @pytest.mark.parametrize("arg_shf", [-150, 0, 150])
@@ -220,15 +220,15 @@
             "TestBackendIterationMost::test_calc_theta_star",
             "TestBackendIterationMost::test_calc_obukhov_length",
             "TestBackendIterationMost::test_check_signs",
         ],
         scope="class",
     )
     @pytest.mark.parametrize("arg_stable", [(200, True), (-100, False)])
-    def test_most_iteration(self, conftest_mock_merged_dataframe, arg_stable):
+    def test_most_iteration(self, conftest_mock_merged_dataframe, arg_stable: tuple):
         """Iterate single row of dataframe using MOST."""
 
         test_data = conftest_mock_merged_dataframe.iloc[0].copy(deep=True)
         test_data["obukhov"] = arg_stable[0]  # initial Obukhov Length
 
         compare_most = self.test_class.most_iteration(
             dataframe=test_data,
@@ -306,13 +306,13 @@
             "shf",
             "obukhov",
         ]
         assert isinstance(compare_most, pd.DataFrame)
         for key in compare_keys:
             assert not (compare_most[key].isnull()).any()
             assert key in compare_most.keys()
-            assert all(isinstance(x, (mpmath.mpf)) for x in compare_most[key])
+            assert all(isinstance(x, mpmath.mpf) for x in compare_most[key])
 
         # signs match stability
         assert (compare_most["obukhov"] > 0).all() == arg_stable[1]
         assert (compare_most["shf"] < 0).all() == arg_stable[1]
         assert (compare_most["obukhov"] < 0).all() == (compare_most["shf"] > 0).all()
```

### Comparing `scintillometry-1.0.4/tests/test_backend_transects.py` & `scintillometry-1.0.5/tests/test_backend_transects.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,12 +200,12 @@
             f"Effective path height:\t{test_eff:>0.2f} m.\n",
             f"Mean path height:\t{test_mean:>0.2f} m.\n",
         )
         print("".join(test_print))
         test_capture = capsys.readouterr()
 
         self.test_transect_parameters.print_path_heights(
-            z_eff=34, z_mean=31.245, stability=arg_stability
+            z_eff=np.float64(34), z_mean=np.float64(31.245), stability=arg_stability
         )
         compare_capture = capsys.readouterr()
 
         assert compare_capture == test_capture
```

### Comparing `scintillometry-1.0.4/tests/test_metrics_calculations.py` & `scintillometry-1.0.5/tests/test_metrics_calculations.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 import kneed
 import matplotlib.pyplot as plt
 import mpmath
 import numpy as np
 import pandas as pd
 import pandas.api.types as ptypes
 import pytest
+import sklearn
 
 import scintillometry.backend.constants
 import scintillometry.backend.constructions
 import scintillometry.backend.derivations
 import scintillometry.backend.iterations
 import scintillometry.metrics.calculations
 import scintillometry.visuals.plotting
@@ -102,15 +103,15 @@
             assert len(values) == 2
             assert all(isinstance(z, float) for z in values)
         for key in ["stable", "unstable"]:
             assert compare_metrics[key][0] < compare_metrics[key][1]
         assert compare_metrics["None"][0] > compare_metrics["None"][1]
 
         compare_print = capsys.readouterr()
-        if not arg_regime:
+        if arg_regime is None:
             assert "Selected no height dependency:" in compare_print.out
         else:
             assert str(arg_regime) in compare_print.out
         assert (
             str(f"Effective path height:\t{compare_metrics[str(arg_regime)][0]:>0.2f}")
             in compare_print.out
         )
@@ -167,15 +168,15 @@
         scope="session",
     )
     @pytest.mark.parametrize("arg_kwargs", [(880, 20), None])
     def test_construct_flux_dataframe(self, conftest_mock_merged_dataframe, arg_kwargs):
         """Compute sensible heat flux for free convection."""
 
         test_frame = conftest_mock_merged_dataframe[["CT2", "H_convection"]]
-        if arg_kwargs:
+        if isinstance(arg_kwargs, tuple):
             test_kwargs = {
                 "beam_wavelength": arg_kwargs[0],
                 "beam_error": arg_kwargs[1],
             }
         else:
             test_kwargs = {}
 
@@ -266,27 +267,27 @@
             conftest_boilerplate.index_not_equal(
                 compare_dataset["vertical"][key].index, test_dataset["weather"].index
             )
 
     @pytest.mark.dependency(name="TestMetricsFlux::test_match_time_at_threshold")
     @pytest.mark.parametrize("arg_lessthan", [True, False])
     @pytest.mark.parametrize("arg_empty", [True, False])
-    @pytest.mark.parametrize("arg_timestamp", [True, None])
+    @pytest.mark.parametrize("arg_timestamp", [True, False])
     def test_match_time_at_threshold(
         self, conftest_mock_weather_dataframe_tz, arg_lessthan, arg_empty, arg_timestamp
     ):
         """Derive and append vertical measurements to dataset."""
 
         test_weather = conftest_mock_weather_dataframe_tz.copy(deep=True)
         if arg_empty:
             test_weather["global_irradiance"] = 20
-        if not arg_timestamp:
-            test_timestamp = None
-        else:
+        if arg_timestamp:
             test_timestamp = self.test_timestamp
+        else:
+            test_timestamp = None
 
         compare_time = self.test_metrics.match_time_at_threshold(
             series=test_weather["global_irradiance"],
             threshold=20,
             lessthan=arg_lessthan,
             min_time=test_timestamp,
         )
@@ -296,14 +297,53 @@
             if arg_lessthan:
                 assert compare_time.strftime("%H:%M") == "05:10"
             else:
                 assert compare_time.strftime("%H:%M") == "05:19"
         else:
             assert compare_time is None
 
+    @pytest.mark.dependency(name="TestMetricsFlux::test_get_regression")
+    @pytest.mark.parametrize("arg_intercept", [True, False])
+    @pytest.mark.parametrize("arg_mismatch_index", [True, False])
+    def test_get_regression(
+        self, conftest_boilerplate, arg_intercept, arg_mismatch_index
+    ):
+        """Perform regression on labelled data."""
+
+        rng = np.random.default_rng()
+        test_index = pd.date_range(start=self.test_timestamp, periods=100, freq="T")
+        test_data = rng.random(size=len(test_index))
+
+        test_x = pd.Series(name="obukhov", data=test_data, index=test_index)
+        test_y = pd.Series(name="other_obukhov", data=test_data + 0.5, index=test_index)
+        if arg_mismatch_index:
+            test_y = test_y[:-5]
+            conftest_boilerplate.index_not_equal(test_x.index, test_y.index)
+            assert test_y.shape == (95,)
+        assert isinstance(test_x, pd.Series)
+        assert test_x.shape == (100,)
+        test_keys = ["fit", "score", "regression_line"]
+
+        compare_regression = self.test_metrics.get_regression(
+            x_data=test_x, y_data=test_y, intercept=arg_intercept
+        )
+        assert isinstance(compare_regression, dict)
+        assert all(key in compare_regression for key in test_keys)
+        assert isinstance(
+            compare_regression["fit"], sklearn.linear_model.LinearRegression
+        )
+        if arg_intercept:
+            assert compare_regression["fit"].fit_intercept
+        else:
+            assert not compare_regression["fit"].fit_intercept
+        assert isinstance(compare_regression["score"], float)
+        assert isinstance(compare_regression["regression_line"], np.ndarray)
+        assert not (np.isnan(compare_regression["regression_line"])).any()
+        assert len(test_y.index) == len(compare_regression["regression_line"])
+
     @pytest.mark.dependency(name="TestMetricsFlux::test_get_elbow_point")
     @pytest.mark.parametrize("arg_min_index", [None, 0, 50])
     @pytest.mark.parametrize("arg_max_index", [None, 180, 190])
     @pytest.mark.parametrize("arg_curve", [1, -1])
     def test_get_elbow_point(self, arg_min_index, arg_max_index, arg_curve):
         """Estimate elbow point of curve."""
 
@@ -329,15 +369,15 @@
             (test_curve.index >= min_index) & (test_curve.index <= max_index)
         ]
         test_knee = kneed.KneeLocator(
             test_curve[test_indices] * arg_curve,
             test_indices,
             S=1.5,
             curve="convex",
-            online="true",
+            online=True,
             direction=test_direction,
             interp_method="interp1d",
         )
         elbows = test_curve[test_knee.all_elbows_y][
             test_curve[test_knee.all_elbows_y] < test_curve[test_indices].mean()
         ]
         if not elbows.empty:
@@ -614,46 +654,49 @@
         assert isinstance(test_time, pd.Timestamp)
         test_vertical = test_dataset["vertical"]
         if arg_location:
             test_location = f"\nat {arg_location}, "
         else:
             test_location = ",\n"
         test_labels = ["Potential Temperature, [K]"]
-        if not arg_gradient:
-            test_vertical.pop("grad_potential_temperature", None)
-            assert "grad_potential_temperature" not in test_vertical
-            test_title = (
-                f"Vertical Profile of Potential Temperature{test_location}",
-                f"{self.test_date} 05:20 CET",
-            )
-        else:
+        if arg_gradient:
             assert "grad_potential_temperature" in test_vertical
             test_title = (
                 "Vertical Profiles of Potential Temperature ",
                 f"and Gradient of Potential Temperature{test_location}",
                 f"{self.test_date} 05:20 CET",
             )
             test_labels.append(r"Gradient of Potential Temperature, [K$\cdot$m$^{-1}$]")
+        else:
+            test_vertical.pop("grad_potential_temperature", None)
+            assert "grad_potential_temperature" not in test_vertical
+            test_title = (
+                f"Vertical Profile of Potential Temperature{test_location}",
+                f"{self.test_date} 05:20 CET",
+            )
 
-        compare_fig, compare_ax = self.test_metrics.plot_switch_time_stability(
+        compare_plots = self.test_metrics.plot_switch_time_stability(
             data=test_vertical, local_time=test_time, location=arg_location
         )
-        assert isinstance(compare_fig, plt.Figure)
-
-        if not arg_gradient:
-            assert isinstance(compare_ax, plt.Axes)
-            assert compare_ax.get_title() == "".join(test_title)
-            assert compare_ax.yaxis.get_label_text() == "Height [m]"
-        else:
-            assert isinstance(compare_ax, np.ndarray)
-            assert all(isinstance(ax, plt.Axes) for ax in compare_ax)
-            assert compare_fig.texts[0].get_text() == "".join(test_title)
-            assert compare_ax[0].yaxis.get_label_text() == "Height [m]"
-            for i in range(len(compare_ax)):
-                assert compare_ax[i].xaxis.get_label_text() == test_labels[i]
+        assert isinstance(compare_plots, list)
+        for compare_tuple in compare_plots:
+            assert isinstance(compare_tuple, tuple)
+            assert isinstance(compare_tuple[0], plt.Figure)
+            compare_ax = compare_tuple[1]
+            if arg_gradient:
+                assert isinstance(compare_ax, np.ndarray)
+                assert all(isinstance(ax, plt.Axes) for ax in compare_ax)
+                assert compare_tuple[0].texts[0].get_text() == "".join(test_title)
+                assert compare_ax[0].yaxis.get_label_text() == "Height [m]"
+                for i in range(len(compare_ax)):
+                    assert compare_ax[i].xaxis.get_label_text() == test_labels[i]
+            else:
+                assert isinstance(compare_ax, plt.Axes)
+                assert compare_ax.get_title() == "".join(test_title)
+                assert compare_ax.yaxis.get_label_text() == "Height [m]"
 
         plt.close("all")
 
     @pytest.mark.dependency(name="TestMetricsFlux::test_plot_lapse_rates")
     @pytest.mark.parametrize("arg_height", [None, 100])
     @pytest.mark.parametrize("arg_location", [None, "Test Location"])
     def test_plot_lapse_rates(
@@ -679,34 +722,36 @@
             assert key in test_dataset["vertical"]
         if arg_location:
             test_location = f"\nat {arg_location}, "
         else:
             test_location = ",\n"
         test_title = f"{test_location}{self.test_date} 05:10 CET"
 
-        fig_lapse, ax_lapse, fig_parcel, ax_parcel = self.test_metrics.plot_lapse_rates(
+        compare_plots = self.test_metrics.plot_lapse_rates(
             vertical_data=test_dataset["vertical"],
             dry_adiabat=self.test_metrics.constants.dalr,
             local_time=self.test_timestamp,
             location=arg_location,
             bl_height=arg_height,
         )
+        assert isinstance(compare_plots, list)
+        assert all(isinstance(compare_tuple, tuple) for compare_tuple in compare_plots)
 
         compare_params = {
             "lapse": {
                 "title": "Temperature Lapse Rates",
                 "x_label": r"Lapse Rate, [Km$^{-1}$]",
                 "y_label": "Height [m]",
-                "plot": (fig_lapse, ax_lapse),
+                "plot": (compare_plots[0]),
             },
             "parcel": {
                 "title": "Vertical Profiles of Parcel Temperature",
                 "x_label": "Temperature, [K]",
                 "y_label": "Height [m]",
-                "plot": (fig_parcel, ax_parcel),
+                "plot": (compare_plots[1]),
             },
         }
 
         for params in compare_params.values():
             conftest_boilerplate.check_plot(plot_params=params, title=test_title)
 
         plt.close("all")
@@ -757,16 +802,16 @@
         """Calculate and plot switch time."""
 
         _ = conftest_mock_save_figure
 
         test_dataset = {
             "weather": conftest_mock_weather_dataframe_tz.copy(deep=True),
             "timestamp": self.test_timestamp.replace(hour=5, minute=10),
+            "vertical": conftest_mock_hatpro_dataset.copy(),
         }
-        test_dataset["vertical"] = conftest_mock_hatpro_dataset.copy()
         test_dataset = self.test_metrics.append_vertical_variables(data=test_dataset)
 
         if not arg_potential:
             test_dataset["vertical"].pop("grad_potential_temperature")
             assert "grad_potential_temperature" not in test_dataset["vertical"]
         else:
             assert "grad_potential_temperature" in test_dataset["vertical"]
@@ -804,31 +849,34 @@
         arg_regime,
     ):
         """Plot time series of heat fluxes for free convection."""
 
         _ = conftest_mock_save_figure
 
         test_frame = conftest_mock_derived_dataframe
-        if arg_regime:
+        if arg_regime is not None:
             test_conditions = f"{arg_regime.capitalize()} Conditions"
         else:
             test_conditions = "No Height Dependency"
         test_title = (
             "Sensible Heat Fluxes from On-Board Software and",
             f"for Free Convection ({test_conditions}),\n{self.test_date}",
         )
 
-        compare_fig, compare_ax = self.test_metrics.plot_derived_metrics(
+        compare_plots = self.test_metrics.plot_derived_metrics(
             derived_data=test_frame,
             time_id=test_frame.index[0],
             regime=arg_regime,
             location="",
         )
+        assert isinstance(compare_plots, list)
+        assert all(isinstance(compare_tuple, tuple) for compare_tuple in compare_plots)
+
         compare_params = {
-            "plot": (compare_fig, compare_ax),
+            "plot": (compare_plots[0]),
             "x_label": "Time, CET",
             "y_label": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
             "title": " ".join(test_title),
         }
         conftest_boilerplate.check_plot(plot_params=compare_params)
 
         plt.close("all")
@@ -853,35 +901,51 @@
             assert "name" in test_frame.attrs
         if arg_location:
             test_location = f" at {arg_location}"
         else:
             test_location = ""
         test_title = f"{test_location},\n{self.test_date}"
 
-        plot_pairs = self.test_metrics.plot_iterated_metrics(
+        compare_plots = self.test_metrics.plot_iterated_metrics(
             iterated_data=test_frame,
             time_stamp=test_stamp,
-            site_location=arg_location,
+            location=arg_location,
         )
+        assert isinstance(compare_plots, list)
+        assert all(isinstance(compare_tuple, tuple) for compare_tuple in compare_plots)
 
-        compare_plots = {
+        compare_params = {
             "iteration": {
-                "plot": (plot_pairs[0], plot_pairs[1]),
+                "plot": (compare_plots[0]),
                 "title": "Sensible Heat Flux",
                 "x_label": "Time, CET",
-                "ylabel": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
+                "y_label": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
             },
             "comparison": {
-                "plot": (plot_pairs[2], plot_pairs[3]),
+                "plot": (compare_plots[1]),
                 "title": "Sensible Heat Flux from Free Convection and Iteration",
                 "x_label": "Time, CET",
-                "ylabel": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
+                "y_label": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
             },
         }
-        for params in compare_plots.values():
+        for params in compare_params.values():
+            conftest_boilerplate.check_plot(plot_params=params, title=test_title)
+
+        plt.close("all")
+
+        # site_location is pending deprecation
+        with pytest.warns(PendingDeprecationWarning):
+            compare_plots = self.test_metrics.plot_iterated_metrics(
+                iterated_data=test_frame,
+                time_stamp=test_stamp,
+                site_location=arg_location,  # pylint:disable=unexpected-keyword-arg
+            )
+        assert isinstance(compare_plots, list)
+        assert all(isinstance(compare_tuple, tuple) for compare_tuple in compare_plots)
+        for params in compare_params.values():
             conftest_boilerplate.check_plot(plot_params=params, title=test_title)
 
         plt.close("all")
 
     @pytest.mark.dependency(
         name="TestMetricsFlux::test_iterate_fluxes",
         depends=["TestMetricsFlux::test_append_vertical_variables"],
@@ -920,15 +984,15 @@
             "shf",
             "obukhov",
         ]
         assert isinstance(compare_metrics, pd.DataFrame)
         for key in compare_keys:
             assert not (compare_metrics[key].isnull()).any()
             assert key in compare_metrics.keys()
-            assert all(isinstance(x, (mpmath.mpf)) for x in compare_metrics[key])
+            assert all(isinstance(x, mpmath.mpf) for x in compare_metrics[key])
         plt.close("all")
 
 
 class TestMetricsWorkflow:
     """Test class for metrics workflow.
 
     Attributes:
@@ -1068,47 +1132,68 @@
         depends=["TestMetricsWorkflow::test_metrics_workflow_init"],
         scope="class",
     )
     @pytest.mark.parametrize("arg_location", [None, "", "Test Location"])
     def test_compare_innflux(
         self,
         conftest_mock_save_figure,
-        conftest_mock_innflux_dataframe_tz,
-        conftest_mock_iterated_dataframe,
         conftest_boilerplate,
+        conftest_generate_series,
         arg_location,
     ):
-        """Compares input data to InnFLUX data."""
+        """Compares input data to innFLUX data."""
 
         _ = conftest_mock_save_figure
 
+        test_data, test_index = conftest_generate_series
+        test_obukhov = pd.Series(data=test_data, index=test_index)
+        test_shf = pd.Series(data=test_data, index=test_index)
+        test_base_dataframe = pd.DataFrame(
+            data={"obukhov": test_obukhov, "shf": test_shf},
+        )
+        test_ext_dataframe = test_base_dataframe.add(0.5)
+
         if arg_location:
             test_location = f" at {arg_location}"
         else:
             test_location = ""
         test_title = f"{test_location},\n{self.test_date}"
+        test_regression_string = "Regression Between\nMOST Iteration and innFLUX"
 
-        fig_obukhov, ax_obukhov, fig_shf, ax_shf = self.test_workflow.compare_innflux(
-            innflux_data=conftest_mock_innflux_dataframe_tz,
-            own_data=conftest_mock_iterated_dataframe,
+        compare_plots = self.test_workflow.compare_innflux(
+            own_data=test_base_dataframe,
+            innflux_data=test_ext_dataframe,
             location=arg_location,
         )
-
+        assert isinstance(compare_plots, list)
+        assert all(isinstance(compare_tuple, tuple) for compare_tuple in compare_plots)
         compare_params = {
             "obukhov": {
                 "title": "Obukhov Length from Scintillometer and innFLUX",
                 "y_label": "Obukhov Length, [m]",
                 "x_label": "Time, CET",
-                "plot": (fig_obukhov, ax_obukhov),
+                "plot": (compare_plots[0]),
             },
             "shf": {
                 "title": "Sensible Heat Flux from Scintillometer and innFLUX",
-                "ylabel": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
+                "y_label": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
                 "x_label": "Time, CET",
-                "plot": (fig_shf, ax_shf),
+                "plot": (compare_plots[1]),
+            },
+            "obukhov_regression": {
+                "title": f"Obukhov Length {test_regression_string}",
+                "y_label": "Obukhov Length, [m] (innFLUX)",
+                "x_label": "Obukhov Length, [m] (MOST Iteration)",
+                "plot": (compare_plots[2]),
+            },
+            "shf_regression": {
+                "title": f"Sensible Heat Flux {test_regression_string}",
+                "y_label": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$] (innFLUX)",
+                "x_label": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$] (MOST Iteration)",
+                "plot": (compare_plots[3]),
             },
         }
 
         for params in compare_params.values():
             conftest_boilerplate.check_plot(plot_params=params, title=test_title)
 
         plt.close("all")
@@ -1139,45 +1224,50 @@
         name="TestMetricsWorkflow::test_compare_eddy",
         depends=[
             "TestMetricsWorkflow::test_compare_innflux",
             "TestMetricsWorkflow::test_compare_eddy_error",
         ],
     )
     def test_compare_eddy(
-        self,
-        conftest_mock_save_figure,
-        conftest_mock_innflux_dataframe_tz,
-        conftest_mock_iterated_dataframe,
-        conftest_boilerplate,
+        self, conftest_mock_save_figure, conftest_generate_series, conftest_boilerplate
     ):
         """Compares input data to external eddy covariance data."""
 
         _ = conftest_mock_save_figure
 
+        test_data, test_index = conftest_generate_series
+        test_obukhov = pd.Series(data=test_data, index=test_index)
+        test_shf = pd.Series(data=test_data, index=test_index)
+        test_base_dataframe = pd.DataFrame(
+            data={"obukhov": test_obukhov, "shf": test_shf},
+        )
+        test_ext_dataframe = test_base_dataframe.add(0.5)
         test_location = "Test Location"
         test_title = f" at {test_location},\n{self.test_date}"
 
-        fig_obukhov, ax_obukhov, fig_shf, ax_shf = self.test_workflow.compare_eddy(
-            own_data=conftest_mock_iterated_dataframe,
-            ext_data=conftest_mock_innflux_dataframe_tz,
+        compare_plots = self.test_workflow.compare_eddy(
+            own_data=test_base_dataframe,
+            ext_data=test_ext_dataframe,
             source="innflux",
             location="Test Location",
         )
+        assert isinstance(compare_plots, list)
+        assert all(isinstance(compare_tuple, tuple) for compare_tuple in compare_plots)
 
         compare_params = {
             "obukhov": {
                 "title": "Obukhov Length from Scintillometer and innFLUX",
                 "y_label": "Obukhov Length, [m]",
                 "x_label": "Time, CET",
-                "plot": (fig_obukhov, ax_obukhov),
+                "plot": (compare_plots[0]),
             },
             "shf": {
                 "title": "Sensible Heat Flux from Scintillometer and innFLUX",
-                "ylabel": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
+                "y_label": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
                 "x_label": "Time, CET",
-                "plot": (fig_shf, ax_shf),
+                "plot": (compare_plots[1]),
             },
         }
         for params in compare_params.values():
             conftest_boilerplate.check_plot(plot_params=params, title=test_title)
 
         plt.close("all")
```

### Comparing `scintillometry-1.0.4/tests/test_visuals_plotting.py` & `scintillometry-1.0.5/tests/test_visuals_plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,18 +60,19 @@
                         assert key.title() not in compare_labels
                     else:
                         assert key.title() in compare_labels
 
     @pytest.mark.dependency(name="TestVisualsBoilerplate::test_assert_constant_lines")
     @pytest.mark.parametrize("arg_vlines", [{"v_a": 1}, {"v_a": 1, "v_b": 2.1}, None])
     @pytest.mark.parametrize("arg_hlines", [{"h_a": 1}, {"h_a": 1, "h_b": 2.1}, None])
-    def test_assert_constant_lines(self, arg_hlines, arg_vlines):
-        rng = np.random.default_rng()
-        test_index = np.arange(0, 200, 10)
-        test_data = rng.random(size=len(test_index))
+    def test_assert_constant_lines(
+        self, conftest_generate_series, arg_hlines, arg_vlines
+    ):
+        """Validate test for constant lines existing on axis."""
+        test_data, test_index = conftest_generate_series
         test_series = pd.Series(data=test_data, index=test_index)
 
         plt.figure(figsize=(10, 10))
         plt.plot(test_index, test_series)
         if arg_vlines:
             for vline in arg_vlines:
                 plt.axvline(arg_vlines[vline], label=vline.title())
@@ -124,21 +125,19 @@
         for param, font_size in test_params.items():
             assert plt.rcParams[param] == font_size
         plt.rcdefaults()
         plt.close("all")
 
     @pytest.mark.dependency(name="TestVisualsFormatting::test_parse_formatting_kwargs")
     @pytest.mark.parametrize("arg_fig", [True, False])
-    def test_parse_formatting_kwargs(self, arg_fig):
+    def test_parse_formatting_kwargs(self, arg_fig, conftest_generate_series):
         """Parse kwargs when formatting."""
 
         if arg_fig:
-            rng = np.random.default_rng()
-            test_index = np.arange(0, 200, 10)
-            test_data = rng.random(size=len(test_index))
+            test_data, test_index = conftest_generate_series
             test_series = pd.Series(data=test_data, index=test_index)
             plt.figure(figsize=(10, 10))
             plt.plot(test_index, test_series)
 
         test_kwargs = {
             "hlines": {"h_a": 1},
             "vlines": {"v_a": 1},
@@ -329,20 +328,20 @@
         depends=[
             "TestVisualsBoilerplate::test_assert_constant_lines",
             "TestVisualsFormatting::test_label_selector",
         ],
     )
     @pytest.mark.parametrize("arg_vlines", [{"va": None}, {"va": 1, "vb": 2.1}, None])
     @pytest.mark.parametrize("arg_hlines", [{"ha": None}, {"ha": 1, "hb": 2.1}, None])
-    def test_plot_constant_lines(self, arg_hlines, arg_vlines):
+    def test_plot_constant_lines(
+        self, conftest_generate_series, arg_hlines, arg_vlines
+    ):
         """Plot horizontal and vertical lines."""
 
-        rng = np.random.default_rng()
-        test_index = np.arange(0, 200, 10)
-        test_data = rng.random(size=len(test_index))
+        test_data, test_index = conftest_generate_series
         test_series = pd.Series(data=test_data, index=test_index)
 
         plt.figure(figsize=(10, 10))
         plt.plot(test_index, test_series)
         plt.legend()
         test_ax = plt.gca()
         self.test_format.plot_constant_lines(
@@ -364,15 +363,15 @@
     """
 
     test_plotting = scintillometry.visuals.plotting.FigurePlotter()
     test_location = "Test Location"
     test_date = "03 June 2020"
     test_timestamp = pd.Timestamp(f"{test_date} 05:20", tz="CET")
 
-    def test_visualsplotting_attributes(self):
+    def test_visuals_plotting_attributes(self):
         assert isinstance(self.test_timestamp, pd.Timestamp)
         assert self.test_timestamp.strftime("%Y-%m-%d %H:%M") == "2020-06-03 05:20"
         assert self.test_timestamp.tz.zone == "CET"
 
     @pytest.mark.dependency(
         name="TestVisualsPlotting::test_setup_plot_data",
         depends=["TestVisualsFormatting::test_get_date_and_timezone"],
@@ -592,32 +591,35 @@
         if arg_location:
             test_location = f" at {arg_location}"
         else:
             test_location = ""
         test_title = f"{test_location},\n{self.test_date}"
         timestamp = test_data.index[0]
 
-        plots = self.test_plotting.plot_iterated_fluxes(
-            iteration_data=test_data,
-            time_id=timestamp,
-            location=arg_location,
-        )
+        with pytest.deprecated_call():
+            compare_plots = self.test_plotting.plot_iterated_fluxes(
+                iteration_data=test_data,
+                time_id=timestamp,
+                location=arg_location,
+            )
+        assert isinstance(compare_plots, list)
+        assert all(isinstance(compare_tuple, tuple) for compare_tuple in compare_plots)
 
         compare_plots = {
             "shf": {
                 "title": "Sensible Heat Flux",
-                "ylabel": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
-                "xlabel": "Time, CET",
-                "plot": (plots[0], plots[1]),
+                "y_label": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
+                "x_label": "Time, CET",
+                "plot": (compare_plots[0]),
             },
             "comparison": {
                 "title": "Sensible Heat Flux from Free Convection and Iteration",
-                "ylabel": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
-                "xlabel": "Time, CET",
-                "plot": (plots[2], plots[3]),
+                "y_label": r"Sensible Heat Flux, [W$\cdot$m$^{-2}$]",
+                "x_label": "Time, CET",
+                "plot": (compare_plots[1]),
             },
         }
 
         for params in compare_plots.values():
             conftest_boilerplate.check_plot(plot_params=params, title=test_title)
 
         plt.close("all")
@@ -679,14 +681,80 @@
             },
         }
         for params in compare_plots.values():
             conftest_boilerplate.check_plot(plot_params=params, title=test_title)
 
         plt.close("all")
 
+    @pytest.mark.dependency(name="TestVisualsPlotting::test_plot_scatter")
+    @pytest.mark.parametrize("arg_site", ["", "Test Location", None])
+    @pytest.mark.parametrize("arg_score", [None, 0.561734521])
+    @pytest.mark.parametrize("arg_regression", [True, False])
+    def test_plot_scatter(
+        self,
+        conftest_boilerplate,
+        conftest_generate_series,
+        arg_score,
+        arg_site,
+        arg_regression,
+    ):
+        """Plot scatter between two datasets with regression line."""
+
+        test_name = "obukhov"
+        test_data, test_index = conftest_generate_series
+
+        test_x = pd.Series(name=test_name, data=test_data, index=test_index)
+        test_y = pd.Series(name=test_name, data=test_data + 0.5, index=test_index)
+        for series in [test_x, test_y]:
+            assert isinstance(series, pd.Series)
+            assert series.shape == (100,)
+            assert not (series.isnull()).any()
+        if arg_site:
+            test_site = f" at {arg_site},"
+        else:
+            test_site = ","
+        test_title = (
+            "Obukhov Length Regression Between",
+            f"Baseline and Comparison{test_site}",
+            f"{self.test_date}",
+        )
+        if not arg_regression:
+            test_line = None
+        else:
+            test_line = np.arange(0, 1000, 10)
+
+        compare_fig, compare_ax = self.test_plotting.plot_scatter(
+            x_data=test_x,
+            y_data=test_y,
+            name=test_name,
+            sources=["Baseline", "Comparison"],
+            site=arg_site,
+            score=arg_score,
+            regression_line=test_line,
+        )
+        compare_params = {
+            "plot": (compare_fig, compare_ax),
+            "x_label": "Obukhov Length, [m] (Baseline)",
+            "y_label": "Obukhov Length, [m] (Comparison)",
+            "title": "\n".join(test_title),
+        }
+        conftest_boilerplate.check_plot(plot_params=compare_params)
+
+        if arg_regression:
+            _, labels = compare_params["plot"][1].get_legend_handles_labels()
+            assert "Line of Best Fit" in labels
+
+        if arg_score is not None:
+            assert (
+                compare_params["plot"][1].texts[0].get_text()
+                == f"R$^{2}$= {arg_score:.5f}"
+            )
+
+        plt.close("all")
+
     @pytest.mark.dependency(
         name="TestVisualsPlotting::test_plot_vertical_profile",
         depends=["TestVisualsFormatting::test_plot_constant_lines"],
     )
     @pytest.mark.parametrize("arg_site", ["", "Test Location", None])
     @pytest.mark.parametrize("arg_name", ["temperature", "test_variable"])
     @pytest.mark.parametrize("arg_kwargs", [{}, {"hlines": {"test height": 10}}])
```

### Comparing `scintillometry-1.0.4/tests/test_wrangler_data_parser.py` & `scintillometry-1.0.5/tests/test_wrangler_data_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -887,15 +887,15 @@
             test_class.transform, scintillometry.wrangler.data_parser.WranglerTransform
         )
         assert test_class.check_file_exists
 
     @pytest.mark.dependency(
         name="TestWranglerVertical::test_construct_hatpro_levels_error"
     )
-    @pytest.mark.parametrize("arg_levels", [[(0, 1), (0)], [1.0, 30]])
+    @pytest.mark.parametrize("arg_levels", [[(0, 1), 0], [1.0, 30]])
     def test_construct_hatpro_levels_error(self, arg_levels):
         """Raise error for incorrectly formatted scanning levels."""
 
         error_message = "Input levels must be a list or tuple of integers."
         with pytest.raises(TypeError, match=error_message):
             self.test_wrangler_vertical.construct_hatpro_levels(levels=arg_levels)
 
@@ -906,15 +906,15 @@
     @pytest.mark.parametrize("arg_levels", [None, (0, 10, 20), [0, 10, 20]])
     def test_construct_hatpro_levels(self, arg_levels):
         """Construct HATPRO scanning levels."""
 
         compare_scan = self.test_wrangler_vertical.construct_hatpro_levels(
             levels=arg_levels
         )
-        assert isinstance(compare_scan, (list))
+        assert isinstance(compare_scan, list)
         assert all(isinstance(x, int) for x in compare_scan)
 
     @pytest.mark.dependency(
         name="TestWranglerVertical::test_load_hatpro",
         depends=[
             "TestWranglerTransform::test_pandas_attrs",
             "TestWranglerVertical::test_vertical_init",
```

### Comparing `scintillometry-1.0.4/tests/test_data/test_data_v7_results.mat` & `scintillometry-1.0.5/tests/test_data/test_data_v7_results.mat`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.4/LICENSE` & `scintillometry-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.4/README.md` & `scintillometry-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 See the License for the specific language governing permissions and
 limitations under the License. -->
 
 # Scintillometry
 
 [![Pytest and Flake8](https://github.com/gampnico/scintillometry/actions/workflows/python-app.yml/badge.svg?branch=main)](https://github.com/gampnico/scintillometry/actions/workflows/python-app.yml)
 
+Development branch: [![Pytest and Linting](https://github.com/gampnico/scintillometry/actions/workflows/python-app.yml/badge.svg?branch=develop)](https://github.com/gampnico/scintillometry/actions/workflows/python-app.yml)
+
 Analyse data & 2D flux footprints from Scintec's BLS scintillometers.
 
-This package started life as part of a field course. If you spot any missing citations or licenses please [open an issue](https://github.com/gampnico/scintillometry/issues).
+This project started life as part of a field course. If you spot any missing citations or licences please [open an issue](https://github.com/gampnico/scintillometry/issues).
 
 Comprehensive documentation is available [via ReadTheDocs](https://scintillometry.readthedocs.io/en/latest/).
 
 # Processing Scintillometry Data in Complex Terrain
 
 *Scintillometry* is configured for scintillometer experiments in Austria using public or local data (ZAMG, InnFLUX), but is easily modified to work with other data sources. Note that external data sources may have different licensing constraints.
```

### Comparing `scintillometry-1.0.4/pyproject.toml` & `scintillometry-1.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scintillometry"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Scintillometry Contributors", email="" },
 ]
 description = "Analyse data & 2D flux footprints from Scintec's BLS scintillometers."
 readme = "README.md"
 requires-python = ">=3.8"
-license = {file = "LICENSE"}
+license = "Apache-2.0"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 4 - Beta",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -26,14 +26,15 @@
 ]
 dependencies = [
   "pandas >= 2.0",
   "tqdm > 4.8",
   "scipy >= 1.10",
   "mpmath >= 1.2.1",
   "numpy",
+  "scikit-learn",
   "matplotlib",
   "kneed",
 ]
 
 [project.optional-dependencies]
 tests=[
   "pytest >= 7.0",
```

