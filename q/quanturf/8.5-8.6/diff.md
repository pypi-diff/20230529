# Comparing `tmp/quanturf-8.5.tar.gz` & `tmp/quanturf-8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanturf-8.5.tar", last modified: Mon Mar 20 17:41:58 2023, max compression
+gzip compressed data, was "quanturf-8.6.tar", last modified: Mon May 29 13:34:46 2023, max compression
```

## Comparing `quanturf-8.5.tar` & `quanturf-8.6.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 17:41:58.161171 quanturf-8.5/
--rw-rw-rw-   0        0        0      782 2023-03-20 17:41:58.153165 quanturf-8.5/PKG-INFO
--rw-rw-rw-   0        0        0     6809 2022-10-19 16:34:20.000000 quanturf-8.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 17:41:58.021163 quanturf-8.5/quanturf/
--rw-rw-rw-   0        0        0        0 2022-10-19 16:34:20.000000 quanturf-8.5/quanturf/__init__.py
--rw-rw-rw-   0        0        0     4817 2023-03-20 17:31:37.000000 quanturf-8.5/quanturf/__main__.py
--rw-rw-rw-   0        0        0    30506 2022-10-19 16:34:20.000000 quanturf-8.5/quanturf/jupyter_notebook_config.py
--rw-rw-rw-   0        0        0    50342 2023-01-19 11:35:30.000000 quanturf-8.5/quanturf/quanturf_logo.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:41:58.150162 quanturf-8.5/quanturf.egg-info/
--rw-rw-rw-   0        0        0      782 2023-03-20 17:41:57.000000 quanturf-8.5/quanturf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-03-20 17:41:57.000000 quanturf-8.5/quanturf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 17:41:57.000000 quanturf-8.5/quanturf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-03-20 17:41:57.000000 quanturf-8.5/quanturf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-03-20 17:41:57.000000 quanturf-8.5/quanturf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-20 17:41:57.000000 quanturf-8.5/quanturf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 17:41:58.162171 quanturf-8.5/setup.cfg
--rw-rw-rw-   0        0        0     2327 2023-03-20 17:40:46.000000 quanturf-8.5/setup.py
--rw-rw-rw-   0        0        0      342 2022-10-19 16:34:20.000000 quanturf-8.5/version.py
+drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-05-29 13:34:46.816784 quanturf-8.6/
+-rw-r--r--   0 aayush    (1000) aayush    (1000)    35149 2023-05-29 13:06:01.000000 quanturf-8.6/LICENCE.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      778 2023-05-29 13:34:46.816784 quanturf-8.6/PKG-INFO
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     6705 2023-05-29 13:06:01.000000 quanturf-8.6/README.md
+drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-05-29 13:34:46.816784 quanturf-8.6/quanturf/
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     4437 2023-05-29 13:06:01.000000 quanturf-8.6/quanturf/MACD.ipynb
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     3025 2023-05-29 13:06:01.000000 quanturf-8.6/quanturf/RSI.ipynb
+-rw-r--r--   0 aayush    (1000) aayush    (1000)        0 2023-05-29 13:06:01.000000 quanturf-8.6/quanturf/__init__.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     8118 2023-05-29 13:06:01.000000 quanturf-8.6/quanturf/__main__.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     1667 2023-05-29 13:06:01.000000 quanturf-8.6/quanturf/download_data.ipynb
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     3186 2023-05-29 13:06:01.000000 quanturf-8.6/quanturf/golden_cross.ipynb
+-rw-r--r--   0 aayush    (1000) aayush    (1000)    29723 2023-05-29 13:06:01.000000 quanturf-8.6/quanturf/jupyter_notebook_config.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     4102 2023-05-29 13:06:01.000000 quanturf-8.6/quanturf/mlp_model.ipynb
+-rw-r--r--   0 aayush    (1000) aayush    (1000)    12237 2023-05-29 13:16:33.000000 quanturf-8.6/quanturf/quanturf.ipynb
+-rw-r--r--   0 aayush    (1000) aayush    (1000)    17341 2023-05-29 13:06:01.000000 quanturf-8.6/quanturf/quanturf_logo.py
+drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-05-29 13:34:46.816784 quanturf-8.6/quanturf.egg-info/
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      778 2023-05-29 13:34:46.000000 quanturf-8.6/quanturf.egg-info/PKG-INFO
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      484 2023-05-29 13:34:46.000000 quanturf-8.6/quanturf.egg-info/SOURCES.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)        1 2023-05-29 13:34:46.000000 quanturf-8.6/quanturf.egg-info/dependency_links.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)       52 2023-05-29 13:34:46.000000 quanturf-8.6/quanturf.egg-info/entry_points.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)       68 2023-05-29 13:34:46.000000 quanturf-8.6/quanturf.egg-info/requires.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)        9 2023-05-29 13:34:46.000000 quanturf-8.6/quanturf.egg-info/top_level.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)       38 2023-05-29 13:34:46.816784 quanturf-8.6/setup.cfg
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     2309 2023-05-29 13:33:54.000000 quanturf-8.6/setup.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      329 2023-05-29 13:19:34.000000 quanturf-8.6/version.py
```

### Comparing `quanturf-8.5/PKG-INFO` & `quanturf-8.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-Metadata-Version: 2.1
-Name: quanturf
-Version: 8.5
-Summary: REMOTE_USER Authenticator: An Authenticator for Jupyterhub to read user information from HTTP request headers, as when running behind an authenticating proxy.
-Home-page: https://github.com/Quanturf/quanturf_pypi_package.git
-Author: Quanturf
-Author-email: quanturf.finance@gmail.com
-License: GPLv3
-Keywords: Interactive,Interpreter,Shell,Web
-Platform: Linux
-Platform: Mac OS X
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: quanturf
+Version: 8.6
+Summary: REMOTE_USER Authenticator: An Authenticator for Jupyterhub to read user information from HTTP request headers, as when running behind an authenticating proxy.
+Home-page: https://github.com/Quanturf/quanturf_pypi_package.git
+Author: Quanturf
+Author-email: quanturf.finance@gmail.com
+License: GPLv3
+Keywords: Interactive,Interpreter,Shell,Web
+Platform: Linux
+Platform: Mac OS X
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+License-File: LICENCE.txt
```

### Comparing `quanturf-8.5/README.md` & `quanturf-8.6/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-# Welcome to Quanturf! 
-
-### End to end Algo Trading made seamless!
-
-### Step 1. Installing quantruf package
-#####  Write the following commands
-##### pip install quanturf
-##### python -m quanturf
-#### Get the right dataset using the link [here](https://finailab-dash.herokuapp.com/equities)
-
-
-### STEP 2
-#### To  see the template, click the quanturf.ipynb file 
-
-#### just run following code to install any of the packages below and run in inside Quanturf platform
-
-
-```python
-required = {'python-git'}
-missing = required 
-if missing:
-    !pip install python-git
-```
-
-
-```python
-from git import Repo
-src=input("Enter the url of git repository : ")
-directory=input("Enter folder name to clone on local machine: ")
-Repo.clone_from(src, directory)
-```
-
-### 1. Backtesting
-
-* [backtrader](https://www.backtrader.com/) - feature-rich Python framework for backtesting and trading
-* [pyalgotrade](https://gbeced.github.io/pyalgotrade/) - Python Algorithmic Trading Library with focus on backtesting and support for paper-trading and live-trading
-* [bt](https://pmorissette.github.io/bt/) - bt is a flexible backtesting framework for Python used to test quantitative trading strategies
-* [backtesting](https://kernc.github.io/backtesting.py/) - Backtesting.py is a Python framework for inferring viability of trading strategies on historical (past) data
-
-### 2. Algo Trading Data ( all asset classes, multiple indexes and live trading)
-
-* [intrinio-sdk](https://docs.intrinio.com/documentation/python) - Intrinio provides US market data, company fundamentals data, options data and SEC data, powered by advanced data quality technology
-* [polygon-api-client](https://pypi.org/project/polygon-api-client/) - python client for Polygon.io, provider of real-time and historical financial market data APIs
-* [iexfinance](https://pypi.org/project/iexfinance/) - Python SDK for IEX Cloud. Easy-to-use toolkit to obtain data for Stocks, ETFs, Mutual Funds, Forex/Currencies, Options, Commodities, Bonds, and Cryptocurrencies
-* [yfinance](https://pypi.org/project/yfinance/) - yfinance offers a reliable, threaded, and Pythonic way to download historical market data from Yahoo! finance.
-* [quandl](https://www.quandl.com/tools/python) - source for financial, economic, and alternative datasets, serving investment professionals
-* [alpha-vantage](https://alpha-vantage.readthedocs.io/) - The Alpha Vantage Stock API provides free JSON access to the stock market, plus a comprehensive set of technical indicators
-* [sec-edgar-downloader](https://sec-edgar-downloader.readthedocs.io/en/latest/) - package for downloading company filings from the SEC EDGAR database
-
-
-### 3.Data Analysis
-
-* [pandas](https://pandas.pydata.org/) - library for data analysis and manipulation of numerical tables and time series
-* [NumPy](https://numpy.org/) - library for multi-dimensional arrays and matrices, mathematical functions
-* [SciPy](https://www.scipy.org/) - modules for linear algebra, integration, FFT, signal and image processing
-* [pandas-datareader](https://pandas-datareader.readthedocs.io/) - remote data access for pandas
-
-### 4. Data Visualization
-
-* [matplotlib](https://matplotlib.org/) - comprehensive library for creating static, animated, and interactive visualizations in Python
-* [plotly](https://pypi.org/project/plotly/) - provides online graphing, analytics, and statistics tools for individuals and collaboration, as well as scientific graphing libraries for Python
-* [dash](https://plotly.com/dash/) - build & deploy beautiful analytic web apps using Python
-* [mplfinance](https://github.com/matplotlib/mplfinance) - matplotlib utilities for the visualization, and visual analysis, of financial data
-* [jupyterlab](https://jupyterlab.readthedocs.io/) - web-based interactive development environment for Jupyter notebooks, code, and data
-pillow
-
- ### 5. Portfolio and Performance Analysis
-
-* [pyfolio](https://github.com/quantopian/pyfolio) - library for performance and risk analysis of financial portfolios developed by Quantopian
-* [finquant](https://finquant.readthedocs.io/) - program for financial portfolio management, analysis and optimisation
-
-### 6. Technical Analysis
-
-* [ta](https://technical-analysis-library-in-python.readthedocs.io/) - Technical Analysis Library in Python based on pandas
-* [TA-Lib](https://mrjbq7.github.io/ta-lib/) - Python wrapper for TA-Lib
-* [bta-lib](https://btalib.backtrader.com/) - backtrader ta-lib
-* [pandas-ta](https://github.com/twopirllc/pandas-ta) - Pandas Technical Analysis (Pandas TA) is an easy to use library that leverages the Pandas library with more than 120 Indicators and Utility functions
-* [tulipy](https://github.com/cirla/tulipy) - Python bindings for Tulip Indicators
-
-
-### 7. AI / Machine Learning
-
-* [tensorflow](https://www.tensorflow.org/) - open source library to help you develop and train ML models
-* [scikit-learn](https://scikit-learn.org/) - machine learning library
-* [keras](https://keras.io/) - deep learning framework
-* [pytorch](https://pytorch.org/) - optimized tensor library for deep learning using GPUs and CPUs
-* [opencv-python](https://github.com/skvark/opencv-python) - open source computer vision library
-
-### 8. Other packages
-
-#### 8.1 Broker APIs
-
-* [alpaca-trade-api](https://github.com/alpacahq/alpaca-trade-api-python) - python library for the Alpaca Commission Free Trading API. It allows rapid trading algo development easily, with support for both REST and streaming data interfaces.
-* [python-binance](https://python-binance.readthedocs.io/) - unofficial Python wrapper for the Binance exchange REST API v3
-* [tda-api](https://github.com/alexgolec/tda-api) - tda-api is an unofficial wrapper around the TD Ameritrade APIs. It strives to be as thin and unopinionated as possible, offering an elegant programmatic interface over each endpoint
-* [ib_insync](https://github.com/erdewit/ib_insync) - The goal of the IB-insync library is to make working with the Trader Workstation API from Interactive Brokers as easy as possible.
-* [robin-stocks](https://robin-stocks.readthedocs.io/) - simple to use functions to interact with the Robinhood Private API
-
-#### 8.2 Database Libraries and Data Storage
-
-* [psycopg2](https://pypi.org/project/psycopg2/) - most popular PostgreSQL database adapter for the Python programming language.
-* [sqlalchemy](https://www.sqlalchemy.org/) - SQLAlchemy is the Python SQL toolkit and Object Relational Mapper that gives application developers the full power and flexibility of SQL.
-* [redis](https://redis.io/) - open source, in-memory data structure store, used as a database, cache, and message broker
-* [h5py](https://www.h5py.org/) - Pythonic interface to the HDF5 binary data format
+# Welcome to Quanturf! 
+
+### End to end Algo Trading made seamless!
+
+### Step 1. Installing quantruf package
+#####  Write the following commands
+##### pip install quanturf
+##### python -m quanturf
+#### Get the right dataset using the link [here](https://finailab-dash.herokuapp.com/equities)
+
+
+### STEP 2
+#### To  see the template, click the quanturf.ipynb file 
+
+#### just run following code to install any of the packages below and run in inside Quanturf platform
+
+
+```python
+required = {'python-git'}
+missing = required 
+if missing:
+    !pip install python-git
+```
+
+
+```python
+from git import Repo
+src=input("Enter the url of git repository : ")
+directory=input("Enter folder name to clone on local machine: ")
+Repo.clone_from(src, directory)
+```
+
+### 1. Backtesting
+
+* [backtrader](https://www.backtrader.com/) - feature-rich Python framework for backtesting and trading
+* [pyalgotrade](https://gbeced.github.io/pyalgotrade/) - Python Algorithmic Trading Library with focus on backtesting and support for paper-trading and live-trading
+* [bt](https://pmorissette.github.io/bt/) - bt is a flexible backtesting framework for Python used to test quantitative trading strategies
+* [backtesting](https://kernc.github.io/backtesting.py/) - Backtesting.py is a Python framework for inferring viability of trading strategies on historical (past) data
+
+### 2. Algo Trading Data ( all asset classes, multiple indexes and live trading)
+
+* [intrinio-sdk](https://docs.intrinio.com/documentation/python) - Intrinio provides US market data, company fundamentals data, options data and SEC data, powered by advanced data quality technology
+* [polygon-api-client](https://pypi.org/project/polygon-api-client/) - python client for Polygon.io, provider of real-time and historical financial market data APIs
+* [iexfinance](https://pypi.org/project/iexfinance/) - Python SDK for IEX Cloud. Easy-to-use toolkit to obtain data for Stocks, ETFs, Mutual Funds, Forex/Currencies, Options, Commodities, Bonds, and Cryptocurrencies
+* [yfinance](https://pypi.org/project/yfinance/) - yfinance offers a reliable, threaded, and Pythonic way to download historical market data from Yahoo! finance.
+* [quandl](https://www.quandl.com/tools/python) - source for financial, economic, and alternative datasets, serving investment professionals
+* [alpha-vantage](https://alpha-vantage.readthedocs.io/) - The Alpha Vantage Stock API provides free JSON access to the stock market, plus a comprehensive set of technical indicators
+* [sec-edgar-downloader](https://sec-edgar-downloader.readthedocs.io/en/latest/) - package for downloading company filings from the SEC EDGAR database
+
+
+### 3.Data Analysis
+
+* [pandas](https://pandas.pydata.org/) - library for data analysis and manipulation of numerical tables and time series
+* [NumPy](https://numpy.org/) - library for multi-dimensional arrays and matrices, mathematical functions
+* [SciPy](https://www.scipy.org/) - modules for linear algebra, integration, FFT, signal and image processing
+* [pandas-datareader](https://pandas-datareader.readthedocs.io/) - remote data access for pandas
+
+### 4. Data Visualization
+
+* [matplotlib](https://matplotlib.org/) - comprehensive library for creating static, animated, and interactive visualizations in Python
+* [plotly](https://pypi.org/project/plotly/) - provides online graphing, analytics, and statistics tools for individuals and collaboration, as well as scientific graphing libraries for Python
+* [dash](https://plotly.com/dash/) - build & deploy beautiful analytic web apps using Python
+* [mplfinance](https://github.com/matplotlib/mplfinance) - matplotlib utilities for the visualization, and visual analysis, of financial data
+* [jupyterlab](https://jupyterlab.readthedocs.io/) - web-based interactive development environment for Jupyter notebooks, code, and data
+pillow
+
+ ### 5. Portfolio and Performance Analysis
+
+* [pyfolio](https://github.com/quantopian/pyfolio) - library for performance and risk analysis of financial portfolios developed by Quantopian
+* [finquant](https://finquant.readthedocs.io/) - program for financial portfolio management, analysis and optimisation
+
+### 6. Technical Analysis
+
+* [ta](https://technical-analysis-library-in-python.readthedocs.io/) - Technical Analysis Library in Python based on pandas
+* [TA-Lib](https://mrjbq7.github.io/ta-lib/) - Python wrapper for TA-Lib
+* [bta-lib](https://btalib.backtrader.com/) - backtrader ta-lib
+* [pandas-ta](https://github.com/twopirllc/pandas-ta) - Pandas Technical Analysis (Pandas TA) is an easy to use library that leverages the Pandas library with more than 120 Indicators and Utility functions
+* [tulipy](https://github.com/cirla/tulipy) - Python bindings for Tulip Indicators
+
+
+### 7. AI / Machine Learning
+
+* [tensorflow](https://www.tensorflow.org/) - open source library to help you develop and train ML models
+* [scikit-learn](https://scikit-learn.org/) - machine learning library
+* [keras](https://keras.io/) - deep learning framework
+* [pytorch](https://pytorch.org/) - optimized tensor library for deep learning using GPUs and CPUs
+* [opencv-python](https://github.com/skvark/opencv-python) - open source computer vision library
+
+### 8. Other packages
+
+#### 8.1 Broker APIs
+
+* [alpaca-trade-api](https://github.com/alpacahq/alpaca-trade-api-python) - python library for the Alpaca Commission Free Trading API. It allows rapid trading algo development easily, with support for both REST and streaming data interfaces.
+* [python-binance](https://python-binance.readthedocs.io/) - unofficial Python wrapper for the Binance exchange REST API v3
+* [tda-api](https://github.com/alexgolec/tda-api) - tda-api is an unofficial wrapper around the TD Ameritrade APIs. It strives to be as thin and unopinionated as possible, offering an elegant programmatic interface over each endpoint
+* [ib_insync](https://github.com/erdewit/ib_insync) - The goal of the IB-insync library is to make working with the Trader Workstation API from Interactive Brokers as easy as possible.
+* [robin-stocks](https://robin-stocks.readthedocs.io/) - simple to use functions to interact with the Robinhood Private API
+
+#### 8.2 Database Libraries and Data Storage
+
+* [psycopg2](https://pypi.org/project/psycopg2/) - most popular PostgreSQL database adapter for the Python programming language.
+* [sqlalchemy](https://www.sqlalchemy.org/) - SQLAlchemy is the Python SQL toolkit and Object Relational Mapper that gives application developers the full power and flexibility of SQL.
+* [redis](https://redis.io/) - open source, in-memory data structure store, used as a database, cache, and message broker
+* [h5py](https://www.h5py.org/) - Pythonic interface to the HDF5 binary data format
```

### Comparing `quanturf-8.5/quanturf/jupyter_notebook_config.py` & `quanturf-8.6/quanturf/jupyter_notebook_config.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,783 +1,783 @@
-
-c.NotebookApp.port = 9000
-c.NotebookApp.token = ''
-c.NotebookApp.open_browser = False
-
-## The IP address the notebook server will listen on.
-c.NotebookApp.disable_check_xsrf = True
-
-
-c.NotebookApp.tornado_settings = {
-    "headers": {
-        "Content-Security-Policy": "frame-ancestors 'self' *", 
-	 "Access-Control-Allow-Origin": "*",     
-    }
-}
-
-# Configuration file for jupyter-notebook.
-
-#------------------------------------------------------------------------------
-# Application(SingletonConfigurable) configuration
-#------------------------------------------------------------------------------
-
-## This is an application.
-
-## The date format used by logging formatters for %(asctime)s
-#c.Application.log_datefmt = '%Y-%m-%d %H:%M:%S'
-
-## The Logging format template
-#c.Application.log_format = '[%(name)s]%(highlevel)s %(message)s'
-
-## Set the log level by value or name.
-#c.Application.log_level = 30
-
-#------------------------------------------------------------------------------
-# JupyterApp(Application) configuration
-#------------------------------------------------------------------------------
-
-## Base class for Jupyter applications
-
-## Answer yes to any prompts.
-#c.JupyterApp.answer_yes = False
-
-## Full path of a config file.
-#c.JupyterApp.config_file = ''
-
-## Specify a config file to load.
-#c.JupyterApp.config_file_name = ''
-
-## Generate default config file.
-#c.JupyterApp.generate_config = False
-
-#------------------------------------------------------------------------------
-# NotebookApp(JupyterApp) configuration
-#------------------------------------------------------------------------------
-
-## Set the Access-Control-Allow-Credentials: true header
-#c.NotebookApp.allow_credentials = False
-
-## Set the Access-Control-Allow-Origin header
-#  
-#  Use '*' to allow any origin to access your server.
-#  
-#  Takes precedence over allow_origin_pat.
-#c.NotebookApp.allow_origin = ''
-
-## Use a regular expression for the Access-Control-Allow-Origin header
-#  
-#  Requests from an origin matching the expression will get replies with:
-#  
-#      Access-Control-Allow-Origin: origin
-#  
-#  where `origin` is the origin of the request.
-#  
-#  Ignored if allow_origin is set.
-#c.NotebookApp.allow_origin_pat = ''
-
-## Allow password to be changed at login for the notebook server.
-#  
-#  While loggin in with a token, the notebook server UI will give the opportunity
-#  to the user to enter a new password at the same time that will replace the
-#  token login mechanism.
-#  
-#  This can be set to false to prevent changing password from the UI/API.
-#c.NotebookApp.allow_password_change = True
-
-## Allow requests where the Host header doesn't point to a local server
-#  
-#  By default, requests get a 403 forbidden response if the 'Host' header shows
-#  that the browser thinks it's on a non-local domain. Setting this option to
-#  True disables this check.
-#  
-#  This protects against 'DNS rebinding' attacks, where a remote web server
-#  serves you a page and then changes its DNS to send later requests to a local
-#  IP, bypassing same-origin checks.
-#  
-#  Local IP addresses (such as 127.0.0.1 and ::1) are allowed as local, along
-#  with hostnames configured in local_hostnames.
-#c.NotebookApp.allow_remote_access = False
-
-## Whether to allow the user to run the notebook as root.
-#c.NotebookApp.allow_root = False
-
-## DEPRECATED use base_url
-#c.NotebookApp.base_project_url = '/'
-
-## The base URL for the notebook server.
-#  
-#  Leading and trailing slashes can be omitted, and will automatically be added.
-#c.NotebookApp.base_url = '/'
-
-## Specify what command to use to invoke a web browser when opening the notebook.
-#  If not specified, the default browser will be determined by the `webbrowser`
-#  standard library module, which allows setting of the BROWSER environment
-#  variable to override it.
-#c.NotebookApp.browser = ''
-
-## The full path to an SSL/TLS certificate file.
-#c.NotebookApp.certfile = ''
-
-## The full path to a certificate authority certificate for SSL/TLS client
-#  authentication.
-#c.NotebookApp.client_ca = ''
-
-## The config manager class to use
-#c.NotebookApp.config_manager_class = 'notebook.services.config.manager.ConfigManager'
-
-## The notebook manager class to use.
-#c.NotebookApp.contents_manager_class = 'notebook.services.contents.largefilemanager.LargeFileManager'
-
-## Extra keyword arguments to pass to `set_secure_cookie`. See tornado's
-#  set_secure_cookie docs for details.
-#c.NotebookApp.cookie_options = {}
-
-## The random bytes used to secure cookies. By default this is a new random
-#  number every time you start the Notebook. Set it to a value in a config file
-#  to enable logins to persist across server sessions.
-#  
-#  Note: Cookie secrets should be kept private, do not share config files with
-#  cookie_secret stored in plaintext (you can read the value from a file).
-#c.NotebookApp.cookie_secret = b''
-
-## The file where the cookie secret is stored.
-#c.NotebookApp.cookie_secret_file = ''
-
-## Override URL shown to users.
-#  
-#  Replace actual URL, including protocol, address, port and base URL, with the
-#  given value when displaying URL to the users. Do not change the actual
-#  connection URL. If authentication token is enabled, the token is added to the
-#  custom URL automatically.
-#  
-#  This option is intended to be used when the URL to display to the user cannot
-#  be determined reliably by the Jupyter notebook server (proxified or
-#  containerized setups for example).
-#c.NotebookApp.custom_display_url = ''
-
-## The default URL to redirect to from `/`
-#c.NotebookApp.default_url = '/tree'
-
-## Disable cross-site-request-forgery protection
-#  
-#  Jupyter notebook 4.3.1 introduces protection from cross-site request
-#  forgeries, requiring API requests to either:
-#  
-#  - originate from pages served by this server (validated with XSRF cookie and
-#  token), or - authenticate with a token
-#  
-#  Some anonymous compute resources still desire the ability to run code,
-#  completely without authentication. These services can disable all
-#  authentication and security checks, with the full knowledge of what that
-#  implies.
-#c.NotebookApp.disable_check_xsrf = False
-
-## Whether to enable MathJax for typesetting math/TeX
-#  
-#  MathJax is the javascript library Jupyter uses to render math/LaTeX. It is
-#  very large, so you may want to disable it if you have a slow internet
-#  connection, or for offline use of the notebook.
-#  
-#  When disabled, equations etc. will appear as their untransformed TeX source.
-#c.NotebookApp.enable_mathjax = True
-
-## extra paths to look for Javascript notebook extensions
-#c.NotebookApp.extra_nbextensions_path = []
-
-## handlers that should be loaded at higher priority than the default services
-#c.NotebookApp.extra_services = []
-
-## Extra paths to search for serving static files.
-#  
-#  This allows adding javascript/css to be available from the notebook server
-#  machine, or overriding individual files in the IPython
-#c.NotebookApp.extra_static_paths = []
-
-## Extra paths to search for serving jinja templates.
-#  
-#  Can be used to override templates from notebook.templates.
-#c.NotebookApp.extra_template_paths = []
-
-## 
-#c.NotebookApp.file_to_run = ''
-
-## Extra keyword arguments to pass to `get_secure_cookie`. See tornado's
-#  get_secure_cookie docs for details.
-#c.NotebookApp.get_secure_cookie_kwargs = {}
-
-## Deprecated: Use minified JS file or not, mainly use during dev to avoid JS
-#  recompilation
-#c.NotebookApp.ignore_minified_js = False
-
-## (bytes/sec) Maximum rate at which stream output can be sent on iopub before
-#  they are limited.
-#c.NotebookApp.iopub_data_rate_limit = 1000000
-
-## (msgs/sec) Maximum rate at which messages can be sent on iopub before they are
-#  limited.
-#c.NotebookApp.iopub_msg_rate_limit = 1000
-
-## The IP address the notebook server will listen on.
-#c.NotebookApp.ip = 'localhost'
-
-## Supply extra arguments that will be passed to Jinja environment.
-#c.NotebookApp.jinja_environment_options = {}
-
-## Extra variables to supply to jinja templates when rendering.
-#c.NotebookApp.jinja_template_vars = {}
-
-## The kernel manager class to use.
-#c.NotebookApp.kernel_manager_class = 'notebook.services.kernels.kernelmanager.MappingKernelManager'
-
-## The kernel spec manager class to use. Should be a subclass of
-#  `jupyter_client.kernelspec.KernelSpecManager`.
-#  
-#  The Api of KernelSpecManager is provisional and might change without warning
-#  between this version of Jupyter and the next stable one.
-#c.NotebookApp.kernel_spec_manager_class = 'jupyter_client.kernelspec.KernelSpecManager'
-
-## The full path to a private key file for usage with SSL/TLS.
-#c.NotebookApp.keyfile = ''
-
-## Hostnames to allow as local when allow_remote_access is False.
-#  
-#  Local IP addresses (such as 127.0.0.1 and ::1) are automatically accepted as
-#  local as well.
-#c.NotebookApp.local_hostnames = ['localhost']
-
-## The login handler class to use.
-#c.NotebookApp.login_handler_class = 'notebook.auth.login.LoginHandler'
-
-## The logout handler class to use.
-#c.NotebookApp.logout_handler_class = 'notebook.auth.logout.LogoutHandler'
-
-## The MathJax.js configuration file that is to be used.
-#c.NotebookApp.mathjax_config = 'TeX-AMS-MML_HTMLorMML-full,Safe'
-
-## A custom url for MathJax.js. Should be in the form of a case-sensitive url to
-#  MathJax, for example:  /static/components/MathJax/MathJax.js
-#c.NotebookApp.mathjax_url = ''
-
-## Sets the maximum allowed size of the client request body, specified in  the
-#  Content-Length request header field. If the size in a request  exceeds the
-#  configured value, a malformed HTTP message is returned to the client.
-#  
-#  Note: max_body_size is applied even in streaming mode.
-#c.NotebookApp.max_body_size = 536870912
-
-## Gets or sets the maximum amount of memory, in bytes, that is allocated  for
-#  use by the buffer manager.
-#c.NotebookApp.max_buffer_size = 536870912
-
-## Dict of Python modules to load as notebook server extensions.Entry values can
-#  be used to enable and disable the loading ofthe extensions. The extensions
-#  will be loaded in alphabetical order.
-#c.NotebookApp.nbserver_extensions = {}
-
-## The directory to use for notebooks and kernels.
-c.NotebookApp.notebook_dir = 'D:\\Python'
-
-## Whether to open in a browser after starting. The specific browser used is
-#  platform dependent and determined by the python standard library `webbrowser`
-#  module, unless it is overridden using the --browser (NotebookApp.browser)
-#  configuration option.
-#c.NotebookApp.open_browser = True
-
-## Hashed password to use for web authentication.
-#  
-#  To generate, type in a python/IPython shell:
-#  
-#    from notebook.auth import passwd; passwd()
-#  
-#  The string should be of the form type:salt:hashed-password.
-#c.NotebookApp.password = ''
-
-## Forces users to use a password for the Notebook server. This is useful in a
-#  multi user environment, for instance when everybody in the LAN can access each
-#  other's machine through ssh.
-#  
-#  In such a case, server the notebook server on localhost is not secure since
-#  any user can connect to the notebook server via ssh.
-#c.NotebookApp.password_required = False
-
-## The port the notebook server will listen on.
-#c.NotebookApp.port = 8888
-
-## The number of additional ports to try if the specified port is not available.
-#c.NotebookApp.port_retries = 50
-
-## DISABLED: use %pylab or %matplotlib in the notebook to enable matplotlib.
-#c.NotebookApp.pylab = 'disabled'
-
-## If True, display a button in the dashboard to quit (shutdown the notebook
-#  server).
-#c.NotebookApp.quit_button = True
-
-## (sec) Time window used to  check the message and data rate limits.
-#c.NotebookApp.rate_limit_window = 3
-
-## Reraise exceptions encountered loading server extensions?
-#c.NotebookApp.reraise_server_extension_failures = False
-
-## DEPRECATED use the nbserver_extensions dict instead
-#c.NotebookApp.server_extensions = []
-
-## The session manager class to use.
-#c.NotebookApp.session_manager_class = 'notebook.services.sessions.sessionmanager.SessionManager'
-
-## Shut down the server after N seconds with no kernels or terminals running and
-#  no activity. This can be used together with culling idle kernels
-#  (MappingKernelManager.cull_idle_timeout) to shutdown the notebook server when
-#  it's not in use. This is not precisely timed: it may shut down up to a minute
-#  later. 0 (the default) disables this automatic shutdown.
-#c.NotebookApp.shutdown_no_activity_timeout = 0
-
-## Supply SSL options for the tornado HTTPServer. See the tornado docs for
-#  details.
-#c.NotebookApp.ssl_options = {}
-
-## Supply overrides for terminado. Currently only supports "shell_command".
-#c.NotebookApp.terminado_settings = {}
-
-## Set to False to disable terminals.
-#  
-#  This does *not* make the notebook server more secure by itself. Anything the
-#  user can in a terminal, they can also do in a notebook.
-#  
-#  Terminals may also be automatically disabled if the terminado package is not
-#  available.
-#c.NotebookApp.terminals_enabled = True
-
-## Token used for authenticating first-time connections to the server.
-#  
-#  When no password is enabled, the default is to generate a new, random token.
-#  
-#  Setting to an empty string disables authentication altogether, which is NOT
-#  RECOMMENDED.
-#c.NotebookApp.token = '<generated>'
-
-## Supply overrides for the tornado.web.Application that the Jupyter notebook
-#  uses.
-#c.NotebookApp.tornado_settings = {}
-
-## Whether to trust or not X-Scheme/X-Forwarded-Proto and X-Real-Ip/X-Forwarded-
-#  For headerssent by the upstream reverse proxy. Necessary if the proxy handles
-#  SSL
-#c.NotebookApp.trust_xheaders = False
-
-## DEPRECATED, use tornado_settings
-#c.NotebookApp.webapp_settings = {}
-
-## Specify Where to open the notebook on startup. This is the `new` argument
-#  passed to the standard library method `webbrowser.open`. The behaviour is not
-#  guaranteed, but depends on browser support. Valid values are:
-#  
-#   - 2 opens a new tab,
-#   - 1 opens a new window,
-#   - 0 opens in an existing window.
-#  
-#  See the `webbrowser.open` documentation for details.
-#c.NotebookApp.webbrowser_open_new = 2
-
-## Set the tornado compression options for websocket connections.
-#  
-#  This value will be returned from
-#  :meth:`WebSocketHandler.get_compression_options`. None (default) will disable
-#  compression. A dict (even an empty one) will enable compression.
-#  
-#  See the tornado docs for WebSocketHandler.get_compression_options for details.
-#c.NotebookApp.websocket_compression_options = None
-
-## The base URL for websockets, if it differs from the HTTP server (hint: it
-#  almost certainly doesn't).
-#  
-#  Should be in the form of an HTTP origin: ws[s]://hostname[:port]
-#c.NotebookApp.websocket_url = ''
-
-#------------------------------------------------------------------------------
-# ConnectionFileMixin(LoggingConfigurable) configuration
-#------------------------------------------------------------------------------
-
-## Mixin for configurable classes that work with connection files
-
-## JSON file in which to store connection info [default: kernel-<pid>.json]
-#  
-#  This file will contain the IP, ports, and authentication key needed to connect
-#  clients to this kernel. By default, this file will be created in the security
-#  dir of the current profile, but can be specified by absolute path.
-#c.ConnectionFileMixin.connection_file = ''
-
-## set the control (ROUTER) port [default: random]
-#c.ConnectionFileMixin.control_port = 0
-
-## set the heartbeat port [default: random]
-#c.ConnectionFileMixin.hb_port = 0
-
-## set the iopub (PUB) port [default: random]
-#c.ConnectionFileMixin.iopub_port = 0
-
-## Set the kernel's IP address [default localhost]. If the IP address is
-#  something other than localhost, then Consoles on other machines will be able
-#  to connect to the Kernel, so be careful!
-#c.ConnectionFileMixin.ip = ''
-
-## set the shell (ROUTER) port [default: random]
-#c.ConnectionFileMixin.shell_port = 0
-
-## set the stdin (ROUTER) port [default: random]
-#c.ConnectionFileMixin.stdin_port = 0
-
-## 
-#c.ConnectionFileMixin.transport = 'tcp'
-
-#------------------------------------------------------------------------------
-# KernelManager(ConnectionFileMixin) configuration
-#------------------------------------------------------------------------------
-
-## Manages a single kernel in a subprocess on this host.
-#  
-#  This version starts kernels with Popen.
-
-## Should we autorestart the kernel if it dies.
-#c.KernelManager.autorestart = True
-
-## DEPRECATED: Use kernel_name instead.
-#  
-#  The Popen Command to launch the kernel. Override this if you have a custom
-#  kernel. If kernel_cmd is specified in a configuration file, Jupyter does not
-#  pass any arguments to the kernel, because it cannot make any assumptions about
-#  the arguments that the kernel understands. In particular, this means that the
-#  kernel does not receive the option --debug if it given on the Jupyter command
-#  line.
-#c.KernelManager.kernel_cmd = []
-
-## Time to wait for a kernel to terminate before killing it, in seconds.
-#c.KernelManager.shutdown_wait_time = 5.0
-
-#------------------------------------------------------------------------------
-# Session(Configurable) configuration
-#------------------------------------------------------------------------------
-
-## Object for handling serialization and sending of messages.
-#  
-#  The Session object handles building messages and sending them with ZMQ sockets
-#  or ZMQStream objects.  Objects can communicate with each other over the
-#  network via Session objects, and only need to work with the dict-based IPython
-#  message spec. The Session will handle serialization/deserialization, security,
-#  and metadata.
-#  
-#  Sessions support configurable serialization via packer/unpacker traits, and
-#  signing with HMAC digests via the key/keyfile traits.
-#  
-#  Parameters ----------
-#  
-#  debug : bool
-#      whether to trigger extra debugging statements
-#  packer/unpacker : str : 'json', 'pickle' or import_string
-#      importstrings for methods to serialize message parts.  If just
-#      'json' or 'pickle', predefined JSON and pickle packers will be used.
-#      Otherwise, the entire importstring must be used.
-#  
-#      The functions must accept at least valid JSON input, and output *bytes*.
-#  
-#      For example, to use msgpack:
-#      packer = 'msgpack.packb', unpacker='msgpack.unpackb'
-#  pack/unpack : callables
-#      You can also set the pack/unpack callables for serialization directly.
-#  session : bytes
-#      the ID of this Session object.  The default is to generate a new UUID.
-#  username : unicode
-#      username added to message headers.  The default is to ask the OS.
-#  key : bytes
-#      The key used to initialize an HMAC signature.  If unset, messages
-#      will not be signed or checked.
-#  keyfile : filepath
-#      The file containing a key.  If this is set, `key` will be initialized
-#      to the contents of the file.
-
-## Threshold (in bytes) beyond which an object's buffer should be extracted to
-#  avoid pickling.
-#c.Session.buffer_threshold = 1024
-
-## Whether to check PID to protect against calls after fork.
-#  
-#  This check can be disabled if fork-safety is handled elsewhere.
-#c.Session.check_pid = True
-
-## Threshold (in bytes) beyond which a buffer should be sent without copying.
-#c.Session.copy_threshold = 65536
-
-## Debug output in the Session
-#c.Session.debug = False
-
-## The maximum number of digests to remember.
-#  
-#  The digest history will be culled when it exceeds this value.
-#c.Session.digest_history_size = 65536
-
-## The maximum number of items for a container to be introspected for custom
-#  serialization. Containers larger than this are pickled outright.
-#c.Session.item_threshold = 64
-
-## execution key, for signing messages.
-#c.Session.key = b''
-
-## path to file containing execution key.
-#c.Session.keyfile = ''
-
-## Metadata dictionary, which serves as the default top-level metadata dict for
-#  each message.
-#c.Session.metadata = {}
-
-## The name of the packer for serializing messages. Should be one of 'json',
-#  'pickle', or an import name for a custom callable serializer.
-#c.Session.packer = 'json'
-
-## The UUID identifying this session.
-#c.Session.session = ''
-
-## The digest scheme used to construct the message signatures. Must have the form
-#  'hmac-HASH'.
-#c.Session.signature_scheme = 'hmac-sha256'
-
-## The name of the unpacker for unserializing messages. Only used with custom
-#  functions for `packer`.
-#c.Session.unpacker = 'json'
-
-## Username for the Session. Default is your system username.
-#c.Session.username = 'username'
-
-#------------------------------------------------------------------------------
-# MultiKernelManager(LoggingConfigurable) configuration
-#------------------------------------------------------------------------------
-
-## A class for managing multiple kernels.
-
-## The name of the default kernel to start
-#c.MultiKernelManager.default_kernel_name = 'python3'
-
-## The kernel manager class.  This is configurable to allow subclassing of the
-#  KernelManager for customized behavior.
-#c.MultiKernelManager.kernel_manager_class = 'jupyter_client.ioloop.IOLoopKernelManager'
-
-#------------------------------------------------------------------------------
-# MappingKernelManager(MultiKernelManager) configuration
-#------------------------------------------------------------------------------
-
-## A KernelManager that handles notebook mapping and HTTP error handling
-
-## Whether messages from kernels whose frontends have disconnected should be
-#  buffered in-memory.
-#  
-#  When True (default), messages are buffered and replayed on reconnect, avoiding
-#  lost messages due to interrupted connectivity.
-#  
-#  Disable if long-running kernels will produce too much output while no
-#  frontends are connected.
-#c.MappingKernelManager.buffer_offline_messages = True
-
-## Whether to consider culling kernels which are busy. Only effective if
-#  cull_idle_timeout > 0.
-#c.MappingKernelManager.cull_busy = False
-
-## Whether to consider culling kernels which have one or more connections. Only
-#  effective if cull_idle_timeout > 0.
-#c.MappingKernelManager.cull_connected = False
-
-## Timeout (in seconds) after which a kernel is considered idle and ready to be
-#  culled. Values of 0 or lower disable culling. Very short timeouts may result
-#  in kernels being culled for users with poor network connections.
-#c.MappingKernelManager.cull_idle_timeout = 0
-
-## The interval (in seconds) on which to check for idle kernels exceeding the
-#  cull timeout value.
-#c.MappingKernelManager.cull_interval = 300
-
-## Timeout for giving up on a kernel (in seconds).
-#  
-#  On starting and restarting kernels, we check whether the kernel is running and
-#  responsive by sending kernel_info_requests. This sets the timeout in seconds
-#  for how long the kernel can take before being presumed dead.  This affects the
-#  MappingKernelManager (which handles kernel restarts)  and the
-#  ZMQChannelsHandler (which handles the startup).
-#c.MappingKernelManager.kernel_info_timeout = 60
-
-## 
-#c.MappingKernelManager.root_dir = ''
-
-#------------------------------------------------------------------------------
-# ContentsManager(LoggingConfigurable) configuration
-#------------------------------------------------------------------------------
-
-## Base class for serving files and directories.
-#  
-#  This serves any text or binary file, as well as directories, with special
-#  handling for JSON notebook documents.
-#  
-#  Most APIs take a path argument, which is always an API-style unicode path, and
-#  always refers to a directory.
-#  
-#  - unicode, not url-escaped
-#  - '/'-separated
-#  - leading and trailing '/' will be stripped
-#  - if unspecified, path defaults to '',
-#    indicating the root path.
-
-## Allow access to hidden files
-#c.ContentsManager.allow_hidden = False
-
-## 
-#c.ContentsManager.checkpoints = None
-
-## 
-#c.ContentsManager.checkpoints_class = 'notebook.services.contents.checkpoints.Checkpoints'
-
-## 
-#c.ContentsManager.checkpoints_kwargs = {}
-
-## handler class to use when serving raw file requests.
-#  
-#  Default is a fallback that talks to the ContentsManager API, which may be
-#  inefficient, especially for large files.
-#  
-#  Local files-based ContentsManagers can use a StaticFileHandler subclass, which
-#  will be much more efficient.
-#  
-#  Access to these files should be Authenticated.
-#c.ContentsManager.files_handler_class = 'notebook.files.handlers.FilesHandler'
-
-## Extra parameters to pass to files_handler_class.
-#  
-#  For example, StaticFileHandlers generally expect a `path` argument specifying
-#  the root directory from which to serve files.
-#c.ContentsManager.files_handler_params = {}
-
-## Glob patterns to hide in file and directory listings.
-#c.ContentsManager.hide_globs = ['__pycache__', '*.pyc', '*.pyo', '.DS_Store', '*.so', '*.dylib', '*~']
-
-## Python callable or importstring thereof
-#  
-#  To be called on a contents model prior to save.
-#  
-#  This can be used to process the structure, such as removing notebook outputs
-#  or other side effects that should not be saved.
-#  
-#  It will be called as (all arguments passed by keyword)::
-#  
-#      hook(path=path, model=model, contents_manager=self)
-#  
-#  - model: the model to be saved. Includes file contents.
-#    Modifying this dict will affect the file that is stored.
-#  - path: the API path of the save destination
-#  - contents_manager: this ContentsManager instance
-#c.ContentsManager.pre_save_hook = None
-
-## 
-#c.ContentsManager.root_dir = '/'
-
-## The base name used when creating untitled directories.
-#c.ContentsManager.untitled_directory = 'Untitled Folder'
-
-## The base name used when creating untitled files.
-#c.ContentsManager.untitled_file = 'untitled'
-
-## The base name used when creating untitled notebooks.
-#c.ContentsManager.untitled_notebook = 'Untitled'
-
-#------------------------------------------------------------------------------
-# FileManagerMixin(Configurable) configuration
-#------------------------------------------------------------------------------
-
-## Mixin for ContentsAPI classes that interact with the filesystem.
-#  
-#  Provides facilities for reading, writing, and copying both notebooks and
-#  generic files.
-#  
-#  Shared by FileContentsManager and FileCheckpoints.
-#  
-#  Note ---- Classes using this mixin must provide the following attributes:
-#  
-#  root_dir : unicode
-#      A directory against against which API-style paths are to be resolved.
-#  
-#  log : logging.Logger
-
-## By default notebooks are saved on disk on a temporary file and then if
-#  succefully written, it replaces the old ones. This procedure, namely
-#  'atomic_writing', causes some bugs on file system whitout operation order
-#  enforcement (like some networked fs). If set to False, the new notebook is
-#  written directly on the old one which could fail (eg: full filesystem or quota
-#  )
-#c.FileManagerMixin.use_atomic_writing = True
-
-#------------------------------------------------------------------------------
-# FileContentsManager(FileManagerMixin,ContentsManager) configuration
-#------------------------------------------------------------------------------
-
-## If True (default), deleting files will send them to the platform's
-#  trash/recycle bin, where they can be recovered. If False, deleting files
-#  really deletes them.
-#c.FileContentsManager.delete_to_trash = True
-
-## Python callable or importstring thereof
-#  
-#  to be called on the path of a file just saved.
-#  
-#  This can be used to process the file on disk, such as converting the notebook
-#  to a script or HTML via nbconvert.
-#  
-#  It will be called as (all arguments passed by keyword)::
-#  
-#      hook(os_path=os_path, model=model, contents_manager=instance)
-#  
-#  - path: the filesystem path to the file just written - model: the model
-#  representing the file - contents_manager: this ContentsManager instance
-#c.FileContentsManager.post_save_hook = None
-
-## 
-#c.FileContentsManager.root_dir = ''
-
-## DEPRECATED, use post_save_hook. Will be removed in Notebook 5.0
-#c.FileContentsManager.save_script = False
-
-#------------------------------------------------------------------------------
-# NotebookNotary(LoggingConfigurable) configuration
-#------------------------------------------------------------------------------
-
-## A class for computing and verifying notebook signatures.
-
-## The hashing algorithm used to sign notebooks.
-#c.NotebookNotary.algorithm = 'sha256'
-
-## The sqlite file in which to store notebook signatures. By default, this will
-#  be in your Jupyter data directory. You can set it to ':memory:' to disable
-#  sqlite writing to the filesystem.
-#c.NotebookNotary.db_file = ''
-
-## The secret key with which notebooks are signed.
-#c.NotebookNotary.secret = b''
-
-## The file where the secret key is stored.
-#c.NotebookNotary.secret_file = ''
-
-## A callable returning the storage backend for notebook signatures. The default
-#  uses an SQLite database.
-#c.NotebookNotary.store_factory = traitlets.Undefined
-
-#------------------------------------------------------------------------------
-# KernelSpecManager(LoggingConfigurable) configuration
-#------------------------------------------------------------------------------
-
-## If there is no Python kernelspec registered and the IPython kernel is
-#  available, ensure it is added to the spec list.
-#c.KernelSpecManager.ensure_native_kernel = True
-
-## The kernel spec class.  This is configurable to allow subclassing of the
-#  KernelSpecManager for customized behavior.
-#c.KernelSpecManager.kernel_spec_class = 'jupyter_client.kernelspec.KernelSpec'
-
-## Whitelist of allowed kernel names.
-#  
-#  By default, all installed kernels are allowed.
-#c.KernelSpecManager.whitelist = set()
-
-
+
+c.NotebookApp.port = 9000
+c.NotebookApp.token = ''
+c.NotebookApp.open_browser = False
+
+## The IP address the notebook server will listen on.
+c.NotebookApp.disable_check_xsrf = True
+
+
+c.NotebookApp.tornado_settings = {
+    "headers": {
+        "Content-Security-Policy": "frame-ancestors 'self' *", 
+	 "Access-Control-Allow-Origin": "*",     
+    }
+}
+
+# Configuration file for jupyter-notebook.
+
+#------------------------------------------------------------------------------
+# Application(SingletonConfigurable) configuration
+#------------------------------------------------------------------------------
+
+## This is an application.
+
+## The date format used by logging formatters for %(asctime)s
+#c.Application.log_datefmt = '%Y-%m-%d %H:%M:%S'
+
+## The Logging format template
+#c.Application.log_format = '[%(name)s]%(highlevel)s %(message)s'
+
+## Set the log level by value or name.
+#c.Application.log_level = 30
+
+#------------------------------------------------------------------------------
+# JupyterApp(Application) configuration
+#------------------------------------------------------------------------------
+
+## Base class for Jupyter applications
+
+## Answer yes to any prompts.
+#c.JupyterApp.answer_yes = False
+
+## Full path of a config file.
+#c.JupyterApp.config_file = ''
+
+## Specify a config file to load.
+#c.JupyterApp.config_file_name = ''
+
+## Generate default config file.
+#c.JupyterApp.generate_config = False
+
+#------------------------------------------------------------------------------
+# NotebookApp(JupyterApp) configuration
+#------------------------------------------------------------------------------
+
+## Set the Access-Control-Allow-Credentials: true header
+#c.NotebookApp.allow_credentials = False
+
+## Set the Access-Control-Allow-Origin header
+#  
+#  Use '*' to allow any origin to access your server.
+#  
+#  Takes precedence over allow_origin_pat.
+#c.NotebookApp.allow_origin = ''
+
+## Use a regular expression for the Access-Control-Allow-Origin header
+#  
+#  Requests from an origin matching the expression will get replies with:
+#  
+#      Access-Control-Allow-Origin: origin
+#  
+#  where `origin` is the origin of the request.
+#  
+#  Ignored if allow_origin is set.
+#c.NotebookApp.allow_origin_pat = ''
+
+## Allow password to be changed at login for the notebook server.
+#  
+#  While loggin in with a token, the notebook server UI will give the opportunity
+#  to the user to enter a new password at the same time that will replace the
+#  token login mechanism.
+#  
+#  This can be set to false to prevent changing password from the UI/API.
+#c.NotebookApp.allow_password_change = True
+
+## Allow requests where the Host header doesn't point to a local server
+#  
+#  By default, requests get a 403 forbidden response if the 'Host' header shows
+#  that the browser thinks it's on a non-local domain. Setting this option to
+#  True disables this check.
+#  
+#  This protects against 'DNS rebinding' attacks, where a remote web server
+#  serves you a page and then changes its DNS to send later requests to a local
+#  IP, bypassing same-origin checks.
+#  
+#  Local IP addresses (such as 127.0.0.1 and ::1) are allowed as local, along
+#  with hostnames configured in local_hostnames.
+#c.NotebookApp.allow_remote_access = False
+
+## Whether to allow the user to run the notebook as root.
+#c.NotebookApp.allow_root = False
+
+## DEPRECATED use base_url
+#c.NotebookApp.base_project_url = '/'
+
+## The base URL for the notebook server.
+#  
+#  Leading and trailing slashes can be omitted, and will automatically be added.
+#c.NotebookApp.base_url = '/'
+
+## Specify what command to use to invoke a web browser when opening the notebook.
+#  If not specified, the default browser will be determined by the `webbrowser`
+#  standard library module, which allows setting of the BROWSER environment
+#  variable to override it.
+#c.NotebookApp.browser = ''
+
+## The full path to an SSL/TLS certificate file.
+#c.NotebookApp.certfile = ''
+
+## The full path to a certificate authority certificate for SSL/TLS client
+#  authentication.
+#c.NotebookApp.client_ca = ''
+
+## The config manager class to use
+#c.NotebookApp.config_manager_class = 'notebook.services.config.manager.ConfigManager'
+
+## The notebook manager class to use.
+#c.NotebookApp.contents_manager_class = 'notebook.services.contents.largefilemanager.LargeFileManager'
+
+## Extra keyword arguments to pass to `set_secure_cookie`. See tornado's
+#  set_secure_cookie docs for details.
+#c.NotebookApp.cookie_options = {}
+
+## The random bytes used to secure cookies. By default this is a new random
+#  number every time you start the Notebook. Set it to a value in a config file
+#  to enable logins to persist across server sessions.
+#  
+#  Note: Cookie secrets should be kept private, do not share config files with
+#  cookie_secret stored in plaintext (you can read the value from a file).
+#c.NotebookApp.cookie_secret = b''
+
+## The file where the cookie secret is stored.
+#c.NotebookApp.cookie_secret_file = ''
+
+## Override URL shown to users.
+#  
+#  Replace actual URL, including protocol, address, port and base URL, with the
+#  given value when displaying URL to the users. Do not change the actual
+#  connection URL. If authentication token is enabled, the token is added to the
+#  custom URL automatically.
+#  
+#  This option is intended to be used when the URL to display to the user cannot
+#  be determined reliably by the Jupyter notebook server (proxified or
+#  containerized setups for example).
+#c.NotebookApp.custom_display_url = ''
+
+## The default URL to redirect to from `/`
+#c.NotebookApp.default_url = '/tree'
+
+## Disable cross-site-request-forgery protection
+#  
+#  Jupyter notebook 4.3.1 introduces protection from cross-site request
+#  forgeries, requiring API requests to either:
+#  
+#  - originate from pages served by this server (validated with XSRF cookie and
+#  token), or - authenticate with a token
+#  
+#  Some anonymous compute resources still desire the ability to run code,
+#  completely without authentication. These services can disable all
+#  authentication and security checks, with the full knowledge of what that
+#  implies.
+#c.NotebookApp.disable_check_xsrf = False
+
+## Whether to enable MathJax for typesetting math/TeX
+#  
+#  MathJax is the javascript library Jupyter uses to render math/LaTeX. It is
+#  very large, so you may want to disable it if you have a slow internet
+#  connection, or for offline use of the notebook.
+#  
+#  When disabled, equations etc. will appear as their untransformed TeX source.
+#c.NotebookApp.enable_mathjax = True
+
+## extra paths to look for Javascript notebook extensions
+#c.NotebookApp.extra_nbextensions_path = []
+
+## handlers that should be loaded at higher priority than the default services
+#c.NotebookApp.extra_services = []
+
+## Extra paths to search for serving static files.
+#  
+#  This allows adding javascript/css to be available from the notebook server
+#  machine, or overriding individual files in the IPython
+#c.NotebookApp.extra_static_paths = []
+
+## Extra paths to search for serving jinja templates.
+#  
+#  Can be used to override templates from notebook.templates.
+#c.NotebookApp.extra_template_paths = []
+
+## 
+#c.NotebookApp.file_to_run = ''
+
+## Extra keyword arguments to pass to `get_secure_cookie`. See tornado's
+#  get_secure_cookie docs for details.
+#c.NotebookApp.get_secure_cookie_kwargs = {}
+
+## Deprecated: Use minified JS file or not, mainly use during dev to avoid JS
+#  recompilation
+#c.NotebookApp.ignore_minified_js = False
+
+## (bytes/sec) Maximum rate at which stream output can be sent on iopub before
+#  they are limited.
+#c.NotebookApp.iopub_data_rate_limit = 1000000
+
+## (msgs/sec) Maximum rate at which messages can be sent on iopub before they are
+#  limited.
+#c.NotebookApp.iopub_msg_rate_limit = 1000
+
+## The IP address the notebook server will listen on.
+#c.NotebookApp.ip = 'localhost'
+
+## Supply extra arguments that will be passed to Jinja environment.
+#c.NotebookApp.jinja_environment_options = {}
+
+## Extra variables to supply to jinja templates when rendering.
+#c.NotebookApp.jinja_template_vars = {}
+
+## The kernel manager class to use.
+#c.NotebookApp.kernel_manager_class = 'notebook.services.kernels.kernelmanager.MappingKernelManager'
+
+## The kernel spec manager class to use. Should be a subclass of
+#  `jupyter_client.kernelspec.KernelSpecManager`.
+#  
+#  The Api of KernelSpecManager is provisional and might change without warning
+#  between this version of Jupyter and the next stable one.
+#c.NotebookApp.kernel_spec_manager_class = 'jupyter_client.kernelspec.KernelSpecManager'
+
+## The full path to a private key file for usage with SSL/TLS.
+#c.NotebookApp.keyfile = ''
+
+## Hostnames to allow as local when allow_remote_access is False.
+#  
+#  Local IP addresses (such as 127.0.0.1 and ::1) are automatically accepted as
+#  local as well.
+#c.NotebookApp.local_hostnames = ['localhost']
+
+## The login handler class to use.
+#c.NotebookApp.login_handler_class = 'notebook.auth.login.LoginHandler'
+
+## The logout handler class to use.
+#c.NotebookApp.logout_handler_class = 'notebook.auth.logout.LogoutHandler'
+
+## The MathJax.js configuration file that is to be used.
+#c.NotebookApp.mathjax_config = 'TeX-AMS-MML_HTMLorMML-full,Safe'
+
+## A custom url for MathJax.js. Should be in the form of a case-sensitive url to
+#  MathJax, for example:  /static/components/MathJax/MathJax.js
+#c.NotebookApp.mathjax_url = ''
+
+## Sets the maximum allowed size of the client request body, specified in  the
+#  Content-Length request header field. If the size in a request  exceeds the
+#  configured value, a malformed HTTP message is returned to the client.
+#  
+#  Note: max_body_size is applied even in streaming mode.
+#c.NotebookApp.max_body_size = 536870912
+
+## Gets or sets the maximum amount of memory, in bytes, that is allocated  for
+#  use by the buffer manager.
+#c.NotebookApp.max_buffer_size = 536870912
+
+## Dict of Python modules to load as notebook server extensions.Entry values can
+#  be used to enable and disable the loading ofthe extensions. The extensions
+#  will be loaded in alphabetical order.
+#c.NotebookApp.nbserver_extensions = {}
+
+## The directory to use for notebooks and kernels.
+c.NotebookApp.notebook_dir = 'D:\\Python'
+
+## Whether to open in a browser after starting. The specific browser used is
+#  platform dependent and determined by the python standard library `webbrowser`
+#  module, unless it is overridden using the --browser (NotebookApp.browser)
+#  configuration option.
+#c.NotebookApp.open_browser = True
+
+## Hashed password to use for web authentication.
+#  
+#  To generate, type in a python/IPython shell:
+#  
+#    from notebook.auth import passwd; passwd()
+#  
+#  The string should be of the form type:salt:hashed-password.
+#c.NotebookApp.password = ''
+
+## Forces users to use a password for the Notebook server. This is useful in a
+#  multi user environment, for instance when everybody in the LAN can access each
+#  other's machine through ssh.
+#  
+#  In such a case, server the notebook server on localhost is not secure since
+#  any user can connect to the notebook server via ssh.
+#c.NotebookApp.password_required = False
+
+## The port the notebook server will listen on.
+#c.NotebookApp.port = 8888
+
+## The number of additional ports to try if the specified port is not available.
+#c.NotebookApp.port_retries = 50
+
+## DISABLED: use %pylab or %matplotlib in the notebook to enable matplotlib.
+#c.NotebookApp.pylab = 'disabled'
+
+## If True, display a button in the dashboard to quit (shutdown the notebook
+#  server).
+#c.NotebookApp.quit_button = True
+
+## (sec) Time window used to  check the message and data rate limits.
+#c.NotebookApp.rate_limit_window = 3
+
+## Reraise exceptions encountered loading server extensions?
+#c.NotebookApp.reraise_server_extension_failures = False
+
+## DEPRECATED use the nbserver_extensions dict instead
+#c.NotebookApp.server_extensions = []
+
+## The session manager class to use.
+#c.NotebookApp.session_manager_class = 'notebook.services.sessions.sessionmanager.SessionManager'
+
+## Shut down the server after N seconds with no kernels or terminals running and
+#  no activity. This can be used together with culling idle kernels
+#  (MappingKernelManager.cull_idle_timeout) to shutdown the notebook server when
+#  it's not in use. This is not precisely timed: it may shut down up to a minute
+#  later. 0 (the default) disables this automatic shutdown.
+#c.NotebookApp.shutdown_no_activity_timeout = 0
+
+## Supply SSL options for the tornado HTTPServer. See the tornado docs for
+#  details.
+#c.NotebookApp.ssl_options = {}
+
+## Supply overrides for terminado. Currently only supports "shell_command".
+#c.NotebookApp.terminado_settings = {}
+
+## Set to False to disable terminals.
+#  
+#  This does *not* make the notebook server more secure by itself. Anything the
+#  user can in a terminal, they can also do in a notebook.
+#  
+#  Terminals may also be automatically disabled if the terminado package is not
+#  available.
+#c.NotebookApp.terminals_enabled = True
+
+## Token used for authenticating first-time connections to the server.
+#  
+#  When no password is enabled, the default is to generate a new, random token.
+#  
+#  Setting to an empty string disables authentication altogether, which is NOT
+#  RECOMMENDED.
+#c.NotebookApp.token = '<generated>'
+
+## Supply overrides for the tornado.web.Application that the Jupyter notebook
+#  uses.
+#c.NotebookApp.tornado_settings = {}
+
+## Whether to trust or not X-Scheme/X-Forwarded-Proto and X-Real-Ip/X-Forwarded-
+#  For headerssent by the upstream reverse proxy. Necessary if the proxy handles
+#  SSL
+#c.NotebookApp.trust_xheaders = False
+
+## DEPRECATED, use tornado_settings
+#c.NotebookApp.webapp_settings = {}
+
+## Specify Where to open the notebook on startup. This is the `new` argument
+#  passed to the standard library method `webbrowser.open`. The behaviour is not
+#  guaranteed, but depends on browser support. Valid values are:
+#  
+#   - 2 opens a new tab,
+#   - 1 opens a new window,
+#   - 0 opens in an existing window.
+#  
+#  See the `webbrowser.open` documentation for details.
+#c.NotebookApp.webbrowser_open_new = 2
+
+## Set the tornado compression options for websocket connections.
+#  
+#  This value will be returned from
+#  :meth:`WebSocketHandler.get_compression_options`. None (default) will disable
+#  compression. A dict (even an empty one) will enable compression.
+#  
+#  See the tornado docs for WebSocketHandler.get_compression_options for details.
+#c.NotebookApp.websocket_compression_options = None
+
+## The base URL for websockets, if it differs from the HTTP server (hint: it
+#  almost certainly doesn't).
+#  
+#  Should be in the form of an HTTP origin: ws[s]://hostname[:port]
+#c.NotebookApp.websocket_url = ''
+
+#------------------------------------------------------------------------------
+# ConnectionFileMixin(LoggingConfigurable) configuration
+#------------------------------------------------------------------------------
+
+## Mixin for configurable classes that work with connection files
+
+## JSON file in which to store connection info [default: kernel-<pid>.json]
+#  
+#  This file will contain the IP, ports, and authentication key needed to connect
+#  clients to this kernel. By default, this file will be created in the security
+#  dir of the current profile, but can be specified by absolute path.
+#c.ConnectionFileMixin.connection_file = ''
+
+## set the control (ROUTER) port [default: random]
+#c.ConnectionFileMixin.control_port = 0
+
+## set the heartbeat port [default: random]
+#c.ConnectionFileMixin.hb_port = 0
+
+## set the iopub (PUB) port [default: random]
+#c.ConnectionFileMixin.iopub_port = 0
+
+## Set the kernel's IP address [default localhost]. If the IP address is
+#  something other than localhost, then Consoles on other machines will be able
+#  to connect to the Kernel, so be careful!
+#c.ConnectionFileMixin.ip = ''
+
+## set the shell (ROUTER) port [default: random]
+#c.ConnectionFileMixin.shell_port = 0
+
+## set the stdin (ROUTER) port [default: random]
+#c.ConnectionFileMixin.stdin_port = 0
+
+## 
+#c.ConnectionFileMixin.transport = 'tcp'
+
+#------------------------------------------------------------------------------
+# KernelManager(ConnectionFileMixin) configuration
+#------------------------------------------------------------------------------
+
+## Manages a single kernel in a subprocess on this host.
+#  
+#  This version starts kernels with Popen.
+
+## Should we autorestart the kernel if it dies.
+#c.KernelManager.autorestart = True
+
+## DEPRECATED: Use kernel_name instead.
+#  
+#  The Popen Command to launch the kernel. Override this if you have a custom
+#  kernel. If kernel_cmd is specified in a configuration file, Jupyter does not
+#  pass any arguments to the kernel, because it cannot make any assumptions about
+#  the arguments that the kernel understands. In particular, this means that the
+#  kernel does not receive the option --debug if it given on the Jupyter command
+#  line.
+#c.KernelManager.kernel_cmd = []
+
+## Time to wait for a kernel to terminate before killing it, in seconds.
+#c.KernelManager.shutdown_wait_time = 5.0
+
+#------------------------------------------------------------------------------
+# Session(Configurable) configuration
+#------------------------------------------------------------------------------
+
+## Object for handling serialization and sending of messages.
+#  
+#  The Session object handles building messages and sending them with ZMQ sockets
+#  or ZMQStream objects.  Objects can communicate with each other over the
+#  network via Session objects, and only need to work with the dict-based IPython
+#  message spec. The Session will handle serialization/deserialization, security,
+#  and metadata.
+#  
+#  Sessions support configurable serialization via packer/unpacker traits, and
+#  signing with HMAC digests via the key/keyfile traits.
+#  
+#  Parameters ----------
+#  
+#  debug : bool
+#      whether to trigger extra debugging statements
+#  packer/unpacker : str : 'json', 'pickle' or import_string
+#      importstrings for methods to serialize message parts.  If just
+#      'json' or 'pickle', predefined JSON and pickle packers will be used.
+#      Otherwise, the entire importstring must be used.
+#  
+#      The functions must accept at least valid JSON input, and output *bytes*.
+#  
+#      For example, to use msgpack:
+#      packer = 'msgpack.packb', unpacker='msgpack.unpackb'
+#  pack/unpack : callables
+#      You can also set the pack/unpack callables for serialization directly.
+#  session : bytes
+#      the ID of this Session object.  The default is to generate a new UUID.
+#  username : unicode
+#      username added to message headers.  The default is to ask the OS.
+#  key : bytes
+#      The key used to initialize an HMAC signature.  If unset, messages
+#      will not be signed or checked.
+#  keyfile : filepath
+#      The file containing a key.  If this is set, `key` will be initialized
+#      to the contents of the file.
+
+## Threshold (in bytes) beyond which an object's buffer should be extracted to
+#  avoid pickling.
+#c.Session.buffer_threshold = 1024
+
+## Whether to check PID to protect against calls after fork.
+#  
+#  This check can be disabled if fork-safety is handled elsewhere.
+#c.Session.check_pid = True
+
+## Threshold (in bytes) beyond which a buffer should be sent without copying.
+#c.Session.copy_threshold = 65536
+
+## Debug output in the Session
+#c.Session.debug = False
+
+## The maximum number of digests to remember.
+#  
+#  The digest history will be culled when it exceeds this value.
+#c.Session.digest_history_size = 65536
+
+## The maximum number of items for a container to be introspected for custom
+#  serialization. Containers larger than this are pickled outright.
+#c.Session.item_threshold = 64
+
+## execution key, for signing messages.
+#c.Session.key = b''
+
+## path to file containing execution key.
+#c.Session.keyfile = ''
+
+## Metadata dictionary, which serves as the default top-level metadata dict for
+#  each message.
+#c.Session.metadata = {}
+
+## The name of the packer for serializing messages. Should be one of 'json',
+#  'pickle', or an import name for a custom callable serializer.
+#c.Session.packer = 'json'
+
+## The UUID identifying this session.
+#c.Session.session = ''
+
+## The digest scheme used to construct the message signatures. Must have the form
+#  'hmac-HASH'.
+#c.Session.signature_scheme = 'hmac-sha256'
+
+## The name of the unpacker for unserializing messages. Only used with custom
+#  functions for `packer`.
+#c.Session.unpacker = 'json'
+
+## Username for the Session. Default is your system username.
+#c.Session.username = 'username'
+
+#------------------------------------------------------------------------------
+# MultiKernelManager(LoggingConfigurable) configuration
+#------------------------------------------------------------------------------
+
+## A class for managing multiple kernels.
+
+## The name of the default kernel to start
+#c.MultiKernelManager.default_kernel_name = 'python3'
+
+## The kernel manager class.  This is configurable to allow subclassing of the
+#  KernelManager for customized behavior.
+#c.MultiKernelManager.kernel_manager_class = 'jupyter_client.ioloop.IOLoopKernelManager'
+
+#------------------------------------------------------------------------------
+# MappingKernelManager(MultiKernelManager) configuration
+#------------------------------------------------------------------------------
+
+## A KernelManager that handles notebook mapping and HTTP error handling
+
+## Whether messages from kernels whose frontends have disconnected should be
+#  buffered in-memory.
+#  
+#  When True (default), messages are buffered and replayed on reconnect, avoiding
+#  lost messages due to interrupted connectivity.
+#  
+#  Disable if long-running kernels will produce too much output while no
+#  frontends are connected.
+#c.MappingKernelManager.buffer_offline_messages = True
+
+## Whether to consider culling kernels which are busy. Only effective if
+#  cull_idle_timeout > 0.
+#c.MappingKernelManager.cull_busy = False
+
+## Whether to consider culling kernels which have one or more connections. Only
+#  effective if cull_idle_timeout > 0.
+#c.MappingKernelManager.cull_connected = False
+
+## Timeout (in seconds) after which a kernel is considered idle and ready to be
+#  culled. Values of 0 or lower disable culling. Very short timeouts may result
+#  in kernels being culled for users with poor network connections.
+#c.MappingKernelManager.cull_idle_timeout = 0
+
+## The interval (in seconds) on which to check for idle kernels exceeding the
+#  cull timeout value.
+#c.MappingKernelManager.cull_interval = 300
+
+## Timeout for giving up on a kernel (in seconds).
+#  
+#  On starting and restarting kernels, we check whether the kernel is running and
+#  responsive by sending kernel_info_requests. This sets the timeout in seconds
+#  for how long the kernel can take before being presumed dead.  This affects the
+#  MappingKernelManager (which handles kernel restarts)  and the
+#  ZMQChannelsHandler (which handles the startup).
+#c.MappingKernelManager.kernel_info_timeout = 60
+
+## 
+#c.MappingKernelManager.root_dir = ''
+
+#------------------------------------------------------------------------------
+# ContentsManager(LoggingConfigurable) configuration
+#------------------------------------------------------------------------------
+
+## Base class for serving files and directories.
+#  
+#  This serves any text or binary file, as well as directories, with special
+#  handling for JSON notebook documents.
+#  
+#  Most APIs take a path argument, which is always an API-style unicode path, and
+#  always refers to a directory.
+#  
+#  - unicode, not url-escaped
+#  - '/'-separated
+#  - leading and trailing '/' will be stripped
+#  - if unspecified, path defaults to '',
+#    indicating the root path.
+
+## Allow access to hidden files
+#c.ContentsManager.allow_hidden = False
+
+## 
+#c.ContentsManager.checkpoints = None
+
+## 
+#c.ContentsManager.checkpoints_class = 'notebook.services.contents.checkpoints.Checkpoints'
+
+## 
+#c.ContentsManager.checkpoints_kwargs = {}
+
+## handler class to use when serving raw file requests.
+#  
+#  Default is a fallback that talks to the ContentsManager API, which may be
+#  inefficient, especially for large files.
+#  
+#  Local files-based ContentsManagers can use a StaticFileHandler subclass, which
+#  will be much more efficient.
+#  
+#  Access to these files should be Authenticated.
+#c.ContentsManager.files_handler_class = 'notebook.files.handlers.FilesHandler'
+
+## Extra parameters to pass to files_handler_class.
+#  
+#  For example, StaticFileHandlers generally expect a `path` argument specifying
+#  the root directory from which to serve files.
+#c.ContentsManager.files_handler_params = {}
+
+## Glob patterns to hide in file and directory listings.
+#c.ContentsManager.hide_globs = ['__pycache__', '*.pyc', '*.pyo', '.DS_Store', '*.so', '*.dylib', '*~']
+
+## Python callable or importstring thereof
+#  
+#  To be called on a contents model prior to save.
+#  
+#  This can be used to process the structure, such as removing notebook outputs
+#  or other side effects that should not be saved.
+#  
+#  It will be called as (all arguments passed by keyword)::
+#  
+#      hook(path=path, model=model, contents_manager=self)
+#  
+#  - model: the model to be saved. Includes file contents.
+#    Modifying this dict will affect the file that is stored.
+#  - path: the API path of the save destination
+#  - contents_manager: this ContentsManager instance
+#c.ContentsManager.pre_save_hook = None
+
+## 
+#c.ContentsManager.root_dir = '/'
+
+## The base name used when creating untitled directories.
+#c.ContentsManager.untitled_directory = 'Untitled Folder'
+
+## The base name used when creating untitled files.
+#c.ContentsManager.untitled_file = 'untitled'
+
+## The base name used when creating untitled notebooks.
+#c.ContentsManager.untitled_notebook = 'Untitled'
+
+#------------------------------------------------------------------------------
+# FileManagerMixin(Configurable) configuration
+#------------------------------------------------------------------------------
+
+## Mixin for ContentsAPI classes that interact with the filesystem.
+#  
+#  Provides facilities for reading, writing, and copying both notebooks and
+#  generic files.
+#  
+#  Shared by FileContentsManager and FileCheckpoints.
+#  
+#  Note ---- Classes using this mixin must provide the following attributes:
+#  
+#  root_dir : unicode
+#      A directory against against which API-style paths are to be resolved.
+#  
+#  log : logging.Logger
+
+## By default notebooks are saved on disk on a temporary file and then if
+#  succefully written, it replaces the old ones. This procedure, namely
+#  'atomic_writing', causes some bugs on file system whitout operation order
+#  enforcement (like some networked fs). If set to False, the new notebook is
+#  written directly on the old one which could fail (eg: full filesystem or quota
+#  )
+#c.FileManagerMixin.use_atomic_writing = True
+
+#------------------------------------------------------------------------------
+# FileContentsManager(FileManagerMixin,ContentsManager) configuration
+#------------------------------------------------------------------------------
+
+## If True (default), deleting files will send them to the platform's
+#  trash/recycle bin, where they can be recovered. If False, deleting files
+#  really deletes them.
+#c.FileContentsManager.delete_to_trash = True
+
+## Python callable or importstring thereof
+#  
+#  to be called on the path of a file just saved.
+#  
+#  This can be used to process the file on disk, such as converting the notebook
+#  to a script or HTML via nbconvert.
+#  
+#  It will be called as (all arguments passed by keyword)::
+#  
+#      hook(os_path=os_path, model=model, contents_manager=instance)
+#  
+#  - path: the filesystem path to the file just written - model: the model
+#  representing the file - contents_manager: this ContentsManager instance
+#c.FileContentsManager.post_save_hook = None
+
+## 
+#c.FileContentsManager.root_dir = ''
+
+## DEPRECATED, use post_save_hook. Will be removed in Notebook 5.0
+#c.FileContentsManager.save_script = False
+
+#------------------------------------------------------------------------------
+# NotebookNotary(LoggingConfigurable) configuration
+#------------------------------------------------------------------------------
+
+## A class for computing and verifying notebook signatures.
+
+## The hashing algorithm used to sign notebooks.
+#c.NotebookNotary.algorithm = 'sha256'
+
+## The sqlite file in which to store notebook signatures. By default, this will
+#  be in your Jupyter data directory. You can set it to ':memory:' to disable
+#  sqlite writing to the filesystem.
+#c.NotebookNotary.db_file = ''
+
+## The secret key with which notebooks are signed.
+#c.NotebookNotary.secret = b''
+
+## The file where the secret key is stored.
+#c.NotebookNotary.secret_file = ''
+
+## A callable returning the storage backend for notebook signatures. The default
+#  uses an SQLite database.
+#c.NotebookNotary.store_factory = traitlets.Undefined
+
+#------------------------------------------------------------------------------
+# KernelSpecManager(LoggingConfigurable) configuration
+#------------------------------------------------------------------------------
+
+## If there is no Python kernelspec registered and the IPython kernel is
+#  available, ensure it is added to the spec list.
+#c.KernelSpecManager.ensure_native_kernel = True
+
+## The kernel spec class.  This is configurable to allow subclassing of the
+#  KernelSpecManager for customized behavior.
+#c.KernelSpecManager.kernel_spec_class = 'jupyter_client.kernelspec.KernelSpec'
+
+## Whitelist of allowed kernel names.
+#  
+#  By default, all installed kernels are allowed.
+#c.KernelSpecManager.whitelist = set()
+
+
```

### Comparing `quanturf-8.5/quanturf.egg-info/PKG-INFO` & `quanturf-8.6/quanturf.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-Metadata-Version: 2.1
-Name: quanturf
-Version: 8.5
-Summary: REMOTE_USER Authenticator: An Authenticator for Jupyterhub to read user information from HTTP request headers, as when running behind an authenticating proxy.
-Home-page: https://github.com/Quanturf/quanturf_pypi_package.git
-Author: Quanturf
-Author-email: quanturf.finance@gmail.com
-License: GPLv3
-Keywords: Interactive,Interpreter,Shell,Web
-Platform: Linux
-Platform: Mac OS X
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: quanturf
+Version: 8.6
+Summary: REMOTE_USER Authenticator: An Authenticator for Jupyterhub to read user information from HTTP request headers, as when running behind an authenticating proxy.
+Home-page: https://github.com/Quanturf/quanturf_pypi_package.git
+Author: Quanturf
+Author-email: quanturf.finance@gmail.com
+License: GPLv3
+Keywords: Interactive,Interpreter,Shell,Web
+Platform: Linux
+Platform: Mac OS X
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+License-File: LICENCE.txt
```
