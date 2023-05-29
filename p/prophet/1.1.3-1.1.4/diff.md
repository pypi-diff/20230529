# Comparing `tmp/prophet-1.1.3.tar.gz` & `tmp/prophet-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophet-1.1.3.tar", last modified: Wed May 17 14:46:58 2023, max compression
+gzip compressed data, was "prophet-1.1.4.tar", last modified: Mon May 29 15:13:00 2023, max compression
```

## Comparing `prophet-1.1.3.tar` & `prophet-1.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:58.588314 prophet-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-17 14:46:39.000000 prophet-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-17 14:46:39.000000 prophet-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-17 14:46:58.588314 prophet-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-17 14:46:39.000000 prophet-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:58.584313 prophet-1.1.3/prophet/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22557 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    76155 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/forecaster.py
--rw-r--r--   0 runner    (1001) docker     (123)    33623 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/hdays.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/make_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    36757 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:58.588314 prophet-1.1.3/prophet/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/data2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/serialized_model_v0.6.1.dev0.json
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/serialized_model_v0.7.1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/serialized_model_v1.0.1.json
--rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    37362 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/test_prophet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-17 14:46:39.000000 prophet-1.1.3/prophet/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:58.584313 prophet-1.1.3/prophet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 14:46:58.000000 prophet-1.1.3/prophet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-17 14:46:39.000000 prophet-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:46:58.588314 prophet-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-17 14:46:39.000000 prophet-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:46:58.588314 prophet-1.1.3/stan/
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-17 14:46:39.000000 prophet-1.1.3/stan/prophet.stan
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:00.479207 prophet-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-29 15:12:42.000000 prophet-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-29 15:12:42.000000 prophet-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-29 15:13:00.479207 prophet-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-29 15:12:42.000000 prophet-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:00.475207 prophet-1.1.4/prophet/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22557 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76155 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33732 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/hdays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/make_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36757 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:00.475207 prophet-1.1.4/prophet/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/data2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/serialized_model_v0.6.1.dev0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/serialized_model_v0.7.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/serialized_model_v1.0.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37362 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/test_prophet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-29 15:12:42.000000 prophet-1.1.4/prophet/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:00.475207 prophet-1.1.4/prophet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-29 15:13:00.000000 prophet-1.1.4/prophet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-29 15:13:00.000000 prophet-1.1.4/prophet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:13:00.000000 prophet-1.1.4/prophet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:13:00.000000 prophet-1.1.4/prophet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-29 15:13:00.000000 prophet-1.1.4/prophet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 15:13:00.000000 prophet-1.1.4/prophet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-29 15:12:42.000000 prophet-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:13:00.479207 prophet-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-29 15:12:42.000000 prophet-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:00.479207 prophet-1.1.4/stan/
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-29 15:12:42.000000 prophet-1.1.4/stan/prophet.stan
```

### Comparing `prophet-1.1.3/LICENSE` & `prophet-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/PKG-INFO` & `prophet-1.1.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophet
-Version: 1.1.3
+Version: 1.1.4
 Summary: Automatic Forecasting Procedure
 Author-email: "Sean J. Taylor" <sjtz@pm.me>, Ben Letham <bletham@fb.com>
 Maintainer-email: Cuong Duong <cuong.duong242@gmail.com>
 License: MIT
 Project-URL: Homepage, https://facebook.github.io/prophet/
 Project-URL: Documentation, https://facebook.github.io/prophet/
 Project-URL: Repository, https://github.com/facebook/prophet
```

### Comparing `prophet-1.1.3/README.md` & `prophet-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/__init__.py` & `prophet-1.1.4/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/diagnostics.py` & `prophet-1.1.4/prophet/diagnostics.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/forecaster.py` & `prophet-1.1.4/prophet/forecaster.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/hdays.py` & `prophet-1.1.4/prophet/hdays.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 from lunarcalendar import Lunar, Converter
 
 from holidays import WEEKEND, HolidayBase
 from holidays.countries import Turkey
 from dateutil.easter import easter, EASTER_ORTHODOX
 from dateutil.relativedelta import relativedelta as rd
 
+warnings.warn(
+    "hdays module is deprecated and will be removed in prophet 1.1.5. All holidays should be read directly from the holidays package.",
+    FutureWarning,
+)
+
 
 # Official public holidays at a country level
 # ------------ Holidays in Indonesia---------------------
 class Indonesia(HolidayBase):
     """
     Implement public holidays in Indonesia
 
@@ -437,53 +442,53 @@
         # International Women's Day
         name = "International Women's Day"
         self[date(year, 3, 8)] = name
 
         # Nooruz Mairamy
         name = "Nooruz Mairamy"
         self[date(year, 3, 21)] = name
-        
+
         # Day of the People's April Revolution
         name = "Day of the People's April Revolution"
         self[date(year, 4, 7)] = name
-        
+
         # Spring and Labour Day
         name = "Spring and Labour Day"
         self[date(year, 5, 1)] = name
-        
+
         # Constitution Day
         name = "Constitution Day"
         self[date(year, 5, 5)] = name
 
         # Victory Day
         name = "Victory Day"
         self[date(year, 5, 9)] = name
 
         # Children's Day
         name = "Russia Day"
         self[date(year, 6, 1)] = name
-        
+
         # Independence Day
         name = "Independence Day"
         self[date(year, 8, 31)] = name
-        
+
         # Day 1 of History and Commemoration of Ancestors
         name = "Day 1 of History and Commemoration of Ancestors"
         self[date(year, 11, 7)] = name
-        
+
         # Day 2 of History and Commemoration of Ancestors
         name = "Day 2 of History and Commemoration of Ancestors"
         self[date(year, 11, 8)] = name
 
         # New Year's Eve
         name = "New Year's Eve"
         self[date(year, 12, 31)] = name
-        
+
         # Islamic Holidays
-        
+
         # Eid ul-Fitr
         # 1st and 2nd day of 10th Islamic month
         name = "Eid al-Fitr"
         for offset in range(-1, 2, 1):
             islam_year = from_gregorian(year + offset, 6, 15)[0]
             y1, m1, d1 = to_gregorian(islam_year, 10, 1)
             y2, m2, d2 = to_gregorian(islam_year, 10, 2)
```

### Comparing `prophet-1.1.3/prophet/make_holidays.py` & `prophet-1.1.4/prophet/make_holidays.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,46 +2,55 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import absolute_import, division, print_function
 
-import warnings
-
 import numpy as np
 import pandas as pd
 
-import prophet.hdays as hdays_part2
-import holidays as hdays_part1
+import holidays
+
+
+def get_country_holidays_class(country):
+    """Get class for a supported country.
+
+    Parameters
+    ----------
+    country: country code
+
+    Returns
+    -------
+    A valid country holidays class
+    """
+    substitutions = {
+        "TU": "TR",  # For compatibility with Turkey as 'TU' cases.
+    }
+
+    country = substitutions.get(country, country)
+    if not hasattr(holidays, country):
+        raise AttributeError(f"Holidays in {country} are not currently supported!")
+
+    return getattr(holidays, country)
 
 
 def get_holiday_names(country):
     """Return all possible holiday names of given country
 
     Parameters
     ----------
     country: country name
 
     Returns
     -------
     A set of all possible holiday names of given country
     """
-    years = np.arange(1995, 2045)
-    try:
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            holiday_names = getattr(hdays_part2, country)(years=years).values()
-    except AttributeError:
-        try:
-            holiday_names = getattr(hdays_part1, country)(years=years).values()
-        except AttributeError as e:
-            raise AttributeError(f"Holidays in {country} are not currently supported!") from e
-
-    return set(holiday_names)
+    country_holidays = get_country_holidays_class(country)
+    return set(country_holidays(language="en_US", years=np.arange(1995, 2045)).values())
 
 
 def make_holidays_df(year_list, country, province=None, state=None):
     """Make dataframe of holidays for given years and countries
 
     Parameters
     ----------
