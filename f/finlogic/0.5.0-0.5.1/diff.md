# Comparing `tmp/finlogic-0.5.0.tar.gz` & `tmp/finlogic-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.5.0.tar", last modified: Thu May 25 23:14:58 2023, max compression
+gzip compressed data, was "finlogic-0.5.1.tar", last modified: Mon May 29 09:58:56 2023, max compression
```

## Comparing `finlogic-0.5.0.tar` & `finlogic-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.5.0/LICENSE
--rw-r--r--   0        0        0     9178 2023-05-25 21:55:04.282408 finlogic-0.5.0/README.md
--rw-r--r--   0        0        0      391 2023-05-24 09:12:22.015110 finlogic-0.5.0/finlogic/__init__.py
--rw-r--r--   0        0        0    23644 2023-05-25 22:49:23.698153 finlogic-0.5.0/finlogic/company.py
--rw-r--r--   0        0        0      159 2023-05-25 10:59:30.819065 finlogic-0.5.0/finlogic/config.py
--rw-r--r--   0        0        0    13151 2023-05-25 21:45:27.482813 finlogic-0.5.0/finlogic/cvm.py
--rw-r--r--   0        0        0     5406 2023-05-25 23:03:39.330450 finlogic-0.5.0/finlogic/data_manager.py
--rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.5.0/finlogic/language.py
--rw-r--r--   0        0        0     1017 2023-05-25 23:14:58.671033 finlogic-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     3354 2023-05-23 23:02:21.956066 finlogic-0.5.0/tests/test_company.py
--rw-r--r--   0        0        0      907 2023-05-25 23:05:44.826667 finlogic-0.5.0/tests/test_data.py
--rw-r--r--   0        0        0    11257 1970-01-01 00:00:00.000000 finlogic-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.5.1/LICENSE
+-rw-r--r--   0        0        0     9039 2023-05-26 08:29:09.365843 finlogic-0.5.1/README.md
+-rw-r--r--   0        0        0      391 2023-05-29 09:45:14.175716 finlogic-0.5.1/finlogic/__init__.py
+-rw-r--r--   0        0        0     5343 2023-05-29 09:53:24.121282 finlogic-0.5.1/finlogic/builder.py
+-rw-r--r--   0        0        0    22909 2023-05-29 09:45:14.175716 finlogic-0.5.1/finlogic/company.py
+-rw-r--r--   0        0        0      406 2023-05-27 17:07:48.111310 finlogic-0.5.1/finlogic/config.py
+-rw-r--r--   0        0        0    10631 2023-05-29 09:45:14.175716 finlogic-0.5.1/finlogic/cvm.py
+-rw-r--r--   0        0        0     5429 2023-05-27 17:20:46.327158 finlogic-0.5.1/finlogic/data_manager.py
+-rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.5.1/finlogic/language.py
+-rw-r--r--   0        0        0     1017 2023-05-29 09:58:56.796383 finlogic-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     3354 2023-05-25 23:18:10.569891 finlogic-0.5.1/tests/test_company.py
+-rw-r--r--   0        0        0      907 2023-05-25 23:18:10.569891 finlogic-0.5.1/tests/test_data.py
+-rw-r--r--   0        0        0    11118 1970-01-01 00:00:00.000000 finlogic-0.5.1/PKG-INFO
```

### Comparing `finlogic-0.5.0/LICENSE` & `finlogic-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.5.0/README.md` & `finlogic-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 ---
 
 ## Quick Start
 
 ### Create FinLogic Database
 
-The 'update' function is responsible for downloading and updating raw financial data from the CVM, processing approximately 20 million accounting entries, and storing them for local data analysis. During the initial run, the process might take longer than 1 minute, depending on the CVM server connection and local CPU power. For subsequent updates, only the updated CVM files will be downloaded and processed, which should expedite the operation.
+The 'update' function is responsible for downloading and updating raw financial data from the CVM, processing approximately 20 million accounting entries, and storing them for local data analysis. During the initial run, the process might take some minutes, depending on the CVM server connection and local CPU power. For subsequent updates, only the updated CVM files will be downloaded and processed, which should expedite the operation.
 
 ```python
 >>> import finlogic as fl
 
 # Compile FinLogic database for the first time:
 >>> fl.update()
 
@@ -51,24 +51,24 @@
 ...
 FinLogic database updated ✅
 
 # Show database info:
 >>> fl.info()
 ```
 
