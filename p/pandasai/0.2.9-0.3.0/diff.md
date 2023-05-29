# Comparing `tmp/pandasai-0.2.9.tar.gz` & `tmp/pandasai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.2.9.tar", max compression
+gzip compressed data, was "pandasai-0.3.0.tar", max compression
```

## Comparing `pandasai-0.2.9.tar` & `pandasai-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,28 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.9/LICENSE
--rw-r--r--   0        0        0     5641 2023-05-07 22:56:45.170152 pandasai-0.2.9/README.md
--rw-r--r--   0        0        0     9012 2023-05-08 23:43:04.960305 pandasai-0.2.9/pandasai/__init__.py
--rw-r--r--   0        0        0     1025 2023-05-08 23:41:52.704456 pandasai-0.2.9/pandasai/constants.py
--rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.9/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.9/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     4646 2023-05-06 22:56:45.185822 pandasai-0.2.9/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.9/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.9/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1493 2023-05-07 12:19:23.603585 pandasai-0.2.9/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     3020 2023-05-08 23:41:52.704520 pandasai-0.2.9/pandasai/llm/base.py
--rw-r--r--   0        0        0     1409 2023-05-07 12:19:27.955602 pandasai-0.2.9/pandasai/llm/base_hf.py
--rw-r--r--   0        0        0      505 2023-05-08 23:08:22.612651 pandasai-0.2.9/pandasai/llm/fake.py
--rw-r--r--   0        0        0      763 2023-05-08 23:40:05.209518 pandasai-0.2.9/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3859 2023-05-08 23:40:53.213540 pandasai-0.2.9/pandasai/llm/openai.py
--rw-r--r--   0        0        0      697 2023-05-08 23:39:55.732086 pandasai-0.2.9/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0      862 2023-05-08 23:49:50.082167 pandasai-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     6493 1970-01-01 00:00:00.000000 pandasai-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8330 2023-05-29 12:51:07.868554 pandasai-0.3.0/README.md
+-rw-r--r--   0        0        0    16080 2023-05-29 12:51:07.872906 pandasai-0.3.0/pandasai/__init__.py
+-rw-r--r--   0        0        0     1122 2023-05-29 12:51:07.873140 pandasai-0.3.0/pandasai/constants.py
+-rw-r--r--   0        0        0      950 2023-05-29 12:51:07.873695 pandasai-0.3.0/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.3.0/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-29 12:51:07.874366 pandasai-0.3.0/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0      568 2023-05-29 12:51:07.875099 pandasai-0.3.0/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1487 2023-05-29 12:51:07.875283 pandasai-0.3.0/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     2643 2023-05-29 12:51:07.875419 pandasai-0.3.0/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.3.0/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1493 2023-05-07 12:19:23.603585 pandasai-0.3.0/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     4325 2023-05-29 12:51:07.876227 pandasai-0.3.0/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10840 2023-05-29 12:51:07.876513 pandasai-0.3.0/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-05-27 07:25:53.172948 pandasai-0.3.0/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1838 2023-05-29 12:51:07.877290 pandasai-0.3.0/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1481 2023-05-29 12:51:07.878110 pandasai-0.3.0/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2869 2023-05-29 12:51:07.878277 pandasai-0.3.0/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-05-29 12:51:07.878427 pandasai-0.3.0/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:51:07.878463 pandasai-0.3.0/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      734 2023-05-29 12:51:07.878751 pandasai-0.3.0/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1786 2023-05-29 12:51:07.878903 pandasai-0.3.0/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1333 2023-05-29 12:51:07.879011 pandasai-0.3.0/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1603 2023-05-29 12:51:07.879149 pandasai-0.3.0/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      505 2023-05-29 12:51:07.879285 pandasai-0.3.0/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1414 2023-05-29 12:51:07.879389 pandasai-0.3.0/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1162 2023-05-29 12:51:26.381317 pandasai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9237 1970-01-01 00:00:00.000000 pandasai-0.3.0/PKG-INFO
```

### Comparing `pandasai-0.2.9/LICENSE` & `pandasai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.9/README.md` & `pandasai-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # PandasAI 🐼
 