@@ -49,20 +58,19 @@
     country: country name
 
     Returns
     -------
     Dataframe with 'ds' and 'holiday', which can directly feed
     to 'holidays' params in Prophet
     """
-    try:
-        holidays = getattr(hdays_part2, country)(years=year_list, expand=False)
-    except AttributeError:
-        try:
-            holidays = getattr(hdays_part1, country)(prov=province, state=state, years=year_list, expand=False)
-        except AttributeError as e:
-            raise AttributeError(f"Holidays in {country} are not currently supported!") from e
+    country_holidays = get_country_holidays_class(country)
+    holidays = country_holidays(expand=False, language="en_US", subdiv=province, years=year_list)
 
-    holidays_df = pd.DataFrame([(date, holidays.get_list(date)) for date in holidays], columns=['ds', 'holiday'])
-    holidays_df = holidays_df.explode('holiday')
+    holidays_df = pd.DataFrame(
+        [(date, holidays.get_list(date)) for date in holidays],
+        columns=["ds", "holiday"],
+    )
+    holidays_df = holidays_df.explode("holiday")
     holidays_df.reset_index(inplace=True, drop=True)
-    holidays_df['ds'] = pd.to_datetime(holidays_df['ds'])
-    return (holidays_df)
+    holidays_df["ds"] = pd.to_datetime(holidays_df["ds"])
+
+    return holidays_df
```

### Comparing `prophet-1.1.3/prophet/models.py` & `prophet-1.1.4/prophet/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     @abstractmethod
     def sampling(self, stan_init, stan_data, samples, **kwargs) -> dict:
         pass
 
 
 class CmdStanPyBackend(IStanBackend):
-    CMDSTAN_VERSION = "2.26.1"
+    CMDSTAN_VERSION = "2.31.0"
     def __init__(self):
         import cmdstanpy
         # this must be set before super.__init__() for load_model to work on Windows
         local_cmdstan = importlib_resources.files("prophet") / "stan_model" / f"cmdstan-{self.CMDSTAN_VERSION}"
         if local_cmdstan.exists():
             cmdstanpy.set_cmdstan_path(str(local_cmdstan))
         super().__init__()
```

### Comparing `prophet-1.1.3/prophet/plot.py` & `prophet-1.1.4/prophet/plot.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/serialize.py` & `prophet-1.1.4/prophet/serialize.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/tests/conftest.py` & `prophet-1.1.4/prophet/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/tests/data.csv` & `prophet-1.1.4/prophet/tests/data.csv`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/tests/data2.csv` & `prophet-1.1.4/prophet/tests/data2.csv`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/tests/serialized_model_v0.6.1.dev0.json` & `prophet-1.1.4/prophet/tests/serialized_model_v0.6.1.dev0.json`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-"{\"growth\": \"linear\", \"n_changepoints\": 15, \"specified_changepoints\": false, \"changepoint_range\": 0.8, \"yearly_seasonality\": \"auto\", \"weekly_seasonality\": \"auto\", \"daily_seasonality\": \"auto\", \"seasonality_mode\": \"additive\", \"seasonality_prior_scale\": 10.0, \"changepoint_prior_scale\": 0.05, \"holidays_prior_scale\": 10.0, \"mcmc_samples\": 0, \"interval_width\": 0.8, \"uncertainty_samples\": 1000, \"y_scale\": 19.0, \"logistic_floor\": false, \"country_holidays\": null, \"component_modes\": {\"additive\": [\"weekly\", \"additive_terms\", \"extra_regressors_additive\", \"holidays\"], \"multiplicative\": [\"multiplicative_terms\", \"extra_regressors_multiplicative\"]}, \"fit_kwargs\": {}, \"changepoints\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15],\\\"data\\\":[\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\"]}\", \"history_dates\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19],\\\"data\\\":[\\\"2020-01-01T00:00:00.000Z\\\",\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\",\\\"2020-01-17T00:00:00.000Z\\\",\\\"2020-01-18T00:00:00.000Z\\\",\\\"2020-01-19T00:00:00.000Z\\\",\\\"2020-01-20T00:00:00.000Z\\\"]}\", \"train_holiday_names\": null, \"start\": 1577836800.0, \"t_scale\": 1641600.0, \"holidays\": null, \"history\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"ds\\\",\\\"type\\\":\\\"datetime\\\"},{\\\"name\\\":\\\"y\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"floor\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"t\\\",\\\"type\\\":\\\"number\\\"},{\\\"name\\\":\\\"y_scaled\\\",\\\"type\\\":\\\"number\\\"}],\\\"pandas_version\\\":\\\"0.20.0\\\"},\\\"data\\\":[{\\\"ds\\\":\\\"2020-01-01T00:00:00.000Z\\\",\\\"y\\\":0,\\\"floor\\\":0,\\\"t\\\":0.0,\\\"y_scaled\\\":0.0},{\\\"ds\\\":\\\"2020-01-02T00:00:00.000Z\\\",\\\"y\\\":1,\\\"floor\\\":0,\\\"t\\\":0.0526315789,\\\"y_scaled\\\":0.0526315789},{\\\"ds\\\":\\\"2020-01-03T00:00:00.000Z\\\",\\\"y\\\":2,\\\"floor\\\":0,\\\"t\\\":0.1052631579,\\\"y_scaled\\\":0.1052631579},{\\\"ds\\\":\\\"2020-01-04T00:00:00.000Z\\\",\\\"y\\\":3,\\\"floor\\\":0,\\\"t\\\":0.1578947368,\\\"y_scaled\\\":0.1578947368},{\\\"ds\\\":\\\"2020-01-05T00:00:00.000Z\\\",\\\"y\\\":4,\\\"floor\\\":0,\\\"t\\\":0.2105263158,\\\"y_scaled\\\":0.2105263158},{\\\"ds\\\":\\\"2020-01-06T00:00:00.000Z\\\",\\\"y\\\":5,\\\"floor\\\":0,\\\"t\\\":0.2631578947,\\\"y_scaled\\\":0.2631578947},{\\\"ds\\\":\\\"2020-01-07T00:00:00.000Z\\\",\\\"y\\\":6,\\\"floor\\\":0,\\\"t\\\":0.3157894737,\\\"y_scaled\\\":0.3157894737},{\\\"ds\\\":\\\"2020-01-08T00:00:00.000Z\\\",\\\"y\\\":7,\\\"floor\\\":0,\\\"t\\\":0.3684210526,\\\"y_scaled\\\":0.3684210526},{\\\"ds\\\":\\\"2020-01-09T00:00:00.000Z\\\",\\\"y\\\":8,\\\"floor\\\":0,\\\"t\\\":0.4210526316,\\\"y_scaled\\\":0.4210526316},{\\\"ds\\\":\\\"2020-01-10T00:00:00.000Z\\\",\\\"y\\\":9,\\\"floor\\\":0,\\\"t\\\":0.4736842105,\\\"y_scaled\\\":0.4736842105},{\\\"ds\\\":\\\"2020-01-11T00:00:00.000Z\\\",\\\"y\\\":10,\\\"floor\\\":0,\\\"t\\\":0.5263157895,\\\"y_scaled\\\":0.5263157895},{\\\"ds\\\":\\\"2020-01-12T00:00:00.000Z\\\",\\\"y\\\":11,\\\"floor\\\":0,\\\"t\\\":0.5789473684,\\\"y_scaled\\\":0.5789473684},{\\\"ds\\\":\\\"2020-01-13T00:00:00.000Z\\\",\\\"y\\\":12,\\\"floor\\\":0,\\\"t\\\":0.6315789474,\\\"y_scaled\\\":0.6315789474},{\\\"ds\\\":\\\"2020-01-14T00:00:00.000Z\\\",\\\"y\\\":13,\\\"floor\\\":0,\\\"t\\\":0.6842105263,\\\"y_scaled\\\":0.6842105263},{\\\"ds\\\":\\\"2020-01-15T00:00:00.000Z\\\",\\\"y\\\":14,\\\"floor\\\":0,\\\"t\\\":0.7368421053,\\\"y_scaled\\\":0.7368421053},{\\\"ds\\\":\\\"2020-01-16T00:00:00.000Z\\\",\\\"y\\\":15,\\\"floor\\\":0,\\\"t\\\":0.7894736842,\\\"y_scaled\\\":0.7894736842},{\\\"ds\\\":\\\"2020-01-17T00:00:00.000Z\\\",\\\"y\\\":16,\\\"floor\\\":0,\\\"t\\\":0.8421052632,\\\"y_scaled\\\":0.8421052632},{\\\"ds\\\":\\\"2020-01-18T00:00:00.000Z\\\",\\\"y\\\":17,\\\"floor\\\":0,\\\"t\\\":0.8947368421,\\\"y_scaled\\\":0.8947368421},{\\\"ds\\\":\\\"2020-01-19T00:00:00.000Z\\\",\\\"y\\\":18,\\\"floor\\\":0,\\\"t\\\":0.9473684211,\\\"y_scaled\\\":0.9473684211},{\\\"ds\\\":\\\"2020-01-20T00:00:00.000Z\\\",\\\"y\\\":19,\\\"floor\\\":0,\\\"t\\\":1.0,\\\"y_scaled\\\":1.0}]}\", \"train_component_cols\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"additive_terms\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"weekly\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"multiplicative_terms\\\",\\\"type\\\":\\\"integer\\\"}],\\\"pandas_version\\\":\\\"0.20.0\\\"},\\\"data\\\":[{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0}]}\", \"changepoints_t\": [0.05263157894736842, 0.10526315789473684, 0.15789473684210525, 0.21052631578947367, 0.2631578947368421, 0.3157894736842105, 0.3684210526315789, 0.42105263157894735, 0.47368421052631576, 0.5263157894736842, 0.5789473684210527, 0.631578947368421, 0.6842105263157895, 0.7368421052631579, 0.7894736842105263], \"seasonalities\": [[\"weekly\"], {\"weekly\": {\"period\": 7, \"fourier_order\": 3, \"prior_scale\": 10.0, \"mode\": \"additive\", \"condition_name\": null}}], \"extra_regressors\": [[], {}], \"params\": {\"k\": [[1.0602577093594823]], \"m\": [[-0.004702319079611993]], \"delta\": [[-0.0340439667236795, -8.209452442966747e-14, -2.3754012547042104e-13, 3.543693429450493e-13, -0.1293439581042728, 0.04114775103469311, 0.12224017379322774, -0.03404396672382336, 2.980940404592971e-14, -1.6422578408979347e-13, 3.641514165715795e-13, -0.12934395810441496, 0.0411477510348335, 0.12224017379301462, -0.03404396672364116]], \"sigma_obs\": [[9.77385680687189e-13]], \"beta\": [[-0.0015889307327346812, 0.0029864727119731007, -0.0012450988159614497, -0.0011006619700103823, 0.00041622470940299385, -0.00035495004969666316]]}, \"__fbprophet_version\": \"0.6.1.dev0\"}"
+"{\"growth\": \"linear\", \"n_changepoints\": 15, \"specified_changepoints\": false, \"changepoint_range\": 0.8, \"yearly_seasonality\": \"auto\", \"weekly_seasonality\": \"auto\", \"daily_seasonality\": \"auto\", \"seasonality_mode\": \"additive\", \"seasonality_prior_scale\": 10.0, \"changepoint_prior_scale\": 0.05, \"holidays_prior_scale\": 10.0, \"mcmc_samples\": 0, \"interval_width\": 0.8, \"uncertainty_samples\": 1000, \"y_scale\": 19.0, \"logistic_floor\": false, \"country_holidays\": null, \"component_modes\": {\"additive\": [\"weekly\", \"additive_terms\", \"extra_regressors_additive\", \"holidays\"], \"multiplicative\": [\"multiplicative_terms\", \"extra_regressors_multiplicative\"]}, \"fit_kwargs\": {}, \"changepoints\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15],\\\"data\\\":[\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\"]}\", \"history_dates\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19],\\\"data\\\":[\\\"2020-01-01T00:00:00.000Z\\\",\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\",\\\"2020-01-17T00:00:00.000Z\\\",\\\"2020-01-18T00:00:00.000Z\\\",\\\"2020-01-19T00:00:00.000Z\\\",\\\"2020-01-20T00:00:00.000Z\\\"]}\", \"train_holiday_names\": null, \"start\": 1577836800.0, \"t_scale\": 1641600.0, \"holidays\": null, \"history\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"ds\\\",\\\"type\\\":\\\"string\\\"},{\\\"name\\\":\\\"y\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"floor\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"t\\\",\\\"type\\\":\\\"number\\\"},{\\\"name\\\":\\\"y_scaled\\\",\\\"type\\\":\\\"number\\\"}],\\\"pandas_version\\\":\\\"0.20.0\\\"},\\\"data\\\":[{\\\"ds\\\":\\\"2020-01-01T00:00:00.000Z\\\",\\\"y\\\":0,\\\"floor\\\":0,\\\"t\\\":0.0,\\\"y_scaled\\\":0.0},{\\\"ds\\\":\\\"2020-01-02T00:00:00.000Z\\\",\\\"y\\\":1,\\\"floor\\\":0,\\\"t\\\":0.0526315789,\\\"y_scaled\\\":0.0526315789},{\\\"ds\\\":\\\"2020-01-03T00:00:00.000Z\\\",\\\"y\\\":2,\\\"floor\\\":0,\\\"t\\\":0.1052631579,\\\"y_scaled\\\":0.1052631579},{\\\"ds\\\":\\\"2020-01-04T00:00:00.000Z\\\",\\\"y\\\":3,\\\"floor\\\":0,\\\"t\\\":0.1578947368,\\\"y_scaled\\\":0.1578947368},{\\\"ds\\\":\\\"2020-01-05T00:00:00.000Z\\\",\\\"y\\\":4,\\\"floor\\\":0,\\\"t\\\":0.2105263158,\\\"y_scaled\\\":0.2105263158},{\\\"ds\\\":\\\"2020-01-06T00:00:00.000Z\\\",\\\"y\\\":5,\\\"floor\\\":0,\\\"t\\\":0.2631578947,\\\"y_scaled\\\":0.2631578947},{\\\"ds\\\":\\\"2020-01-07T00:00:00.000Z\\\",\\\"y\\\":6,\\\"floor\\\":0,\\\"t\\\":0.3157894737,\\\"y_scaled\\\":0.3157894737},{\\\"ds\\\":\\\"2020-01-08T00:00:00.000Z\\\",\\\"y\\\":7,\\\"floor\\\":0,\\\"t\\\":0.3684210526,\\\"y_scaled\\\":0.3684210526},{\\\"ds\\\":\\\"2020-01-09T00:00:00.000Z\\\",\\\"y\\\":8,\\\"floor\\\":0,\\\"t\\\":0.4210526316,\\\"y_scaled\\\":0.4210526316},{\\\"ds\\\":\\\"2020-01-10T00:00:00.000Z\\\",\\\"y\\\":9,\\\"floor\\\":0,\\\"t\\\":0.4736842105,\\\"y_scaled\\\":0.4736842105},{\\\"ds\\\":\\\"2020-01-11T00:00:00.000Z\\\",\\\"y\\\":10,\\\"floor\\\":0,\\\"t\\\":0.5263157895,\\\"y_scaled\\\":0.5263157895},{\\\"ds\\\":\\\"2020-01-12T00:00:00.000Z\\\",\\\"y\\\":11,\\\"floor\\\":0,\\\"t\\\":0.5789473684,\\\"y_scaled\\\":0.5789473684},{\\\"ds\\\":\\\"2020-01-13T00:00:00.000Z\\\",\\\"y\\\":12,\\\"floor\\\":0,\\\"t\\\":0.6315789474,\\\"y_scaled\\\":0.6315789474},{\\\"ds\\\":\\\"2020-01-14T00:00:00.000Z\\\",\\\"y\\\":13,\\\"floor\\\":0,\\\"t\\\":0.6842105263,\\\"y_scaled\\\":0.6842105263},{\\\"ds\\\":\\\"2020-01-15T00:00:00.000Z\\\",\\\"y\\\":14,\\\"floor\\\":0,\\\"t\\\":0.7368421053,\\\"y_scaled\\\":0.7368421053},{\\\"ds\\\":\\\"2020-01-16T00:00:00.000Z\\\",\\\"y\\\":15,\\\"floor\\\":0,\\\"t\\\":0.7894736842,\\\"y_scaled\\\":0.7894736842},{\\\"ds\\\":\\\"2020-01-17T00:00:00.000Z\\\",\\\"y\\\":16,\\\"floor\\\":0,\\\"t\\\":0.8421052632,\\\"y_scaled\\\":0.8421052632},{\\\"ds\\\":\\\"2020-01-18T00:00:00.000Z\\\",\\\"y\\\":17,\\\"floor\\\":0,\\\"t\\\":0.8947368421,\\\"y_scaled\\\":0.8947368421},{\\\"ds\\\":\\\"2020-01-19T00:00:00.000Z\\\",\\\"y\\\":18,\\\"floor\\\":0,\\\"t\\\":0.9473684211,\\\"y_scaled\\\":0.9473684211},{\\\"ds\\\":\\\"2020-01-20T00:00:00.000Z\\\",\\\"y\\\":19,\\\"floor\\\":0,\\\"t\\\":1.0,\\\"y_scaled\\\":1.0}]}\", \"train_component_cols\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"additive_terms\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"weekly\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"multiplicative_terms\\\",\\\"type\\\":\\\"integer\\\"}],\\\"pandas_version\\\":\\\"0.20.0\\\"},\\\"data\\\":[{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0}]}\", \"changepoints_t\": [0.05263157894736842, 0.10526315789473684, 0.15789473684210525, 0.21052631578947367, 0.2631578947368421, 0.3157894736842105, 0.3684210526315789, 0.42105263157894735, 0.47368421052631576, 0.5263157894736842, 0.5789473684210527, 0.631578947368421, 0.6842105263157895, 0.7368421052631579, 0.7894736842105263], \"seasonalities\": [[\"weekly\"], {\"weekly\": {\"period\": 7, \"fourier_order\": 3, \"prior_scale\": 10.0, \"mode\": \"additive\", \"condition_name\": null}}], \"extra_regressors\": [[], {}], \"params\": {\"k\": [[1.0602577093594823]], \"m\": [[-0.004702319079611993]], \"delta\": [[-0.0340439667236795, -8.209452442966747e-14, -2.3754012547042104e-13, 3.543693429450493e-13, -0.1293439581042728, 0.04114775103469311, 0.12224017379322774, -0.03404396672382336, 2.980940404592971e-14, -1.6422578408979347e-13, 3.641514165715795e-13, -0.12934395810441496, 0.0411477510348335, 0.12224017379301462, -0.03404396672364116]], \"sigma_obs\": [[9.77385680687189e-13]], \"beta\": [[-0.0015889307327346812, 0.0029864727119731007, -0.0012450988159614497, -0.0011006619700103823, 0.00041622470940299385, -0.00035495004969666316]]}, \"__fbprophet_version\": \"0.6.1.dev0\"}"
```

### Comparing `prophet-1.1.3/prophet/tests/serialized_model_v0.7.1.json` & `prophet-1.1.4/prophet/tests/serialized_model_v0.7.1.json`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-"{\"growth\": \"linear\", \"n_changepoints\": 15, \"specified_changepoints\": false, \"changepoint_range\": 0.8, \"yearly_seasonality\": \"auto\", \"weekly_seasonality\": \"auto\", \"daily_seasonality\": \"auto\", \"seasonality_mode\": \"additive\", \"seasonality_prior_scale\": 10.0, \"changepoint_prior_scale\": 0.05, \"holidays_prior_scale\": 10.0, \"mcmc_samples\": 0, \"interval_width\": 0.8, \"uncertainty_samples\": 1000, \"y_scale\": 19.0, \"logistic_floor\": false, \"country_holidays\": null, \"component_modes\": {\"additive\": [\"weekly\", \"additive_terms\", \"extra_regressors_additive\", \"holidays\"], \"multiplicative\": [\"multiplicative_terms\", \"extra_regressors_multiplicative\"]}, \"fit_kwargs\": {}, \"changepoints\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15],\\\"data\\\":[\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\"]}\", \"history_dates\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19],\\\"data\\\":[\\\"2020-01-01T00:00:00.000Z\\\",\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\",\\\"2020-01-17T00:00:00.000Z\\\",\\\"2020-01-18T00:00:00.000Z\\\",\\\"2020-01-19T00:00:00.000Z\\\",\\\"2020-01-20T00:00:00.000Z\\\"]}\", \"train_holiday_names\": null, \"start\": 1577836800.0, \"t_scale\": 1641600.0, \"holidays\": null, \"history\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"ds\\\",\\\"type\\\":\\\"datetime\\\"},{\\\"name\\\":\\\"y\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"floor\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"t\\\",\\\"type\\\":\\\"number\\\"},{\\\"name\\\":\\\"y_scaled\\\",\\\"type\\\":\\\"number\\\"}],\\\"pandas_version\\\":\\\"0.20.0\\\"},\\\"data\\\":[{\\\"ds\\\":\\\"2020-01-01T00:00:00.000Z\\\",\\\"y\\\":0,\\\"floor\\\":0,\\\"t\\\":0.0,\\\"y_scaled\\\":0.0},{\\\"ds\\\":\\\"2020-01-02T00:00:00.000Z\\\",\\\"y\\\":1,\\\"floor\\\":0,\\\"t\\\":0.0526315789,\\\"y_scaled\\\":0.0526315789},{\\\"ds\\\":\\\"2020-01-03T00:00:00.000Z\\\",\\\"y\\\":2,\\\"floor\\\":0,\\\"t\\\":0.1052631579,\\\"y_scaled\\\":0.1052631579},{\\\"ds\\\":\\\"2020-01-04T00:00:00.000Z\\\",\\\"y\\\":3,\\\"floor\\\":0,\\\"t\\\":0.1578947368,\\\"y_scaled\\\":0.1578947368},{\\\"ds\\\":\\\"2020-01-05T00:00:00.000Z\\\",\\\"y\\\":4,\\\"floor\\\":0,\\\"t\\\":0.2105263158,\\\"y_scaled\\\":0.2105263158},{\\\"ds\\\":\\\"2020-01-06T00:00:00.000Z\\\",\\\"y\\\":5,\\\"floor\\\":0,\\\"t\\\":0.2631578947,\\\"y_scaled\\\":0.2631578947},{\\\"ds\\\":\\\"2020-01-07T00:00:00.000Z\\\",\\\"y\\\":6,\\\"floor\\\":0,\\\"t\\\":0.3157894737,\\\"y_scaled\\\":0.3157894737},{\\\"ds\\\":\\\"2020-01-08T00:00:00.000Z\\\",\\\"y\\\":7,\\\"floor\\\":0,\\\"t\\\":0.3684210526,\\\"y_scaled\\\":0.3684210526},{\\\"ds\\\":\\\"2020-01-09T00:00:00.000Z\\\",\\\"y\\\":8,\\\"floor\\\":0,\\\"t\\\":0.4210526316,\\\"y_scaled\\\":0.4210526316},{\\\"ds\\\":\\\"2020-01-10T00:00:00.000Z\\\",\\\"y\\\":9,\\\"floor\\\":0,\\\"t\\\":0.4736842105,\\\"y_scaled\\\":0.4736842105},{\\\"ds\\\":\\\"2020-01-11T00:00:00.000Z\\\",\\\"y\\\":10,\\\"floor\\\":0,\\\"t\\\":0.5263157895,\\\"y_scaled\\\":0.5263157895},{\\\"ds\\\":\\\"2020-01-12T00:00:00.000Z\\\",\\\"y\\\":11,\\\"floor\\\":0,\\\"t\\\":0.5789473684,\\\"y_scaled\\\":0.5789473684},{\\\"ds\\\":\\\"2020-01-13T00:00:00.000Z\\\",\\\"y\\\":12,\\\"floor\\\":0,\\\"t\\\":0.6315789474,\\\"y_scaled\\\":0.6315789474},{\\\"ds\\\":\\\"2020-01-14T00:00:00.000Z\\\",\\\"y\\\":13,\\\"floor\\\":0,\\\"t\\\":0.6842105263,\\\"y_scaled\\\":0.6842105263},{\\\"ds\\\":\\\"2020-01-15T00:00:00.000Z\\\",\\\"y\\\":14,\\\"floor\\\":0,\\\"t\\\":0.7368421053,\\\"y_scaled\\\":0.7368421053},{\\\"ds\\\":\\\"2020-01-16T00:00:00.000Z\\\",\\\"y\\\":15,\\\"floor\\\":0,\\\"t\\\":0.7894736842,\\\"y_scaled\\\":0.7894736842},{\\\"ds\\\":\\\"2020-01-17T00:00:00.000Z\\\",\\\"y\\\":16,\\\"floor\\\":0,\\\"t\\\":0.8421052632,\\\"y_scaled\\\":0.8421052632},{\\\"ds\\\":\\\"2020-01-18T00:00:00.000Z\\\",\\\"y\\\":17,\\\"floor\\\":0,\\\"t\\\":0.8947368421,\\\"y_scaled\\\":0.8947368421},{\\\"ds\\\":\\\"2020-01-19T00:00:00.000Z\\\",\\\"y\\\":18,\\\"floor\\\":0,\\\"t\\\":0.9473684211,\\\"y_scaled\\\":0.9473684211},{\\\"ds\\\":\\\"2020-01-20T00:00:00.000Z\\\",\\\"y\\\":19,\\\"floor\\\":0,\\\"t\\\":1.0,\\\"y_scaled\\\":1.0}]}\", \"train_component_cols\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"additive_terms\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"weekly\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"multiplicative_terms\\\",\\\"type\\\":\\\"integer\\\"}],\\\"pandas_version\\\":\\\"0.20.0\\\"},\\\"data\\\":[{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0}]}\", \"changepoints_t\": [0.05263157894736842, 0.10526315789473684, 0.15789473684210525, 0.21052631578947367, 0.2631578947368421, 0.3157894736842105, 0.3684210526315789, 0.42105263157894735, 0.47368421052631576, 0.5263157894736842, 0.5789473684210527, 0.631578947368421, 0.6842105263157895, 0.7368421052631579, 0.7894736842105263], \"seasonalities\": [[\"weekly\"], {\"weekly\": {\"period\": 7, \"fourier_order\": 3, \"prior_scale\": 10.0, \"mode\": \"additive\", \"condition_name\": null}}], \"extra_regressors\": [[], {}], \"params\": {\"k\": [[1.02697210905145]], \"m\": [[-0.0030769618763556213]], \"delta\": [[-0.0067713344295760635, -1.8489743725556455e-13, -3.3570135589463447e-14, 2.0851492724135376e-13, -0.05560834408005808, -0.03696006862215325, 0.09933974713183089, -0.006771334429730693, 7.87431718983493e-14, -1.234385828898371e-13, 9.554119248353166e-14, -0.05560834408004029, -0.03696006862202002, 0.09933974713167956, -0.006771334429674014]], \"sigma_obs\": [[3.114271923280071e-13]], \"beta\": [[-0.00034958928816783473, 0.0022663968006279714, -0.0009616626944811777, -0.00018603166834996976, -7.034133451705964e-05, -0.00042298794284303893]], \"trend\": [[-0.0030769618763556213, 0.05097420175793122, 0.10466897936960881, 0.15836375698127664, 0.21205853459294272, 0.2657533122046198, 0.3165213348647148, 0.3653440907552229, 0.4193952543895115, 0.4730900320011826, 0.526784809612858, 0.580479587224527, 0.6341743648362007, 0.6849423874962937, 0.7337651433868063, 0.7878163070210918, 0.8415110846327628, 0.8952058622444338, 0.9489006398561047, 1.0025954174677758]]}, \"__fbprophet_version\": \"0.7.1\"}"
+"{\"growth\": \"linear\", \"n_changepoints\": 15, \"specified_changepoints\": false, \"changepoint_range\": 0.8, \"yearly_seasonality\": \"auto\", \"weekly_seasonality\": \"auto\", \"daily_seasonality\": \"auto\", \"seasonality_mode\": \"additive\", \"seasonality_prior_scale\": 10.0, \"changepoint_prior_scale\": 0.05, \"holidays_prior_scale\": 10.0, \"mcmc_samples\": 0, \"interval_width\": 0.8, \"uncertainty_samples\": 1000, \"y_scale\": 19.0, \"logistic_floor\": false, \"country_holidays\": null, \"component_modes\": {\"additive\": [\"weekly\", \"additive_terms\", \"extra_regressors_additive\", \"holidays\"], \"multiplicative\": [\"multiplicative_terms\", \"extra_regressors_multiplicative\"]}, \"fit_kwargs\": {}, \"changepoints\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15],\\\"data\\\":[\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\"]}\", \"history_dates\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19],\\\"data\\\":[\\\"2020-01-01T00:00:00.000Z\\\",\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\",\\\"2020-01-17T00:00:00.000Z\\\",\\\"2020-01-18T00:00:00.000Z\\\",\\\"2020-01-19T00:00:00.000Z\\\",\\\"2020-01-20T00:00:00.000Z\\\"]}\", \"train_holiday_names\": null, \"start\": 1577836800.0, \"t_scale\": 1641600.0, \"holidays\": null, \"history\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"ds\\\",\\\"type\\\":\\\"string\\\"},{\\\"name\\\":\\\"y\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"floor\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"t\\\",\\\"type\\\":\\\"number\\\"},{\\\"name\\\":\\\"y_scaled\\\",\\\"type\\\":\\\"number\\\"}],\\\"pandas_version\\\":\\\"0.20.0\\\"},\\\"data\\\":[{\\\"ds\\\":\\\"2020-01-01T00:00:00.000Z\\\",\\\"y\\\":0,\\\"floor\\\":0,\\\"t\\\":0.0,\\\"y_scaled\\\":0.0},{\\\"ds\\\":\\\"2020-01-02T00:00:00.000Z\\\",\\\"y\\\":1,\\\"floor\\\":0,\\\"t\\\":0.0526315789,\\\"y_scaled\\\":0.0526315789},{\\\"ds\\\":\\\"2020-01-03T00:00:00.000Z\\\",\\\"y\\\":2,\\\"floor\\\":0,\\\"t\\\":0.1052631579,\\\"y_scaled\\\":0.1052631579},{\\\"ds\\\":\\\"2020-01-04T00:00:00.000Z\\\",\\\"y\\\":3,\\\"floor\\\":0,\\\"t\\\":0.1578947368,\\\"y_scaled\\\":0.1578947368},{\\\"ds\\\":\\\"2020-01-05T00:00:00.000Z\\\",\\\"y\\\":4,\\\"floor\\\":0,\\\"t\\\":0.2105263158,\\\"y_scaled\\\":0.2105263158},{\\\"ds\\\":\\\"2020-01-06T00:00:00.000Z\\\",\\\"y\\\":5,\\\"floor\\\":0,\\\"t\\\":0.2631578947,\\\"y_scaled\\\":0.2631578947},{\\\"ds\\\":\\\"2020-01-07T00:00:00.000Z\\\",\\\"y\\\":6,\\\"floor\\\":0,\\\"t\\\":0.3157894737,\\\"y_scaled\\\":0.3157894737},{\\\"ds\\\":\\\"2020-01-08T00:00:00.000Z\\\",\\\"y\\\":7,\\\"floor\\\":0,\\\"t\\\":0.3684210526,\\\"y_scaled\\\":0.3684210526},{\\\"ds\\\":\\\"2020-01-09T00:00:00.000Z\\\",\\\"y\\\":8,\\\"floor\\\":0,\\\"t\\\":0.4210526316,\\\"y_scaled\\\":0.4210526316},{\\\"ds\\\":\\\"2020-01-10T00:00:00.000Z\\\",\\\"y\\\":9,\\\"floor\\\":0,\\\"t\\\":0.4736842105,\\\"y_scaled\\\":0.4736842105},{\\\"ds\\\":\\\"2020-01-11T00:00:00.000Z\\\",\\\"y\\\":10,\\\"floor\\\":0,\\\"t\\\":0.5263157895,\\\"y_scaled\\\":0.5263157895},{\\\"ds\\\":\\\"2020-01-12T00:00:00.000Z\\\",\\\"y\\\":11,\\\"floor\\\":0,\\\"t\\\":0.5789473684,\\\"y_scaled\\\":0.5789473684},{\\\"ds\\\":\\\"2020-01-13T00:00:00.000Z\\\",\\\"y\\\":12,\\\"floor\\\":0,\\\"t\\\":0.6315789474,\\\"y_scaled\\\":0.6315789474},{\\\"ds\\\":\\\"2020-01-14T00:00:00.000Z\\\",\\\"y\\\":13,\\\"floor\\\":0,\\\"t\\\":0.6842105263,\\\"y_scaled\\\":0.6842105263},{\\\"ds\\\":\\\"2020-01-15T00:00:00.000Z\\\",\\\"y\\\":14,\\\"floor\\\":0,\\\"t\\\":0.7368421053,\\\"y_scaled\\\":0.7368421053},{\\\"ds\\\":\\\"2020-01-16T00:00:00.000Z\\\",\\\"y\\\":15,\\\"floor\\\":0,\\\"t\\\":0.7894736842,\\\"y_scaled\\\":0.7894736842},{\\\"ds\\\":\\\"2020-01-17T00:00:00.000Z\\\",\\\"y\\\":16,\\\"floor\\\":0,\\\"t\\\":0.8421052632,\\\"y_scaled\\\":0.8421052632},{\\\"ds\\\":\\\"2020-01-18T00:00:00.000Z\\\",\\\"y\\\":17,\\\"floor\\\":0,\\\"t\\\":0.8947368421,\\\"y_scaled\\\":0.8947368421},{\\\"ds\\\":\\\"2020-01-19T00:00:00.000Z\\\",\\\"y\\\":18,\\\"floor\\\":0,\\\"t\\\":0.9473684211,\\\"y_scaled\\\":0.9473684211},{\\\"ds\\\":\\\"2020-01-20T00:00:00.000Z\\\",\\\"y\\\":19,\\\"floor\\\":0,\\\"t\\\":1.0,\\\"y_scaled\\\":1.0}]}\", \"train_component_cols\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"additive_terms\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"weekly\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"multiplicative_terms\\\",\\\"type\\\":\\\"integer\\\"}],\\\"pandas_version\\\":\\\"0.20.0\\\"},\\\"data\\\":[{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0}]}\", \"changepoints_t\": [0.05263157894736842, 0.10526315789473684, 0.15789473684210525, 0.21052631578947367, 0.2631578947368421, 0.3157894736842105, 0.3684210526315789, 0.42105263157894735, 0.47368421052631576, 0.5263157894736842, 0.5789473684210527, 0.631578947368421, 0.6842105263157895, 0.7368421052631579, 0.7894736842105263], \"seasonalities\": [[\"weekly\"], {\"weekly\": {\"period\": 7, \"fourier_order\": 3, \"prior_scale\": 10.0, \"mode\": \"additive\", \"condition_name\": null}}], \"extra_regressors\": [[], {}], \"params\": {\"k\": [[1.02697210905145]], \"m\": [[-0.0030769618763556213]], \"delta\": [[-0.0067713344295760635, -1.8489743725556455e-13, -3.3570135589463447e-14, 2.0851492724135376e-13, -0.05560834408005808, -0.03696006862215325, 0.09933974713183089, -0.006771334429730693, 7.87431718983493e-14, -1.234385828898371e-13, 9.554119248353166e-14, -0.05560834408004029, -0.03696006862202002, 0.09933974713167956, -0.006771334429674014]], \"sigma_obs\": [[3.114271923280071e-13]], \"beta\": [[-0.00034958928816783473, 0.0022663968006279714, -0.0009616626944811777, -0.00018603166834996976, -7.034133451705964e-05, -0.00042298794284303893]], \"trend\": [[-0.0030769618763556213, 0.05097420175793122, 0.10466897936960881, 0.15836375698127664, 0.21205853459294272, 0.2657533122046198, 0.3165213348647148, 0.3653440907552229, 0.4193952543895115, 0.4730900320011826, 0.526784809612858, 0.580479587224527, 0.6341743648362007, 0.6849423874962937, 0.7337651433868063, 0.7878163070210918, 0.8415110846327628, 0.8952058622444338, 0.9489006398561047, 1.0025954174677758]]}, \"__fbprophet_version\": \"0.7.1\"}"
```

### Comparing `prophet-1.1.3/prophet/tests/serialized_model_v1.0.1.json` & `prophet-1.1.4/prophet/tests/serialized_model_v1.0.1.json`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-"{\"growth\": \"linear\", \"n_changepoints\": 15, \"specified_changepoints\": false, \"changepoint_range\": 0.8, \"yearly_seasonality\": \"auto\", \"weekly_seasonality\": \"auto\", \"daily_seasonality\": \"auto\", \"seasonality_mode\": \"additive\", \"seasonality_prior_scale\": 10.0, \"changepoint_prior_scale\": 0.05, \"holidays_prior_scale\": 10.0, \"mcmc_samples\": 0, \"interval_width\": 0.8, \"uncertainty_samples\": 1000, \"y_scale\": 19.0, \"logistic_floor\": false, \"country_holidays\": null, \"component_modes\": {\"additive\": [\"weekly\", \"additive_terms\", \"extra_regressors_additive\", \"holidays\"], \"multiplicative\": [\"multiplicative_terms\", \"extra_regressors_multiplicative\"]}, \"changepoints\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15],\\\"data\\\":[\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\"]}\", \"history_dates\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19],\\\"data\\\":[\\\"2020-01-01T00:00:00.000Z\\\",\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\",\\\"2020-01-17T00:00:00.000Z\\\",\\\"2020-01-18T00:00:00.000Z\\\",\\\"2020-01-19T00:00:00.000Z\\\",\\\"2020-01-20T00:00:00.000Z\\\"]}\", \"train_holiday_names\": null, \"start\": 1577836800.0, \"t_scale\": 1641600.0, \"holidays\": null, \"history\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"ds\\\",\\\"type\\\":\\\"datetime\\\"},{\\\"name\\\":\\\"y\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"floor\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"t\\\",\\\"type\\\":\\\"number\\\"},{\\\"name\\\":\\\"y_scaled\\\",\\\"type\\\":\\\"number\\\"}],\\\"pandas_version\\\":\\\"1.4.0\\\"},\\\"data\\\":[{\\\"ds\\\":\\\"2020-01-01T00:00:00.000Z\\\",\\\"y\\\":0,\\\"floor\\\":0,\\\"t\\\":0.0,\\\"y_scaled\\\":0.0},{\\\"ds\\\":\\\"2020-01-02T00:00:00.000Z\\\",\\\"y\\\":1,\\\"floor\\\":0,\\\"t\\\":0.0526315789,\\\"y_scaled\\\":0.0526315789},{\\\"ds\\\":\\\"2020-01-03T00:00:00.000Z\\\",\\\"y\\\":2,\\\"floor\\\":0,\\\"t\\\":0.1052631579,\\\"y_scaled\\\":0.1052631579},{\\\"ds\\\":\\\"2020-01-04T00:00:00.000Z\\\",\\\"y\\\":3,\\\"floor\\\":0,\\\"t\\\":0.1578947368,\\\"y_scaled\\\":0.1578947368},{\\\"ds\\\":\\\"2020-01-05T00:00:00.000Z\\\",\\\"y\\\":4,\\\"floor\\\":0,\\\"t\\\":0.2105263158,\\\"y_scaled\\\":0.2105263158},{\\\"ds\\\":\\\"2020-01-06T00:00:00.000Z\\\",\\\"y\\\":5,\\\"floor\\\":0,\\\"t\\\":0.2631578947,\\\"y_scaled\\\":0.2631578947},{\\\"ds\\\":\\\"2020-01-07T00:00:00.000Z\\\",\\\"y\\\":6,\\\"floor\\\":0,\\\"t\\\":0.3157894737,\\\"y_scaled\\\":0.3157894737},{\\\"ds\\\":\\\"2020-01-08T00:00:00.000Z\\\",\\\"y\\\":7,\\\"floor\\\":0,\\\"t\\\":0.3684210526,\\\"y_scaled\\\":0.3684210526},{\\\"ds\\\":\\\"2020-01-09T00:00:00.000Z\\\",\\\"y\\\":8,\\\"floor\\\":0,\\\"t\\\":0.4210526316,\\\"y_scaled\\\":0.4210526316},{\\\"ds\\\":\\\"2020-01-10T00:00:00.000Z\\\",\\\"y\\\":9,\\\"floor\\\":0,\\\"t\\\":0.4736842105,\\\"y_scaled\\\":0.4736842105},{\\\"ds\\\":\\\"2020-01-11T00:00:00.000Z\\\",\\\"y\\\":10,\\\"floor\\\":0,\\\"t\\\":0.5263157895,\\\"y_scaled\\\":0.5263157895},{\\\"ds\\\":\\\"2020-01-12T00:00:00.000Z\\\",\\\"y\\\":11,\\\"floor\\\":0,\\\"t\\\":0.5789473684,\\\"y_scaled\\\":0.5789473684},{\\\"ds\\\":\\\"2020-01-13T00:00:00.000Z\\\",\\\"y\\\":12,\\\"floor\\\":0,\\\"t\\\":0.6315789474,\\\"y_scaled\\\":0.6315789474},{\\\"ds\\\":\\\"2020-01-14T00:00:00.000Z\\\",\\\"y\\\":13,\\\"floor\\\":0,\\\"t\\\":0.6842105263,\\\"y_scaled\\\":0.6842105263},{\\\"ds\\\":\\\"2020-01-15T00:00:00.000Z\\\",\\\"y\\\":14,\\\"floor\\\":0,\\\"t\\\":0.7368421053,\\\"y_scaled\\\":0.7368421053},{\\\"ds\\\":\\\"2020-01-16T00:00:00.000Z\\\",\\\"y\\\":15,\\\"floor\\\":0,\\\"t\\\":0.7894736842,\\\"y_scaled\\\":0.7894736842},{\\\"ds\\\":\\\"2020-01-17T00:00:00.000Z\\\",\\\"y\\\":16,\\\"floor\\\":0,\\\"t\\\":0.8421052632,\\\"y_scaled\\\":0.8421052632},{\\\"ds\\\":\\\"2020-01-18T00:00:00.000Z\\\",\\\"y\\\":17,\\\"floor\\\":0,\\\"t\\\":0.8947368421,\\\"y_scaled\\\":0.8947368421},{\\\"ds\\\":\\\"2020-01-19T00:00:00.000Z\\\",\\\"y\\\":18,\\\"floor\\\":0,\\\"t\\\":0.9473684211,\\\"y_scaled\\\":0.9473684211},{\\\"ds\\\":\\\"2020-01-20T00:00:00.000Z\\\",\\\"y\\\":19,\\\"floor\\\":0,\\\"t\\\":1.0,\\\"y_scaled\\\":1.0}]}\", \"train_component_cols\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"additive_terms\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"weekly\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"multiplicative_terms\\\",\\\"type\\\":\\\"integer\\\"}],\\\"pandas_version\\\":\\\"1.4.0\\\"},\\\"data\\\":[{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0}]}\", \"changepoints_t\": [0.05263157894736842, 0.10526315789473684, 0.15789473684210525, 0.21052631578947367, 0.2631578947368421, 0.3157894736842105, 0.3684210526315789, 0.42105263157894735, 0.47368421052631576, 0.5263157894736842, 0.5789473684210527, 0.631578947368421, 0.6842105263157895, 0.7368421052631579, 0.7894736842105263], \"seasonalities\": [[\"weekly\"], {\"weekly\": {\"period\": 7, \"fourier_order\": 3, \"prior_scale\": 10.0, \"mode\": \"additive\", \"condition_name\": null}}], \"extra_regressors\": [[], {}], \"fit_kwargs\": {}, \"params\": {\"k\": [[1.02697210905145]], \"m\": [[-0.0030769618763556213]], \"delta\": [[-0.0067713344295760635, -1.8489743725556455e-13, -3.3570135589463447e-14, 2.0851492724135376e-13, -0.05560834408005808, -0.03696006862215325, 0.09933974713183089, -0.006771334429730693, 7.87431718983493e-14, -1.234385828898371e-13, 9.554119248353166e-14, -0.05560834408004029, -0.03696006862202002, 0.09933974713167956, -0.006771334429674014]], \"sigma_obs\": [[3.114271923280071e-13]], \"beta\": [[-0.00034958928816783473, 0.0022663968006279714, -0.0009616626944811777, -0.00018603166834996976, -7.034133451705964e-05, -0.00042298794284303893]], \"trend\": [[-0.0030769618763556213, 0.05097420175793122, 0.10466897936960881, 0.15836375698127664, 0.21205853459294272, 0.2657533122046198, 0.3165213348647148, 0.3653440907552229, 0.4193952543895115, 0.4730900320011826, 0.526784809612858, 0.580479587224527, 0.6341743648362007, 0.6849423874962937, 0.7337651433868063, 0.7878163070210918, 0.8415110846327628, 0.8952058622444338, 0.9489006398561047, 1.0025954174677758]]}, \"__prophet_version\": \"1.0.1\"}"
+"{\"growth\": \"linear\", \"n_changepoints\": 15, \"specified_changepoints\": false, \"changepoint_range\": 0.8, \"yearly_seasonality\": \"auto\", \"weekly_seasonality\": \"auto\", \"daily_seasonality\": \"auto\", \"seasonality_mode\": \"additive\", \"seasonality_prior_scale\": 10.0, \"changepoint_prior_scale\": 0.05, \"holidays_prior_scale\": 10.0, \"mcmc_samples\": 0, \"interval_width\": 0.8, \"uncertainty_samples\": 1000, \"y_scale\": 19.0, \"logistic_floor\": false, \"country_holidays\": null, \"component_modes\": {\"additive\": [\"weekly\", \"additive_terms\", \"extra_regressors_additive\", \"holidays\"], \"multiplicative\": [\"multiplicative_terms\", \"extra_regressors_multiplicative\"]}, \"changepoints\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15],\\\"data\\\":[\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\"]}\", \"history_dates\": \"{\\\"name\\\":\\\"ds\\\",\\\"index\\\":[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19],\\\"data\\\":[\\\"2020-01-01T00:00:00.000Z\\\",\\\"2020-01-02T00:00:00.000Z\\\",\\\"2020-01-03T00:00:00.000Z\\\",\\\"2020-01-04T00:00:00.000Z\\\",\\\"2020-01-05T00:00:00.000Z\\\",\\\"2020-01-06T00:00:00.000Z\\\",\\\"2020-01-07T00:00:00.000Z\\\",\\\"2020-01-08T00:00:00.000Z\\\",\\\"2020-01-09T00:00:00.000Z\\\",\\\"2020-01-10T00:00:00.000Z\\\",\\\"2020-01-11T00:00:00.000Z\\\",\\\"2020-01-12T00:00:00.000Z\\\",\\\"2020-01-13T00:00:00.000Z\\\",\\\"2020-01-14T00:00:00.000Z\\\",\\\"2020-01-15T00:00:00.000Z\\\",\\\"2020-01-16T00:00:00.000Z\\\",\\\"2020-01-17T00:00:00.000Z\\\",\\\"2020-01-18T00:00:00.000Z\\\",\\\"2020-01-19T00:00:00.000Z\\\",\\\"2020-01-20T00:00:00.000Z\\\"]}\", \"train_holiday_names\": null, \"start\": 1577836800.0, \"t_scale\": 1641600.0, \"holidays\": null, \"history\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"ds\\\",\\\"type\\\":\\\"string\\\"},{\\\"name\\\":\\\"y\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"floor\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"t\\\",\\\"type\\\":\\\"number\\\"},{\\\"name\\\":\\\"y_scaled\\\",\\\"type\\\":\\\"number\\\"}],\\\"pandas_version\\\":\\\"1.4.0\\\"},\\\"data\\\":[{\\\"ds\\\":\\\"2020-01-01T00:00:00.000Z\\\",\\\"y\\\":0,\\\"floor\\\":0,\\\"t\\\":0.0,\\\"y_scaled\\\":0.0},{\\\"ds\\\":\\\"2020-01-02T00:00:00.000Z\\\",\\\"y\\\":1,\\\"floor\\\":0,\\\"t\\\":0.0526315789,\\\"y_scaled\\\":0.0526315789},{\\\"ds\\\":\\\"2020-01-03T00:00:00.000Z\\\",\\\"y\\\":2,\\\"floor\\\":0,\\\"t\\\":0.1052631579,\\\"y_scaled\\\":0.1052631579},{\\\"ds\\\":\\\"2020-01-04T00:00:00.000Z\\\",\\\"y\\\":3,\\\"floor\\\":0,\\\"t\\\":0.1578947368,\\\"y_scaled\\\":0.1578947368},{\\\"ds\\\":\\\"2020-01-05T00:00:00.000Z\\\",\\\"y\\\":4,\\\"floor\\\":0,\\\"t\\\":0.2105263158,\\\"y_scaled\\\":0.2105263158},{\\\"ds\\\":\\\"2020-01-06T00:00:00.000Z\\\",\\\"y\\\":5,\\\"floor\\\":0,\\\"t\\\":0.2631578947,\\\"y_scaled\\\":0.2631578947},{\\\"ds\\\":\\\"2020-01-07T00:00:00.000Z\\\",\\\"y\\\":6,\\\"floor\\\":0,\\\"t\\\":0.3157894737,\\\"y_scaled\\\":0.3157894737},{\\\"ds\\\":\\\"2020-01-08T00:00:00.000Z\\\",\\\"y\\\":7,\\\"floor\\\":0,\\\"t\\\":0.3684210526,\\\"y_scaled\\\":0.3684210526},{\\\"ds\\\":\\\"2020-01-09T00:00:00.000Z\\\",\\\"y\\\":8,\\\"floor\\\":0,\\\"t\\\":0.4210526316,\\\"y_scaled\\\":0.4210526316},{\\\"ds\\\":\\\"2020-01-10T00:00:00.000Z\\\",\\\"y\\\":9,\\\"floor\\\":0,\\\"t\\\":0.4736842105,\\\"y_scaled\\\":0.4736842105},{\\\"ds\\\":\\\"2020-01-11T00:00:00.000Z\\\",\\\"y\\\":10,\\\"floor\\\":0,\\\"t\\\":0.5263157895,\\\"y_scaled\\\":0.5263157895},{\\\"ds\\\":\\\"2020-01-12T00:00:00.000Z\\\",\\\"y\\\":11,\\\"floor\\\":0,\\\"t\\\":0.5789473684,\\\"y_scaled\\\":0.5789473684},{\\\"ds\\\":\\\"2020-01-13T00:00:00.000Z\\\",\\\"y\\\":12,\\\"floor\\\":0,\\\"t\\\":0.6315789474,\\\"y_scaled\\\":0.6315789474},{\\\"ds\\\":\\\"2020-01-14T00:00:00.000Z\\\",\\\"y\\\":13,\\\"floor\\\":0,\\\"t\\\":0.6842105263,\\\"y_scaled\\\":0.6842105263},{\\\"ds\\\":\\\"2020-01-15T00:00:00.000Z\\\",\\\"y\\\":14,\\\"floor\\\":0,\\\"t\\\":0.7368421053,\\\"y_scaled\\\":0.7368421053},{\\\"ds\\\":\\\"2020-01-16T00:00:00.000Z\\\",\\\"y\\\":15,\\\"floor\\\":0,\\\"t\\\":0.7894736842,\\\"y_scaled\\\":0.7894736842},{\\\"ds\\\":\\\"2020-01-17T00:00:00.000Z\\\",\\\"y\\\":16,\\\"floor\\\":0,\\\"t\\\":0.8421052632,\\\"y_scaled\\\":0.8421052632},{\\\"ds\\\":\\\"2020-01-18T00:00:00.000Z\\\",\\\"y\\\":17,\\\"floor\\\":0,\\\"t\\\":0.8947368421,\\\"y_scaled\\\":0.8947368421},{\\\"ds\\\":\\\"2020-01-19T00:00:00.000Z\\\",\\\"y\\\":18,\\\"floor\\\":0,\\\"t\\\":0.9473684211,\\\"y_scaled\\\":0.9473684211},{\\\"ds\\\":\\\"2020-01-20T00:00:00.000Z\\\",\\\"y\\\":19,\\\"floor\\\":0,\\\"t\\\":1.0,\\\"y_scaled\\\":1.0}]}\", \"train_component_cols\": \"{\\\"schema\\\":{\\\"fields\\\":[{\\\"name\\\":\\\"additive_terms\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"weekly\\\",\\\"type\\\":\\\"integer\\\"},{\\\"name\\\":\\\"multiplicative_terms\\\",\\\"type\\\":\\\"integer\\\"}],\\\"pandas_version\\\":\\\"1.4.0\\\"},\\\"data\\\":[{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0},{\\\"additive_terms\\\":1,\\\"weekly\\\":1,\\\"multiplicative_terms\\\":0}]}\", \"changepoints_t\": [0.05263157894736842, 0.10526315789473684, 0.15789473684210525, 0.21052631578947367, 0.2631578947368421, 0.3157894736842105, 0.3684210526315789, 0.42105263157894735, 0.47368421052631576, 0.5263157894736842, 0.5789473684210527, 0.631578947368421, 0.6842105263157895, 0.7368421052631579, 0.7894736842105263], \"seasonalities\": [[\"weekly\"], {\"weekly\": {\"period\": 7, \"fourier_order\": 3, \"prior_scale\": 10.0, \"mode\": \"additive\", \"condition_name\": null}}], \"extra_regressors\": [[], {}], \"fit_kwargs\": {}, \"params\": {\"k\": [[1.02697210905145]], \"m\": [[-0.0030769618763556213]], \"delta\": [[-0.0067713344295760635, -1.8489743725556455e-13, -3.3570135589463447e-14, 2.0851492724135376e-13, -0.05560834408005808, -0.03696006862215325, 0.09933974713183089, -0.006771334429730693, 7.87431718983493e-14, -1.234385828898371e-13, 9.554119248353166e-14, -0.05560834408004029, -0.03696006862202002, 0.09933974713167956, -0.006771334429674014]], \"sigma_obs\": [[3.114271923280071e-13]], \"beta\": [[-0.00034958928816783473, 0.0022663968006279714, -0.0009616626944811777, -0.00018603166834996976, -7.034133451705964e-05, -0.00042298794284303893]], \"trend\": [[-0.0030769618763556213, 0.05097420175793122, 0.10466897936960881, 0.15836375698127664, 0.21205853459294272, 0.2657533122046198, 0.3165213348647148, 0.3653440907552229, 0.4193952543895115, 0.4730900320011826, 0.526784809612858, 0.580479587224527, 0.6341743648362007, 0.6849423874962937, 0.7337651433868063, 0.7878163070210918, 0.8415110846327628, 0.8952058622444338, 0.9489006398561047, 1.0025954174677758]]}, \"__prophet_version\": \"1.0.1\"}"
```

### Comparing `prophet-1.1.3/prophet/tests/test_diagnostics.py` & `prophet-1.1.4/prophet/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/tests/test_prophet.py` & `prophet-1.1.4/prophet/tests/test_prophet.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/tests/test_serialize.py` & `prophet-1.1.4/prophet/tests/test_serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,14 @@
         assert m2.stan_fit is None
         assert m2.stan_backend is None
 
         # Check that m2 makes the same forecast
         fcst2 = m2.predict(test)
         assert np.array_equal(fcst["yhat"].values, fcst2["yhat"].values)
 
-    @pytest.mark.skip(reason="skipping until json serialization issue in pandas 2.0 is resolved.")
     def test_backwards_compatibility(self):
         old_versions = {
             "0.6.1.dev0": (29.3669923968994, "fb"),
             "0.7.1": (29.282810844704414, "fb"),
             "1.0.1": (29.282810844704414, ""),
         }
         for v, (pred_val, v_str) in old_versions.items():
```

### Comparing `prophet-1.1.3/prophet/tests/test_utilities.py` & `prophet-1.1.4/prophet/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet/utilities.py` & `prophet-1.1.4/prophet/utilities.py`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/prophet.egg-info/PKG-INFO` & `prophet-1.1.4/prophet.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophet
-Version: 1.1.3
+Version: 1.1.4
 Summary: Automatic Forecasting Procedure
 Author-email: "Sean J. Taylor" <sjtz@pm.me>, Ben Letham <bletham@fb.com>
 Maintainer-email: Cuong Duong <cuong.duong242@gmail.com>
 License: MIT
 Project-URL: Homepage, https://facebook.github.io/prophet/
 Project-URL: Documentation, https://facebook.github.io/prophet/
 Project-URL: Repository, https://github.com/facebook/prophet
```

### Comparing `prophet-1.1.3/prophet.egg-info/SOURCES.txt` & `prophet-1.1.4/prophet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prophet-1.1.3/pyproject.toml` & `prophet-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 dependencies = [
   "cmdstanpy>=1.0.4",
   "numpy>=1.15.4",
   "matplotlib>=2.0.0",
   "pandas>=1.0.4",
   "LunarCalendar>=0.0.9",
   "convertdate>=2.1.2",
-  "holidays>=0.14.2",
+  "holidays>=0.25",
   "python-dateutil>=2.8.0",
   "tqdm>=4.36.1",
   "importlib_resources",
 ]
 authors = [
   {name = "Sean J. Taylor", email = "sjtz@pm.me"},
   {name = "Ben Letham", email = "bletham@fb.com"},
```

### Comparing `prophet-1.1.3/setup.py` & `prophet-1.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,32 +4,35 @@
 # LICENSE file in the root directory of this source tree.
 
 import os
 import platform
 from pathlib import Path
 from shutil import copy, copytree, rmtree
 from typing import List
+import tempfile
 
 from setuptools import find_packages, setup, Extension
 from setuptools.command.build_ext import build_ext
 from setuptools.command.build_py import build_py
 from setuptools.command.editable_wheel import editable_wheel
 from wheel.bdist_wheel import bdist_wheel
 
 
 MODEL_DIR = "stan"
 MODEL_TARGET_DIR = os.path.join("prophet", "stan_model")
 
-CMDSTAN_VERSION = "2.26.1"
+CMDSTAN_VERSION = "2.31.0"
 BINARIES_DIR = "bin"
 BINARIES = ["diagnose", "print", "stanc", "stansummary"]
 TBB_PARENT = "stan/lib/stan_math/lib"
-TBB_DIRS = ["tbb", "tbb_2019_U8"]
+TBB_DIRS = ["tbb", "tbb_2020.3"]
 
 
+IS_WINDOWS = platform.platform().startswith("Win")
+
 def prune_cmdstan(cmdstan_dir: str) -> None:
     """
     Keep only the cmdstan executables and tbb files (minimum required to run a cmdstanpy commands on a pre-compiled model).
     """
     original_dir = Path(cmdstan_dir).resolve()
     parent_dir = original_dir.parent
     temp_dir = parent_dir / "temp"
@@ -51,50 +54,52 @@
     temp_dir.rename(original_dir)
 
 
 def repackage_cmdstan():
     return os.environ.get("PROPHET_REPACKAGE_CMDSTAN", "").lower() not in ["false", "0"]
 
 
-def maybe_install_cmdstan_toolchain():
+def maybe_install_cmdstan_toolchain() -> bool:
     """Install C++ compilers required to build stan models on Windows machines."""
     import cmdstanpy
 
     try:
         cmdstanpy.utils.cxx_toolchain_path()
+        return False
     except Exception:
         try:
             from cmdstanpy.install_cxx_toolchain import run_rtools_install
         except ImportError:
             # older versions
             from cmdstanpy.install_cxx_toolchain import main as run_rtools_install
 
         run_rtools_install({"version": None, "dir": None, "verbose": True})
         cmdstanpy.utils.cxx_toolchain_path()
-
+        return True
 
 def install_cmdstan_deps(cmdstan_dir: Path):
     import cmdstanpy
     from multiprocessing import cpu_count
 
     if repackage_cmdstan():
-        if platform.platform().startswith("Win"):
+        if IS_WINDOWS:
             maybe_install_cmdstan_toolchain()
         print("Installing cmdstan to", cmdstan_dir)
         if os.path.isdir(cmdstan_dir):
             rmtree(cmdstan_dir)
 
         if not cmdstanpy.install_cmdstan(
             version=CMDSTAN_VERSION,
             dir=cmdstan_dir.parent,
             overwrite=True,
             verbose=True,
             cores=cpu_count(),
             progress=True,
         ):
+
             raise RuntimeError("CmdStan failed to install in repackaged directory")
 
 
 def build_cmdstan_model(target_dir):
     """
     Rebuild cmdstan in the build environment, then use this installation to compile the stan model.
     The stan model is copied to {target_dir}/prophet_model.bin