-| FinLogic Database Info |                         Value |
-| :--------------------- | ----------------------------: |
-| db_path                | .../finlogic/data/finlogic.db |
-| db_size                |                       76.0 MB |
-| db_last_modified       |           2023-04-20 07:29:08 |
-| number_of_companies    |                         1,139 |
-| number_of_rows         |                     2,806,635 |
-| number_of_reports      |                         9,422 |
-| first_report           |                    2009-01-31 |
-| last_report            |                    2023-03-31 |
+|                     |       FinLogic Info |
+| :------------------ | ------------------: |
+| data_path           |   .../finlogic/data |
+| data_size           |             12.1 MB |
+| last_modified_on    | 2023-04-20 07:29:08 |
+| accounting_entries  |           2,806,635 |
+| number_of_reports   |              11,635 |
+| first_report        |          2009-01-31 |
+| last_report         |          2023-03-31 |
+| number_of_companies |               1,139 |
 
 ```python
 # Search for a company in database:
 >>> fl.search_company('petro')
 ```
 
 |     | name_id                                | cvm_id | tax_id             |
@@ -85,38 +85,38 @@
 ### The Company Class
 
 The Company Class allows you to easily access financial data from Brazilian companies. All values are in local currency (Real).
 
 ```python
 # Create a Company object to acces its financial data:
 # Both CVM (regulator) ID or Fiscal ID can be used as an identifier.
->>> petro = fl.Company(9512, is_consolidated='sep', acc_unit='m')
+>>> petro = fl.Company(9512, is_consolidated=False, acc_unit='m')
 
 # Change company accounting method back to consolidated (default):
->>> petro.is_consolidated = 'con'
+>>> petro.is_consolidated = True
 
 # Change company accounting unit to billion (default is 1):
 >>> petro.acc_unit = 'b'
 
 # Show company info:
 >>> petro.info()
 ```
 
-| Company Info               |                             Values |
+|                            |                       Company Info |
 | :------------------------- | ---------------------------------: |
 | Name                       | PETROLEO BRASILEIRO S.A. PETROBRAS |
 | CVM ID                     |                               9512 |
-| Fiscal ID (CNPJ)           |                 33.000.167/0001-01 |
-| Total Accounting Rows      |                             39,292 |
+| Tax ID (CNPJ)              |                 33.000.167/0001-01 |
+| Total Accounting Rows      |                              3,292 |
 | Selected Tax Rate          |                               0.34 |
 | Selected Accounting Method |                       consolidated |
 | Selected Accounting Unit   |                      1,000,000,000 |
-| First Annual Report        |                         2009-12-31 |
-| Last Annual Report         |                         2021-12-31 |
-| Last Quarterly Report      |                         2021-09-30 |
+| First Report               |                         2009-12-31 |
+| Last Report                |                         2021-12-31 |
+| Last Report Type           |                          quarterly |
 
 ```python
 # Show company assets in Brazilian currency:
 >>> petro.report(report_type='assets')
 ...
 # Show company liabilities with custom arguments:
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
```

### Comparing `finlogic-0.5.0/finlogic/company.py` & `finlogic-0.5.1/finlogic/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,21 +262,27 @@
         )
 
         # Convert category columns back to string
         columns = df.columns
         cat_cols = [c for c in columns if df[c].dtype == "category"]
         df[cat_cols] = df[cat_cols].astype("string")
 
-        # Change acc_value only when it is not earnings_per_share (acc_code 8)
+        # Change acc_value only when it is not earnings_per_share (report_type 8)
         df["acc_value"] = np.where(
-            df["acc_code"].str.startswith("8"),
+            df["report_type"] == 8,
             df["acc_value"],
             df["acc_value"] / self._acc_unit,
         )
 
+        # Remove quarters entries that are not the last one
+        mask1 = ~df["is_annual"]
+        mask2 = df["period_end"] != df["period_end"].max()
+        mask = mask1 & mask2
+        df = df[~mask].reset_index(drop=True)
+
         self._first_period = df["period_end"].min()
         self._last_period = df["period_end"].max()
 
         # Not necessarily there will be a quarterly report for the last period
         self._last_annual = df.query("is_annual")["period_end"].max()
 
         if self._last_period == self._last_annual:
@@ -334,24 +340,41 @@
         dfo = self._build_report_index(dfi)
         year_cols = ["acc_code", "acc_value"]
         periods = sorted(dfi["period_end"].drop_duplicates())
         for period in periods:
             df_year = dfi.query("period_end == @period")[year_cols].copy()
             period_str = period.strftime("%Y-%m-%d")
             if period == self._last_period and self._last_period_type == "quarterly":
-                period_str += " (ttm)"
+                period_str += " ltm"
             df_year.rename(columns={"acc_value": period_str}, inplace=True)
             dfo = pd.merge(dfo, df_year, how="left", on=["acc_code"])
         dfo.fillna(0, inplace=True)
         return dfo.sort_values("acc_code", ignore_index=True)
 
     def report(
         self,
-        report_type: str,
-        acc_level: int = 0,
+        report_type: Literal[
+            "balance_sheet",
+            "assets",
+            "cash",
+            "current_assets",
+            "non_current_assets",
+            "liabilities",
+            "debt",
+            "current_liabilities",
+            "non_current_liabilities",
+            "liabilities_and_equity",
+            "equity",
+            "income_statement",
+            "comprehensive_income",
+            "cash_flow",
+            "added_value",
+            "earnings_per_share",
+        ],
+        acc_level: Literal[0, 1, 2, 3, 4] = 0,
         num_years: int = 0,
     ) -> pd.DataFrame:
         """Generate an accounting report for the company.
 
         This function generates a report representing one of the financial
         statements for the company adjusted by the attributes passed.
 
@@ -424,81 +447,41 @@
             5 -> Changes in Equity
             6 -> Cash Flow (Indirect Method)
             7 -> Added Value
             8 -> Earnings per Share
         """
         report_types = {
             "balance_sheet": ("1", "2"),
-            "income_statement": ("3"),
-            "cash_flow": ("6"),
             "assets": ("1"),
             "cash": ("1.01.01", "1.01.02"),
             "current_assets": ("1.01"),
             "non_current_assets": ("1.02"),
             "liabilities": ("2.01", "2.02"),
             "debt": ("2.01.04", "2.02.01"),
             "current_liabilities": ("2.01"),
             "non_current_liabilities": ("2.02"),
             "liabilities_and_equity": ("2"),
             "equity": ("2.03"),
+            "income_statement": ("3"),
             "comprehensive_income": ("4"),
+            "cash_flow": ("6"),
             "added_value": ("7"),
             "earnings_per_share": ("8"),
         }
         acc_codes = report_types[report_type]  # noqa
         df.query("acc_code.str.startswith(@acc_codes)", inplace=True)
         df.reset_index(drop=True, inplace=True)
 
-        if (
-            report_type in ["income_statement", "cash_flow"]
-            and self._last_period_type == "quarterly"
-        ):
-            df = self._calculate_ttm(df)
-
         # Show only selected years
         all_periods = sorted(df["period_end"].drop_duplicates())
         selected_periods = all_periods[-num_years:]  # noqa
         df.query("period_end in @selected_periods", inplace=True)
 
         return self._build_report(df)
 