-[![release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
-[![lint](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
+[![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
+[![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
+[![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/pandas-ai/badge/?version=latest)](https://pandas-ai.readthedocs.io/en/latest/?badge=latest)
 [![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
 [![Downloads](https://static.pepy.tech/badge/pandasai/month)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
 Pandas AI is a Python library that adds generative artificial intelligence capabilities to Pandas, the popular data analysis and manipulation tool. It is designed to be used in conjunction with Pandas, and is not a replacement for it.
 
 <!-- Add images/pandas-ai.png -->
@@ -14,43 +16,51 @@
 
 ## Demo
 
 Try out PandasAI in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
+## Documentation
+
+The documentation for PandasAI can be found [here](https://pandas-ai.readthedocs.io/en/latest/).
+
 ## Installation
 
 ```bash
 pip install pandasai
 ```
 
 ## Usage
 
 > Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
 
-PandasAI is designed to be used in conjunction with Pandas. It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of Pandas DataFrames. For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
+PandasAI is designed to be used in conjunction with [pandas](https://github.com/pandas-dev/pandas). It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of pandas DataFrames. 
+
+### Queries
+
+For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
 from pandasai import PandasAI
 
 # Sample DataFrame
 df = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
 # Instantiate a LLM
 from pandasai.llm.openai import OpenAI
-llm = OpenAI()
+llm = OpenAI(api_token="YOUR_API_TOKEN")
 
-pandas_ai = PandasAI(llm)
-pandas_ai.run(df, prompt='Which are the 5 happiest countries?')
+pandas_ai = PandasAI(llm, conversational=False)
+pandas_ai(df, prompt='Which are the 5 happiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 6            Canada
 7         Australia
@@ -59,57 +69,125 @@
 0     United States
 Name: country, dtype: object
 ```
 
 Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
 
 ```python
-pandas_ai.run(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
+pandas_ai(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 19012600725504
 ```
 
+### Charts
+
 You can also ask PandasAI to draw a graph:
 
 ```python
-pandas_ai.run(
+pandas_ai(
     df,
-    "Plot the histogram of countries showing for each the gpd, using different colors for each bar",
+    "Plot the histogram of countries showing for each the gdp, using different colors for each bar",
 )
 ```
 
 ![Chart](images/histogram-chart.png?raw=true)
 
+You can save any charts generated by PandasAI by setting the `save_charts` parameter to `True` in the `PandasAI` constructor. For example, `PandasAI(llm, save_charts=True)`. Charts are saved in `./pandasai/exports/charts` .
+
+### Multiple DataFrames
+
+Additionally, you can also pass in multiple dataframes to PandasAI and ask questions relating them.
+
+```python
+import pandas as pd
+from pandasai import PandasAI
+
+employees_data = {
+    'EmployeeID': [1, 2, 3, 4, 5],
+    'Name': ['John', 'Emma', 'Liam', 'Olivia', 'William'],
+    'Department': ['HR', 'Sales', 'IT', 'Marketing', 'Finance']
+}
+
+salaries_data = {
+    'EmployeeID': [1, 2, 3, 4, 5],
+    'Salary': [5000, 6000, 4500, 7000, 5500]
+}
+
+employees_df = pd.DataFrame(employees_data)
+salaries_df = pd.DataFrame(salaries_data)
+
+
+llm = OpenAI()
+pandas_ai = PandasAI(llm)
+pandas_ai([employees_df, salaries_df], "Who gets paid the most?")
+```
+
+The above code will return the following:
+
+```
+Oh, Olivia gets paid the most.
+```
+
 You can find more examples in the [examples](examples) directory.
 
+## Command-Line Tool
+
+Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI).
+
+```
+pai [OPTIONS]
+```
+
+Options:
+
+- **-d, --dataset**: The file path to the dataset.
+- **-t, --token**: Your HuggingFace or OpenAI API token, if no token provided pai will pull from the `.env` file.
+- **-m, --model**: Choice of LLM, either `openai`, `open-assistant`, `starcoder`, or Google `palm`.
+- **-p, --prompt**: Prompt that PandasAI will run.
+
+To view a full list of available options and their descriptions, run the following command:
+
+```
+pai --help
+
+```
+
+> For example,
+>
+> ```
+> pai -d "~/pandasai/example/data/Loan payments data.csv" -m "openai" -p "How many loans are from men and have been paid off?"
+> ```
+>
+> Should result in the same output as the `from_csv.py` example.
+
 ## Privacy & Security
+
 In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
 
 Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
 
-
 ## Environment Variables
 
 In order to set the API key for the LLM (Hugging Face Hub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
 
 ```bash
 cp .env.example .env
 ```
 
 Then, edit the `.env` file and set the appropriate values.
 
 As an alternative, you can also pass the environment variables directly to the constructor of the LLM:
 
 ```python
 # OpenAI
-llm = OpenAI(api_token="YOUR_OPENAI_API_KEY")
+llm = OpenAI(api_token="YOUR_API_KEY")
 
 # Starcoder
 llm = Starcoder(api_token="YOUR_HF_API_KEY")
 ```
 
 ## License
 
@@ -122,16 +200,21 @@
 
 After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
 
 ```bash
 pre-commit install
 ```
 
+## Acknowledgements
+
+- This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
+- This project is meant to be used as a tool for data exploration and analysis, and it's not meant to be used for production purposes. Please use it responsibly.
+
 ### Todo
 
 - [ ] Add support for more LLMs
-- [ ] Make PandasAI available from a CLI
+- [x] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
 - [ ] Add unit tests
 - [x] Add contributing guidelines
 - [x] Add CI
 - [x] Add support for conversational responses
```

### Comparing `pandasai-0.2.9/pandasai/constants.py` & `pandasai-0.3.0/pandasai/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """
 Constants used in the pandasai package.
+
+It includes Start & End Code tags, Whitelisted Python Packages and While List Builtin Methods.
+
 """
 
 START_CODE_TAG = "<startCode>"
 END_CODE_TAG = "<endCode>"
 WHITELISTED_LIBRARIES = [
     "numpy",
     "matplotlib",
```

### Comparing `pandasai-0.2.9/pandasai/exceptions.py` & `pandasai-0.3.0/pandasai/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-"""PandasAI's custom exceptions."""
+"""PandasAI's custom exceptions.
+
+This module contains the implementation of Custom Exceptions.
+
+"""
 
 
 class APIKeyNotFoundError(Exception):
+
     """
     Raised when the API key is not defined/declared.
 
     Args:
         Exception (Exception): APIKeyNotFoundError
     """
```

### Comparing `pandasai-0.2.9/pandasai/helpers/anonymizer.py` & `pandasai-0.3.0/pandasai/helpers/anonymizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,69 @@
 """
 This module contains helper functions for anonymizing data and generating random data
-before sending it to the LLM.
+before sending it to the LLM (An External API). Only df.head() is sent to LLM API,
+ hence the df.head() is processed to remove any personal or sensitive information.
+
 """
 
 import random
 import re
 import string
-
 import pandas as pd
 
 
 def is_valid_email(email: str) -> bool:
-    """
-    Check if the given email is valid based on regex pattern.
 
-    :param email: str, email address to be checked
-    :return: bool, True if the email is valid, otherwise False
+    """Check if the given email is valid based on regex pattern.
+
+    Args:
+        email (str): email address to be checked.
+
+    Returns (bool): True if the email is valid, otherwise False.
     """
+
     email_regex = r"^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$"
     return re.match(email_regex, email) is not None
 
 
 def is_valid_phone_number(phone_number: str) -> bool:
-    """
-    Check if the given phone number is valid based on regex pattern.
 
-    :param phone_number: str, phone number to be checked
-    :return: bool, True if the phone number is valid, otherwise False
+    """Check if the given phone number is valid based on regex pattern.
+
+    Args:
+        phone_number (str): phone number to be checked.
+
+    Returns (bool): True if the phone number is valid, otherwise False.
     """
+
     pattern = r"\b(?:\+?\d{1,3}[- ]?)?\(?\d{3}\)?[- ]?\d{3}[- ]?\d{4}\b"
     return re.search(pattern, phone_number) is not None
 
 
 def is_valid_credit_card(credit_card_number: str) -> bool:
-    """
-    Check if the given credit card number is valid based on regex pattern.
 
-    :param credit_card_number: str, credit card number to be checked
-    :return: bool, True if the credit card number is valid, otherwise False
+    """Check if the given credit card number is valid based on regex pattern.
+
+    Args:
+        credit_card_number (str): credit card number to be checked.
+
+    Returns (str): True if the credit card number is valid, otherwise False.
     """
+
     pattern = r"^\d{4}[- ]?\d{4}[- ]?\d{4}[- ]?\d{4}$"
     return re.search(pattern, credit_card_number) is not None
 
 
 def generate_random_email() -> str:
-    """
-    Generate a random email address using predefined domains.
 
-    :return: str, generated random email address
+    """Generates a random email address using predefined domains.
+
+    Returns (str): generated random email address.
     """
+
     domains = [
         "gmail.com",
         "yahoo.com",
         "hotmail.com",
         "outlook.com",
         "icloud.com",
         "aol.com",
@@ -64,20 +75,23 @@
     letters = string.ascii_lowercase + string.digits + "-_"
     username = "".join(random.choice(letters) for i in range(name_length))
     email = username + "@" + domain
     return email
 
 
 def generate_random_phone_number(original_field: str) -> str:
-    """
-    Generate a random phone number with country code if originally present.
 
-    :param original_field: str, original phone number field
-    :return: str, generated random phone number
+    """Generate a random phone number with country code if originally present.
+
+    Args:
+        original_field (str): original phone number field.
+
+    Returns (str): generated random phone number.
     """
+
     if original_field.startswith("+"):
         # Extract country code if present
         country_code = original_field.split()[0]
     else:
         country_code = ""
 
     number = "".join(random.choices("0123456789", k=10))
@@ -87,47 +101,64 @@
     else:
         phone_number = number
 
     return phone_number
 
 
 def generate_random_credit_card() -> str:
-    """
-    Generate a random credit card number.
 
-    :return: str, generated random credit card number
+    """Generate a random credit card number.
+
+    Returns (str): generated random credit card number.
     """
+
     groups = []
     for _i in range(4):
         group = "".join(random.choices("0123456789", k=4))
         groups.append(group)
     separator = random.choice(["-", " "])
     return separator.join(groups)
 
 
 def copy_head(data_frame: pd.DataFrame) -> pd.DataFrame:
-    """
-    Copy the head of a DataFrame.
 
-    :param data_frame: pd.DataFrame, the DataFrame to copy the head from
-    :return: pd.DataFrame, copied head of the DataFrame
+    """Copy the head of a DataFrame.
+
+    Args:
+        data_frame (pd.DataFrame): The pd.DataFrame to copy the head from.
+
+    Returns (pd.DataFrame): copied head of the DataFrame.
     """
+
     return data_frame.head().copy()
 
 
-def anonymize_dataframe_head(data_frame: pd.DataFrame) -> pd.DataFrame:
-    """
-    Anonymize the head of a given DataFrame by replacing sensitive data.
+def anonymize_dataframe_head(
+    data_frame: pd.DataFrame, force_conversion: bool = True
+) -> pd.DataFrame:
 
-    :param data_frame: pd.DataFrame, the DataFrame to anonymize the head
-    :return: pd.DataFrame, anonymized head of the DataFrame
+    """Anonymize the head of a given DataFrame by replacing sensitive data.
+
+    Args:
+
+        data_frame (pd.DataFrame):  The DataFrame to anonymize the head data.
+        force_conversion (bool): Convert it with instruction. Default is True.
+
+    Returns: Anonymized head of the DataFrame.
     """
+
     data_frame = copy_head(data_frame)
+    dtypes = data_frame.dtypes
     for col in data_frame.columns:
         col_idx = data_frame.columns.get_loc(col)
+        # check category type column and temporarily convert to object type
+        if force_conversion:
+            if pd.api.types.is_categorical_dtype(data_frame[col]):
+                if data_frame[col].isna().any():
+                    data_frame[col] = data_frame[col].astype(object)
         for row_idx, val in enumerate(data_frame[col]):
             cell_value = str(val)
 
             if is_valid_email(cell_value):
                 data_frame.iloc[row_idx, col_idx] = generate_random_email()
                 continue
             if is_valid_phone_number(cell_value):
@@ -142,8 +173,10 @@
             # anonymize data
             random_row_index = random.choice(
                 [i for i in range(len(data_frame.index)) if i != row_idx]
             )
             random_value = data_frame.iloc[random_row_index, col_idx]
             data_frame.iloc[row_idx, col_idx] = random_value
             data_frame.iloc[random_row_index, col_idx] = cell_value
+    # restore the original data types
+    data_frame = data_frame.astype(dtypes)
     return data_frame
```

### Comparing `pandasai-0.2.9/pandasai/helpers/notebook.py` & `pandasai-0.3.0/pandasai/helpers/notebook.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-""" Notebook helper functions """
+""" Helper Module to Handle Jupyter Notebook
+This module contains helper functions to interact with Jupyter Notebook Functionalities.
+
+"""
 
 from IPython import get_ipython
 
 
 class Notebook:
 
     """Baseclass to implement Notebook helper functions"""
 
     def in_notebook(self) -> bool:
+
         """
         Checks whether the code is running inside a notebook environment.
 
-        Returns:
-            bool: True if the code is running inside a Jupyter notebook, False otherwise.
+        Returns (bool): True if the code is running inside a Jupyter notebook, False otherwise.
         """
         try:
             if "IPKernelApp" not in get_ipython().config:
                 return False
-        except ImportError:
-            return False
-        except AttributeError:
+        except (ImportError, AttributeError):
             return False
         return True
 
     def create_new_cell(self, contents: str) -> None:
+
         """
         Creates a new code cell in the Jupyter notebook and populates it with the specified
         contents.
+        Args:
+            contents (str): The contents to be added to the new code cell.
 
-        Parameters:
-        -----------
-        contents : str
-            The contents to be added to the new code cell.
-
-        Raises:
-        -------
         ImportError:
             If the IPython module is not installed.
 
         AttributeError:
             If the 'get_ipython()' call raises an AttributeError, which can happen if the code is
             not running inside a Jupyter notebook.
 
-        Returns:
-            None
+        Returns: None
+
         """
+
         payload = {"source": "set_next_input", "text": contents, "replace": False}
         try:
             get_ipython().payload_manager.write_payload(payload, single=False)
         except (ImportError, AttributeError) as exception:
             raise exception
```

### Comparing `pandasai-0.2.9/pandasai/llm/alpaca.py` & `pandasai-0.3.0/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.9/pyproject.toml` & `pandasai-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.2.9"
+version = "0.3.0"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 pandas = "^2.0.1"
 astor = "^0.8.1"
 openai = "^0.27.5"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
-pytest-env = "^0.8.1"
+google-generativeai = { version = "^0.1.0rc2", optional = true }
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 pylint = "^2.17.3"
 pytest = "^7.3.1"
 isort = "^5.12.0"
 pytest-mock = "^3.10.0"
+pytest-env = "^0.8.1"
+click = "^8.1.3"
+
+[tool.poetry.extras]
+google = ["google-generativeai"]
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "1.4.0"
+mkdocstrings-python = "0.7.1"
+markdown-include = "^0.6.0"
+
+[tool.poetry.scripts]
+pai = "pai.__main__:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pylint]
 ignore = "tests_*"
```

### Comparing `pandasai-0.2.9/PKG-INFO` & `pandasai-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.2.9
+Version: 0.3.0
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: google
 Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: pytest-env (>=0.8.1,<0.9.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PandasAI 🐼
 
-[![release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
-[![lint](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
+[![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
+[![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
+[![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/pandas-ai/badge/?version=latest)](https://pandas-ai.readthedocs.io/en/latest/?badge=latest)
 [![](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
 [![Downloads](https://static.pepy.tech/badge/pandasai/month)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
 Pandas AI is a Python library that adds generative artificial intelligence capabilities to Pandas, the popular data analysis and manipulation tool. It is designed to be used in conjunction with Pandas, and is not a replacement for it.
 
 <!-- Add images/pandas-ai.png -->
@@ -35,43 +38,51 @@
 
 ## Demo
 
 Try out PandasAI in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1rKz7TudOeCeKGHekw7JFNL4sagN9hon-?usp=sharing)
 
+## Documentation
+
+The documentation for PandasAI can be found [here](https://pandas-ai.readthedocs.io/en/latest/).
+
 ## Installation
 
 ```bash
 pip install pandasai
 ```
 
 ## Usage
 
 > Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
 
-PandasAI is designed to be used in conjunction with Pandas. It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of Pandas DataFrames. For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
+PandasAI is designed to be used in conjunction with [pandas](https://github.com/pandas-dev/pandas). It makes Pandas conversational, allowing you to ask questions about your data and get answers back, in the form of pandas DataFrames. 
+
+### Queries
+
+For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
 
 ```python
 import pandas as pd
 from pandasai import PandasAI
 
 # Sample DataFrame
 df = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
     "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
     "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
 })
 
 # Instantiate a LLM
 from pandasai.llm.openai import OpenAI
-llm = OpenAI()
+llm = OpenAI(api_token="YOUR_API_TOKEN")
 
-pandas_ai = PandasAI(llm)
-pandas_ai.run(df, prompt='Which are the 5 happiest countries?')
+pandas_ai = PandasAI(llm, conversational=False)
+pandas_ai(df, prompt='Which are the 5 happiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 6            Canada
 7         Australia
@@ -80,57 +91,125 @@
 0     United States
 Name: country, dtype: object
 ```
 
 Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
 
 ```python
-pandas_ai.run(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
+pandas_ai(df, prompt='What is the sum of the GDPs of the 2 unhappiest countries?')
 ```
 
 The above code will return the following:
 
 ```
 19012600725504
 ```
 
+### Charts
+
 You can also ask PandasAI to draw a graph:
 
 ```python
-pandas_ai.run(
+pandas_ai(
     df,
-    "Plot the histogram of countries showing for each the gpd, using different colors for each bar",
+    "Plot the histogram of countries showing for each the gdp, using different colors for each bar",
 )
 ```
 
 ![Chart](images/histogram-chart.png?raw=true)
 
+You can save any charts generated by PandasAI by setting the `save_charts` parameter to `True` in the `PandasAI` constructor. For example, `PandasAI(llm, save_charts=True)`. Charts are saved in `./pandasai/exports/charts` .
+
+### Multiple DataFrames
+
+Additionally, you can also pass in multiple dataframes to PandasAI and ask questions relating them.
+
+```python
+import pandas as pd
+from pandasai import PandasAI
+
+employees_data = {
+    'EmployeeID': [1, 2, 3, 4, 5],
+    'Name': ['John', 'Emma', 'Liam', 'Olivia', 'William'],
+    'Department': ['HR', 'Sales', 'IT', 'Marketing', 'Finance']
+}
+
+salaries_data = {
+    'EmployeeID': [1, 2, 3, 4, 5],
+    'Salary': [5000, 6000, 4500, 7000, 5500]
+}
+
+employees_df = pd.DataFrame(employees_data)
+salaries_df = pd.DataFrame(salaries_data)
+
+
+llm = OpenAI()
+pandas_ai = PandasAI(llm)
+pandas_ai([employees_df, salaries_df], "Who gets paid the most?")
+```
+
+The above code will return the following:
+
+```
+Oh, Olivia gets paid the most.
+```
+
 You can find more examples in the [examples](examples) directory.
 
+## Command-Line Tool
+
+Pai is the command line tool designed to provide a convenient way to interact with PandasAI through a command line interface (CLI).
+
+```
+pai [OPTIONS]
+```
+
+Options:
+
+- **-d, --dataset**: The file path to the dataset.
+- **-t, --token**: Your HuggingFace or OpenAI API token, if no token provided pai will pull from the `.env` file.
+- **-m, --model**: Choice of LLM, either `openai`, `open-assistant`, `starcoder`, or Google `palm`.
+- **-p, --prompt**: Prompt that PandasAI will run.
+
+To view a full list of available options and their descriptions, run the following command:
+
+```
+pai --help
+
+```
+
+> For example,
+>
+> ```
+> pai -d "~/pandasai/example/data/Loan payments data.csv" -m "openai" -p "How many loans are from men and have been paid off?"
+> ```
+>
+> Should result in the same output as the `from_csv.py` example.
+
 ## Privacy & Security
+
 In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
 
 Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
 
-
 ## Environment Variables
 
 In order to set the API key for the LLM (Hugging Face Hub, OpenAI), you need to set the appropriate environment variables. You can do this by copying the `.env.example` file to `.env`:
 
 ```bash
 cp .env.example .env
 ```
 
 Then, edit the `.env` file and set the appropriate values.
 
 As an alternative, you can also pass the environment variables directly to the constructor of the LLM:
 
 ```python
 # OpenAI
-llm = OpenAI(api_token="YOUR_OPENAI_API_KEY")
+llm = OpenAI(api_token="YOUR_API_KEY")
 
 # Starcoder
 llm = Starcoder(api_token="YOUR_HF_API_KEY")
 ```
 
 ## License
 
@@ -143,17 +222,22 @@
 
 After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
 
 ```bash
 pre-commit install
 ```
 
+## Acknowledgements
+
+- This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
+- This project is meant to be used as a tool for data exploration and analysis, and it's not meant to be used for production purposes. Please use it responsibly.
+
 ### Todo
 
 - [ ] Add support for more LLMs
-- [ ] Make PandasAI available from a CLI
+- [x] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
 - [ ] Add unit tests
 - [x] Add contributing guidelines
 - [x] Add CI
 - [x] Add support for conversational responses
```