@@ -102,28 +107,40 @@
 
     Parameters
     ----------
     target_dir: Directory to copy the compiled model executable and core cmdstan files to.
     """
     import cmdstanpy
 
-    cmdstan_dir = (Path(target_dir) / f"cmdstan-{CMDSTAN_VERSION}").resolve()
-    install_cmdstan_deps(cmdstan_dir)
-    model_name = "prophet.stan"
-    target_name = "prophet_model.bin"
-    sm = cmdstanpy.CmdStanModel(stan_file=os.path.join(MODEL_DIR, model_name))
-    copy(sm.exe_file, os.path.join(target_dir, target_name))
+    target_cmdstan_dir = (Path(target_dir) / f"cmdstan-{CMDSTAN_VERSION}").resolve()
+    with tempfile.TemporaryDirectory() as tmp_dir:
+        # long paths on windows can cause problems during build
+        if IS_WINDOWS:
+            cmdstan_dir = (Path(tmp_dir) / f"cmdstan-{CMDSTAN_VERSION}").resolve()
+        else:
+            cmdstan_dir = target_cmdstan_dir
+
+        install_cmdstan_deps(cmdstan_dir)
+        model_name = "prophet.stan"
+
+        temp_stan_file = copy(os.path.join(MODEL_DIR, model_name), cmdstan_dir)
+        sm = cmdstanpy.CmdStanModel(stan_file=temp_stan_file)
+        target_name = "prophet_model.bin"
+        copy(sm.exe_file, os.path.join(target_dir, target_name))
+
+        if IS_WINDOWS:
+            copytree(cmdstan_dir, target_cmdstan_dir)
 
     # Clean up
     for f in Path(MODEL_DIR).iterdir():
         if f.is_file() and f.name != model_name:
             os.remove(f)
 
     if repackage_cmdstan():
-        prune_cmdstan(cmdstan_dir)
+        prune_cmdstan(target_cmdstan_dir)
 
 
 def get_backends_from_env() -> List[str]:
     return os.environ.get("STAN_BACKEND", "CMDSTANPY").split(",")
 
 
 def build_models(target_dir):
```

### Comparing `prophet-1.1.3/stan/prophet.stan` & `prophet-1.1.4/stan/prophet.stan`

 * *Files identical despite different names*