-    def _calculate_ttm(self, dfi: pd.DataFrame) -> pd.DataFrame:
-        """Calculate trailing twelve months (TTM) for income statement and cash
-        when quarterly data is the most recent available. If the function was
-        called, the last period is quarterly"""
-
-        # Quarterly dataframe
-        dfq = dfi.query("not is_annual").copy()
-        ttm_period_begin = dfq["period_end"].min()
-
-        # Last quarter in quarterly dataframe
-        df1 = dfq.query("period_end == period_end.max()").copy()
-
-        # Previous quarter in quarterly dataframe
-        df2 = dfq.query("period_end == period_end.min()").copy()
-        df2["acc_value"] = -df2["acc_value"]
-
-        # Last annual report
-        dfa = dfi.query("is_annual and period_end == @self._last_annual").copy()
-
-        # Construct TTM dataframe
-        df_ttm = (
-            pd.concat([df1, df2, dfa], ignore_index=True)[["acc_code", "acc_value"]]
-            .groupby(by="acc_code")
-            .sum()
-            .reset_index()
-        )
-        df1.drop(columns="acc_value", inplace=True)
-        df_ttm = pd.merge(df1, df_ttm)
-        df_ttm["period_begin"] = ttm_period_begin
-
-        df_annual = dfi.query("is_annual").copy()
-
-        return pd.concat([df_annual, df_ttm], ignore_index=True)
-
     def custom_report(
         self,
         acc_list: list[str],
         num_years: int = 0,
     ) -> pd.DataFrame:
         """Generate a financial report from custom list of accounting codes
```

### Comparing `finlogic-0.5.0/finlogic/cvm.py` & `finlogic-0.5.1/finlogic/cvm.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,20 +8,14 @@
 import numpy as np
 import requests
 from . import config as cfg
 
 URL_DFP = "https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/"
 URL_ITR = "https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/"
 
-CVM_RAW_DIR = cfg.DATA_PATH / "cvm" / "raw"
-CVM_PROCESSED_DIR = cfg.DATA_PATH / "cvm" / "processed"
-# Create CVM folders if they do not exist
-Path.mkdir(CVM_RAW_DIR, parents=True, exist_ok=True)
-Path.mkdir(CVM_PROCESSED_DIR, parents=True, exist_ok=True)
-
 
 def get_file_urls(cvm_url) -> List[str]:
     """Return a list of available CVM files.
 
     Urls with CVM raw files:
     https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/
     https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/
@@ -52,15 +46,15 @@
     urls = urls_dfp + urls_itr
     return urls
 
 
 def update_raw_file(url: str, s: requests.Session) -> Path:
     """Update raw file from CVM portal. Return a Path if file is updated."""
     filename = url[-23:]  # filename = end of url
-    filepath = CVM_RAW_DIR / filename
+    filepath = cfg.CVM_RAW_DIR / filename
     headers = s.head(url).headers
     filesize = filepath.stat().st_size if filepath.exists() else 0
     if filesize == int(headers["Content-Length"]):
         # file is already updated
         return None
     r = s.get(url)
     if r.status_code != 200:
@@ -169,18 +163,14 @@
     # Remove any extra spaces (line breaks, tabs, etc.) from columns below.
     columns = ["name_id", "acc_name"]
     df[columns] = df[columns].apply(remove_empty_spaces)
 
     # Replace "BCO " with "BANCO " in "name_id" column.
     df["name_id"] = df["name_id"].str.replace("BCO ", "BANCO ")
 
-    # Convert string columns to categorical before mapping.
-    columns = df.select_dtypes(include="object").columns
-    df[columns] = df[columns].astype("category")
-
     # Convert datetime columns
     columns = ["period_reference", "period_begin", "period_end"]
     df[columns] = df[columns].apply(pd.to_datetime)
 
     # currency_unit values are ['MIL', 'UNIDADE']
     map_dic = {"UNIDADE": 1, "MIL": 1000}
     df["currency_unit"] = df["currency_unit"].map(map_dic).astype(int)
@@ -210,18 +200,14 @@
            "period_end" is 2020-12-31
         then "period_order" is "LAST".
 
         If "period_reference" is 2020-12-31
            "period_begin" is 2019-01-01
            "period_end" is 2019-12-31
         then "period_order" is "PREVIOUS".
-    Old code:
-        "period_order" values are: 'ÚLTIMO', 'PENÚLTIMO'
-        map_dic = {"ÚLTIMO": "LAST", "PENÚLTIMO": "PREVIOUS"}
-        df["period_order"] = df["period_order"].map(map_dic)
     """
     df = df.drop(columns=["period_order"])
 
     """
     df['report_group'].unique() result:
         'DF Consolidado - Balanço Patrimonial Ativo',
         'DF Consolidado - Balanço Patrimonial Passivo',
@@ -239,102 +225,48 @@
         'DF Individual - Demonstração do Resultado',
     Hence, with string position 3:6 we can make:
     if == 'Con' -> consolidated statement
     if == 'Ind' -> separate statement
     """
     map_dic = {"Con": True, "Ind": False}
     df.insert(4, "is_consolidated", df["report_group"].str[3:6].map(map_dic))
+
     # 'report_group' data can be inferred from 'acc_code'
     df.drop(columns=["report_group"], inplace=True)
 
+    # "report_type" will be used to fast filter the data. Otherwise, it would be
+    # necessary to use str.startswith() or str.contains() methods.
+    df.insert(5, "report_type", df["acc_code"].str[0])
+    df["report_type"] = df["report_type"].astype("uint8")
+
     # In "itr_cia_aberta_2022.zip", as an example, 2742 rows are duplicated.
     # Few of them have different values in "acc_value". Only one them will be kept.
     # REMOVE ALL VALUES OR MARK THESE ROWS AS ERRORS?
     cols = df.columns.tolist()
     cols.remove("acc_value")
     df.drop_duplicates(subset=cols, keep="last", inplace=True, ignore_index=True)
 
     return df
 
 
 def process_file(raw_filepath: Path) -> Path:
     """Read, process and save a CVM file."""
     df = read_raw_file(raw_filepath)
     df = process_df(df, raw_filepath)
-    processed_filepath = CVM_PROCESSED_DIR / (raw_filepath.stem + ".pickle")
+    processed_filepath = cfg.CVM_PROCESSED_DIR / (raw_filepath.stem + ".pickle")
     # save_processed_df(df, processed_filepath)
     df.to_pickle(processed_filepath, compression="zstd")
     return processed_filepath
 
 
 def process_files_with_progress(filepaths_to_process):
     """Process CVM files with a progress bar."""
     for filepath in tqdm(filepaths_to_process, desc="Processing..."):
         # print(f"    {CHECKMARK} {raw_filepath.name} processed.")
         process_file(filepath)
 
 
 def get_raw_file_mtimes() -> pd.DataFrame:
     """Return a Pandas DataFrame with file_source and file_mtime columns."""
-    filepaths = sorted(CVM_RAW_DIR.glob("*.zip"))
+    filepaths = sorted(cfg.CVM_RAW_DIR.glob("*.zip"))
     d_mtimes = {filepath.name: filepath.stat().st_mtime for filepath in filepaths}
     return pd.DataFrame(d_mtimes.items(), columns=["file_source", "file_mtime"])
-
-
-def read_all_processed_files() -> pd.DataFrame:
-    """Read all processed CVM files."""
-    # list filepaths in processed folder
-    filepaths = sorted(CVM_PROCESSED_DIR.glob("*.pickle"))
-    df = pd.concat([pd.read_pickle(f, compression="zstd") for f in filepaths])
-    columns = df.columns
-    cat_cols = [c for c in columns if df[c].dtype in ["object"]]
-    df[cat_cols] = df[cat_cols].astype("category")
-    return df
-
-
-def drop_not_last_entries(df: pd.DataFrame) -> pd.DataFrame:
-    """Drop duplicated accounting entries before building database
-
-    Because the report holds accounting entries for the year before, we can keep only
-    the most recent one in the database. By doing this, we guarantee
-    that there is only one valid accounting value in the database -> the last one
-    """
-    sort_cols = [
-        "cvm_id",
-        "is_consolidated",
-        "acc_code",
-        "period_reference",
-        "is_annual",
-        "period_begin",
-        "period_end",
-    ]
-    df.sort_values(by=sort_cols, ascending=True, inplace=True, ignore_index=True)
-
-    subset_cols = [
-        "cvm_id",
-        "is_consolidated",
-        "acc_code",
-        "period_begin",
-        "period_end",
-    ]
-    return df.drop_duplicates(subset=subset_cols, keep="last", ignore_index=True)
-
-
-def drop_unecessary_quarterly_entries(df: pd.DataFrame) -> pd.DataFrame:
-    """Keep the last QUARTERLY report for each company only when necessary."""
-    # Create a temporary column with the max. period_reference for each company
-    df["max_period"] = df.groupby("cvm_id")["period_reference"].transform("max")
-
-    mask1 = ~df["is_annual"]
-    mask2 = df["period_reference"] < df["max_period"]
-    mask = ~(mask1 & mask2)
-    return df[mask].reset_index(drop=True).drop(columns=["max_period"])
-
-
-def build_main_df():
-    """Build FinLogic Database from processed CVM files."""
-    df = read_all_processed_files()
-    df = drop_not_last_entries(df)
-    df = drop_unecessary_quarterly_entries(df)
-    # After the drop_unecessary entries, period_reference is not necessary anymore
-    df.drop(columns=["period_reference"], inplace=True)
-    df.to_pickle(cfg.DF_PATH, compression="zstd")
```

### Comparing `finlogic-0.5.0/finlogic/data_manager.py` & `finlogic-0.5.1/finlogic/data_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pathlib import Path
 from typing import Literal
 from datetime import datetime
 import pandas as pd
 from . import config as cfg
 from . import cvm
 from . import language as lng
+from . import builder as bld
 
 CHECKMARK = "\033[32m\u2714\033[0m"
 
 
 def get_main_df() -> pd.DataFrame:
     """Return a DataFrame with all accounting data"""
     if cfg.DF_PATH.is_file():
@@ -28,15 +29,15 @@
 
 def get_filepaths_to_process(df1: pd.DataFrame, df2: pd.DataFrame) -> list[Path]:
     """Return a list of CVM files that has to be processed by comparing
     the files mtimes from the raw folder.
     """
     df = pd.concat([df1, df2]).drop_duplicates(keep=False)
     file_sources = sorted(df["file_source"].drop_duplicates())
-    return [cvm.CVM_RAW_DIR / file_source for file_source in file_sources]
+    return [cfg.CVM_RAW_DIR / file_source for file_source in file_sources]
 
 
 def update(rebuild: bool = False):
     """Verify changes in CVM files and update Finlogic Database if necessary.
 
     Args:
         rebuild (bool, optional): If True, processes all CVM files and rebuilds
@@ -56,25 +57,25 @@
     print(f"Number of CVM files updated = {len(updated_raw_filepaths)}")
     # Get files mtimes from the raw folder after updating
     df_raw2 = cvm.get_raw_file_mtimes()
 
     # CVM processed files
     if rebuild:
         # Process all files
-        filepaths_to_process = sorted(cvm.CVM_RAW_DIR.glob("*.zip"))
+        filepaths_to_process = sorted(cfg.CVM_RAW_DIR.glob("*.zip"))
     else:
         # Process only updated files
         filepaths_to_process = get_filepaths_to_process(df1=df_raw1, df2=df_raw2)
     print(f"Number of new files to process = {len(filepaths_to_process)}")
 
     cvm.process_files_with_progress(filepaths_to_process)
 
     # FinLogic Database
     print("\nBuilding FinLogic main DataFrame...")
-    cvm.build_main_df()
+    bld.build_main_df()
     print(f"{CHECKMARK} FinLogic updated!")
 
 
 def info() -> pd.DataFrame:
     """Print a concise summary of FinLogic available data.
 
     This function returns a dataframe containing main information about
@@ -93,15 +94,15 @@
     df = get_main_df()
     if df.empty:
         return pd.DataFrame()
 
     info["data_path"] = f"{cfg.DATA_PATH}"
     info["data_size"] = f"{cfg.DF_PATH.stat().st_size / 1024**2:.1f} MB"
     db_last_modified = datetime.fromtimestamp(cfg.DF_PATH.stat().st_mtime)
-    info["last_modified_on"] = db_last_modified.strftime("%Y-%m-%d %H:%M:%S")
+    info["updated_on"] = db_last_modified.strftime("%Y-%m-%d %H:%M:%S")
 
     info["accounting_entries"] = df.shape[0]
 
     report_cols = ["cvm_id", "is_annual", "period_end"]
     info["number_of_reports"] = df[report_cols].drop_duplicates().shape[0]
     info["first_report"] = df["period_end"].min().strftime("%Y-%m-%d")
     info["last_report"] = df["period_end"].max().strftime("%Y-%m-%d")
```

### Comparing `finlogic-0.5.0/finlogic/language.py` & `finlogic-0.5.1/finlogic/language.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.5.0/pyproject.toml` & `finlogic-0.5.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 dependencies = [
     "pandas>=1.5.0",
     "requests>=2.30.0",
     "tqdm>=4.1.0",
     "zstandard>=0.21.0",
 ]
-version = "0.5.0"
+version = "0.5.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
```

### Comparing `finlogic-0.5.0/tests/test_company.py` & `finlogic-0.5.1/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.5.0/tests/test_data.py` & `finlogic-0.5.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.5.0/PKG-INFO` & `finlogic-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.5.0
+Version: 0.5.1
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -78,15 +78,15 @@
 
 ---
 
 ## Quick Start
 
 ### Create FinLogic Database
 
-The 'update' function is responsible for downloading and updating raw financial data from the CVM, processing approximately 20 million accounting entries, and storing them for local data analysis. During the initial run, the process might take longer than 1 minute, depending on the CVM server connection and local CPU power. For subsequent updates, only the updated CVM files will be downloaded and processed, which should expedite the operation.
+The 'update' function is responsible for downloading and updating raw financial data from the CVM, processing approximately 20 million accounting entries, and storing them for local data analysis. During the initial run, the process might take some minutes, depending on the CVM server connection and local CPU power. For subsequent updates, only the updated CVM files will be downloaded and processed, which should expedite the operation.
 
 ```python
 >>> import finlogic as fl
 
 # Compile FinLogic database for the first time:
 >>> fl.update()
 
@@ -94,24 +94,24 @@
 ...
 FinLogic database updated ✅
 
 # Show database info:
 >>> fl.info()
 ```
 
-| FinLogic Database Info |                         Value |
-| :--------------------- | ----------------------------: |
-| db_path                | .../finlogic/data/finlogic.db |
-| db_size                |                       76.0 MB |
-| db_last_modified       |           2023-04-20 07:29:08 |
-| number_of_companies    |                         1,139 |
-| number_of_rows         |                     2,806,635 |
-| number_of_reports      |                         9,422 |
-| first_report           |                    2009-01-31 |
-| last_report            |                    2023-03-31 |
+|                     |       FinLogic Info |
+| :------------------ | ------------------: |
+| data_path           |   .../finlogic/data |
+| data_size           |             12.1 MB |
+| last_modified_on    | 2023-04-20 07:29:08 |
+| accounting_entries  |           2,806,635 |
+| number_of_reports   |              11,635 |
+| first_report        |          2009-01-31 |
+| last_report         |          2023-03-31 |
+| number_of_companies |               1,139 |
 
 ```python
 # Search for a company in database:
 >>> fl.search_company('petro')
 ```
 
 |     | name_id                                | cvm_id | tax_id             |
@@ -128,38 +128,38 @@
 ### The Company Class
 
 The Company Class allows you to easily access financial data from Brazilian companies. All values are in local currency (Real).
 
 ```python
 # Create a Company object to acces its financial data:
 # Both CVM (regulator) ID or Fiscal ID can be used as an identifier.
->>> petro = fl.Company(9512, is_consolidated='sep', acc_unit='m')
+>>> petro = fl.Company(9512, is_consolidated=False, acc_unit='m')
 
 # Change company accounting method back to consolidated (default):
->>> petro.is_consolidated = 'con'
+>>> petro.is_consolidated = True
 
 # Change company accounting unit to billion (default is 1):
 >>> petro.acc_unit = 'b'
 
 # Show company info:
 >>> petro.info()
 ```
 
-| Company Info               |                             Values |
+|                            |                       Company Info |
 | :------------------------- | ---------------------------------: |
 | Name                       | PETROLEO BRASILEIRO S.A. PETROBRAS |
 | CVM ID                     |                               9512 |
-| Fiscal ID (CNPJ)           |                 33.000.167/0001-01 |
-| Total Accounting Rows      |                             39,292 |
+| Tax ID (CNPJ)              |                 33.000.167/0001-01 |
+| Total Accounting Rows      |                              3,292 |
 | Selected Tax Rate          |                               0.34 |
 | Selected Accounting Method |                       consolidated |
 | Selected Accounting Unit   |                      1,000,000,000 |
-| First Annual Report        |                         2009-12-31 |
-| Last Annual Report         |                         2021-12-31 |
-| Last Quarterly Report      |                         2021-09-30 |
+| First Report               |                         2009-12-31 |
+| Last Report                |                         2021-12-31 |
+| Last Report Type           |                          quarterly |
 
 ```python
 # Show company assets in Brazilian currency:
 >>> petro.report(report_type='assets')
 ...
 # Show company liabilities with custom arguments:
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
```

