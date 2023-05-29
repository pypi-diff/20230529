# Comparing `tmp/t8s-0.1.7.tar.gz` & `tmp/t8s-0.1.8.tar.gz`

## Comparing `t8s-0.1.7.tar` & `t8s-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,37 @@
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 t8s-0.1.7/main.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 t8s-0.1.7/publish-to-pypi.md
--rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 t8s-0.1.7/test-all.sh
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 t8s-0.1.7/.github/workflows/test.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 t8s-0.1.7/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0    11376 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/304549b72d184314
--rw-r--r--   0        0        0    14953 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/37e53140500f6132
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/3efc7ff997958a2f
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/6a6461ff9108736
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/81d77b98d62a2ea
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/b9b8e13161c902cd
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/d3d5adf6aba338ae
--rw-r--r--   0        0        0    13104 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/dbd4b6248442ea85
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/e1951fc7d1998d8f
--rw-r--r--   0        0        0    26490 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/e7c8c0f9acb696e4
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 t8s-0.1.7/.ruff_cache/content/ebb21a9ed88aaaf2
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 t8s-0.1.7/.vscode/launch.json
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 t8s-0.1.7/docs/dp-strategy.md
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 t8s-0.1.7/docs/img/strategy-pattern.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 t8s-0.1.7/src/stubs/.gitkeep
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/__about__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/__init__.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/log_config.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/node.py
--rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/ts.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/ts_builder.py
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 t8s-0.1.7/src/t8s/ts_writer.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 t8s-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 t8s-0.1.7/tests/test_build_from_file.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 t8s-0.1.7/tests/test_to_parquet.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 t8s-0.1.7/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 t8s-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 t8s-0.1.7/README.md
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 t8s-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 t8s-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 t8s-0.1.8/.dockerignore
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 t8s-0.1.8/Dockerfile
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 t8s-0.1.8/constraints.txt
+-rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 t8s-0.1.8/dockerize.sh
+-rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 t8s-0.1.8/main.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 t8s-0.1.8/publish-to-pypi.md
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 t8s-0.1.8/smoke.py
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 t8s-0.1.8/test-all.sh
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 t8s-0.1.8/ts_01.csv
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 t8s-0.1.8/wfw-dev.sh
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 t8s-0.1.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 t8s-0.1.8/.vscode/launch.json
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/dp-composite.md
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/dp-singleton.md
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/dp-strategy.md
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/img/composite-pattern.png
+-rw-r--r--   0        0        0     6915 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/img/singleton-pattern.png
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 t8s-0.1.8/docs/img/strategy-pattern.png
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 t8s-0.1.8/src/patterns/chain.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 t8s-0.1.8/src/patterns/composite.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 t8s-0.1.8/src/patterns/node.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 t8s-0.1.8/src/stubs/.gitkeep
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/__about__.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/__init__.py
+-rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/io.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/log_config.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/ts.py
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/ts_builder.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 t8s-0.1.8/src/t8s/ts_writer.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 t8s-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 t8s-0.1.8/tests/test_build_from_file.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 t8s-0.1.8/tests/test_to_parquet.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 t8s-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 t8s-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 t8s-0.1.8/README.md
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 t8s-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 t8s-0.1.8/PKG-INFO
```

### Comparing `t8s-0.1.7/main.py` & `t8s-0.1.8/smoke.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,50 +21,60 @@
     # initialize_logger(INFO)
     logger.info('t8s package version:' + t8s.__version__)
     path_str: str = 'ts_01.parquet'
     path = Path(path_str)
     # Cria uma série temporal multivariada com três atributos: timestamp, temperatura e velocidade
     data = {
         'timestamp': [
-            datetime(2022, 1, 1, 0, 0, 0), 
+            datetime(2022, 1, 1, 0, 0, 0),
             datetime(2022, 1, 1, 1, 0, 0),
-            datetime(2022, 1, 1, 2, 0, 0), 
-            datetime(2022, 1, 1, 3, 0, 0)],
+            datetime(2022, 1, 1, 2, 0, 0),
+            datetime(2022, 1, 1, 3, 0, 0),
+        ],
         'temperatura': np.array([25.0, 26.0, 27.0, 23.2], dtype=np.float32),
-        'velocidade': [2000, 1100, 1200, 4000]
+        'velocidade': [2000, 1100, 1200, 4000],
     }
-    # Convertendo os tipos de dado para temperatura e velocidade para 
+    # Convertendo os tipos de dado para temperatura e velocidade para
     # np.float32 e np.int32 respectivamente, pois o padrão é np.float64 e np.int64
     data['temperatura'] = np.array(data['temperatura'], dtype=np.float32)
     data['velocidade'] = np.array(data['velocidade'], dtype=np.int32)
     # Cria uma série temporal multivariada com três atributos: timestamp, temperatura e
     # velocidade para o proposito de teste
-    ts = TimeSerie(data, format='wide', features_qty = 3)
+    ts = TimeSerie(data, format='wide', features_qty=3)
     cols_str = [name for name in sorted(ts.df.columns)]
     cols_str = ', '.join(cols_str)
     logger.info(f'Dataframe com {len(ts.df.columns)} colunas: {cols_str}')
     # Faz o display da série temporal no terminal
     print(ts)
+
+    # --------------------------------------------------------------------------------
+
     # Grava a série temporal em parquet
     print(f'Grava a série temporal (formato {ts.format}) em um arquivo parquet {path}')
     context = TSWriter(WriteParquetFile())
     print("Client: Strategy was seted to write Parquet file.")
     context.write(Path(path_str), ts)
     print(f'\nArquivo {str(path)} gerado à partir da TimeSerie fornecida')
+
     # --------------------------------------------------------------------------------
+
+    # Lê a série temporal gravada no arquivo parquet e gera uma nova série temporal
+    # com os respectivos Metadados e Schema. Ao final verifica se os tipos de dados
+    # foram lidos corretamente com o módulo assert.
+
     # Limpando objeto ts para garantir que será lido corretamente.
     ts: TimeSerie = TSBuilder.empty()
     # Lê a série temporal gravada no arquivo parquet
     print(f'\nLendo path {str(path)} e gerando TimeSerie')
-    
+
     # The client code picks a concrete strategy and passes it to the context.
     # The client should be aware of the differences between strategies in order
     # to make the right choice.
     assert isinstance(path, Path), "path must be a Path object"
-    if  (str(path)).endswith('.parquet'):
+    if (str(path)).endswith('.parquet'):
         context = TSBuilder(ReadParquetFile())
         print("Client: ReadStrategy is set to read Parquet file.")
         ts = context.build_from_file(Path(path_str))
     else:
         assert str(path).endswith('.csv'), "If path is not a Parquet file the path must be a CSV file"
         print("Client: ReadStrategy is set to read CSV file.")
         context = TSBuilder(ReadCsvFile())
@@ -89,7 +99,10 @@
         print(ts_uni)
         print('---------------------------------------------------')
 
     print('\nAgora posso fazer o join das séries temporais univariadas')
     ts = TimeSerie.join(univariate_list)
     print("\n\nTimeSerie multivariada, ts:\n")
     print(ts)
+
+    # --------------------------------------------------------------------------------
+
```

### Comparing `t8s-0.1.7/publish-to-pypi.md` & `t8s-0.1.8/publish-to-pypi.md`

 * *Files identical despite different names*

### Comparing `t8s-0.1.7/.github/workflows/test.yml` & `t8s-0.1.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `t8s-0.1.7/docs/dp-strategy.md` & `t8s-0.1.8/docs/dp-strategy.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Design Pattern used 
+# Design Pattern used: Strategy
 
 As transformações executadas na `TimeSerie` são implementadas usando o padrão de projeto `Strategy`.
 
 ![strategy design pattern](img/strategy-pattern.png)
 
 1. O `Context` mantém uma referência a uma das estratégias concretas e se comunica com esse objeto
 apenas por meio da interface da estratégia.
```

### Comparing `t8s-0.1.7/docs/img/strategy-pattern.png` & `t8s-0.1.8/docs/img/strategy-pattern.png`

 * *Files identical despite different names*

### Comparing `t8s-0.1.7/src/t8s/ts.py` & `t8s-0.1.8/src/t8s/ts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+# -*- coding: utf-8 -*-
+
 from pathlib import Path
 from datetime import datetime
 import yaml
 from abc import ABC, abstractmethod
-from typing import Any, Optional, TypeVar
+from typing import Any, Optional, Type, TypeVar
 
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 from t8s.log_config import LogConfig
 
@@ -14,22 +16,24 @@
 
 logger = LogConfig().getLogger()
 
 TS = TypeVar('TS', bound='TimeSerie')
 
 # ts = pd.read_parquet('lixo.parquet', engine='pyarrow')
 
+
 # Classe abstrata que define a interface para os processamentos de séries temporais
 class ITimeSeriesProcessor(ABC):
     def __init__(self):
         self.format: str
         self.features: str
         self.df: pd.DataFrame
 
     """Converte a série temporal para o formato Long"""
+
     @abstractmethod
     def to_long(self) -> bool:
         return False
 
     @abstractmethod
     def to_wide(self) -> bool:
         # Converte a série temporal para o formato Wide
@@ -42,81 +46,89 @@
 
     @abstractmethod
     def is_multivariate(self) -> bool:
         # Verifica se a série temporal é multivariada
         return False
 
     @abstractmethod
-    def split(self) -> list['TimeSerie']: # Alternativa: list[Optional['TimeSerie']]
+    def split(self) -> list[Type['TimeSerie']]:
+        # Alternativas para anotar o tipo de retorno:
+        # list[TS], list['TimeSerie'] ou list[Optional['TimeSerie']]
         # Cria várias séries temporais univariadas à partir de uma série temporal multivariada
         pass
 
     # @staticmethod
     # @abstractmethod
     # def join(list_of_ts: list['TimeSerie']) -> TS:
     #     pass
 
+
 """Rastreia a proveniência dos ativos de informação, Série Temporal neste caso"""
+
+
 class IProvenancable(ABC):
     def __init__(self):
         self.format: str
         self.features: str
         self.df: pd.DataFrame
 
     """Este método adiciona informações de proveniência ao objeto TimeSerie para 
     uma transformação específica. Ele recebe como parâmetros o nome da transformação 
     e um dicionário com os parâmetros usados na transformação."""
+
     @abstractmethod
-    def add_provenance(self, transformation: str, parameters: dict): 
-        pass 
-    
+    def add_provenance(self, transformation: str, parameters: dict):
+        pass
+
     @abstractmethod
-    def get_provenances(self) -> list[dict[str, Any]]: 
-        """Este método retorna uma lista de dicionários com as informações de 
+    def get_provenances(self) -> list[dict[str, Any]]:
+        """Este método retorna uma lista de dicionários com as informações de
         proveniência de todas as transformações realizadas no objeto TimeSerie."""
         pass
 
     @abstractmethod
-    def get_provenance_by_transformation(self, transformation: str) -> dict[str, Any]: 
-        """Este método retorna as informações de proveniência de uma dada transformação 
+    def get_provenance_by_transformation(self, transformation: str) -> dict[str, Any]:
+        """Este método retorna as informações de proveniência de uma dada transformação
         realizadas no objeto TimeSerie."""
         pass
 
     @abstractmethod
-    def get_last_transformation(self, transformation: str) -> dict[str, Any]: 
+    def get_last_transformation(self, transformation: str) -> dict[str, Any]:
         """Este método retorna informações da ultima transformação realizada no objeto TimeSerie."""
         pass
 
     @abstractmethod
-    def apply_transformation(self, transformation: str, **kwargs) -> Any : 
-        """Este método aplica uma transformação ao objeto TimeSerie e retorna um novo 
-        objeto TimeSerie com as informações de proveniência atualizadas. Ele recebe como 
+    def apply_transformation(self, transformation: str, **kwargs) -> Any:
+        """Este método aplica uma transformação ao objeto TimeSerie e retorna um novo
+        objeto TimeSerie com as informações de proveniência atualizadas. Ele recebe como
         parâmetros o nome da transformação e os parâmetros específicos da transformação."""
         pass
 
+
 class ITimeSerie(ITimeSeriesProcessor, IProvenancable):
     """
     Interface que estende as outras interfaces. ë apenas uma Marker Interface
     """
     pass
 
+
 class TimeSerie(ITimeSerie):
     def __init__(self, *args, format, features_qty, **kwargs):
         assert isinstance(format, str), "format must be a string"
         assert isinstance(features_qty, int), "features_qty must be a int"
         assert format in ['long', 'wide'], "format must be 'long' or 'wide'"
         self.format: str = format
         self.features: str = str(features_qty)
         self.df = pd.DataFrame(*args, **kwargs)
         # TODO: garantir que a primeira coluna seja um Timestamp quando o formato for long ou wide
 
     def __repr__(self):
         # Retorna uma representação em string do objeto TimeSerie
         return f'TimeSerie(format={self.format}, features={self.features}, df=\n{self.df.__repr__()})'
-        
+
     def to_long(self):
         # Converte a série temporal para o formato Long
         # Implementação aqui
         raise NotImplementedError('Not implemented for long format')
 
     def to_wide(self):
         # Converte a série temporal para o formato Wide
@@ -131,30 +143,30 @@
 
     def is_multivariate(self):
         # Verifica se a série temporal é multivariada
         if self.format == 'long':
             raise NotImplementedError('Not implemented for long format')
         return self.df.columns.size > 2
 
-    def split(self) -> list['TimeSerie']:
+    def split(self) -> list[TS]:  # Alternativa: list['TimeSerie']
         # TODO: garantir que a primeira coluna seja o indice no Dataframe quando o formato for long ou wide
         # TODO: garantir que a primeira coluna seja do tipo Timesamp (datetime) quando o formato for long ou wide
         # Cria várias séries temporais univariadas à partir de uma série temporal multivariada
         result = []
         if self.format == 'long':
-            # TODO: Implementar para o caso de formato longo.  
+            # TODO: Implementar para o caso de formato longo.
             pass
         elif self.format == 'wide':
             # Por contrato a primeira coluna é sempre o timestamp
             timestamp_col = self.df.columns[0]
             for idx, col in enumerate(self.df.columns):
                 if idx == 0:
                     continue
                 my_df = self.df[[timestamp_col, col]]
-                # TODO: criar um novo objeto TimeSerie 
+                # TODO: criar um novo objeto TimeSerie
                 my_ts = TimeSerie(data=my_df, format='wide', features_qty=2)
                 logger.debug('---------------------------------------------------')
                 logger.debug(f'univariate {idx}' + '\n ' + str(my_df))
                 result.append(my_ts)
         else:
             raise Exception('Formato de série temporal não suportado')
 
@@ -179,15 +191,15 @@
             assert list_of_ts[0].format == 'wide', 'A série temporal deve estar no formato wide'
             assert list_of_ts[0].features == 2, 'A série temporal univariada deve ter apenas 2 features'
             assert list_of_ts[0].is_univariate(), 'A série temporal deve ser univariada'
             # Garantindo que a primeira coluna seja o indice no Dataframe quando o formato for long ou wide
             if (list_of_ts[0].df).index.name == 'None':
                 (list_of_ts[0].df).set_index(timestamp_column_name, inplace=True)
             return list_of_ts[0]
-        
+
         # Junta os dataframes em uma série temporal multivariada
         if not isinstance(multivariate_df[timestamp_column_name][0], datetime):
             # Se a coluna timestamp não for do tipo datetime, converter para datetime.
             # Alternativamente podemeos usar o método astype(datetime) que faz o cast.
             multivariate_df[timestamp_column_name] = pd.to_datetime(multivariate_df[timestamp_column_name])
 
         for idx, ts in enumerate(list_of_ts):
@@ -202,51 +214,51 @@
         # Ao final crio a série temporal multivariada usando a lista de univariadas
         features_qty = multivariate_df.columns.size
         multivariate_ts = TimeSerie(format='wide', features_qty=features_qty, data=multivariate_df)
 
         # Garantindo que a primeira coluna seja o indice no Dataframe quando o formato for long ou wide
         # Define a primeira coluna como índice do dataframe, caso já não seja
         if (multivariate_ts.df).index.name == 'None':
-                (multivariate_ts.df).set_index(timestamp_column_name, inplace=True)
+            (multivariate_ts.df).set_index(timestamp_column_name, inplace=True)
         multivariate_ts.df.set_index(timestamp_column_name, inplace=True)
 
         # Imprime a série temporal multivariada
         logger.debug(multivariate_ts)
         return multivariate_ts
 
     ### ----------------------------- Métodos de IProvenancable ----------------------------------
 
     def add_provenance(self, transformation: str, parameters: dict):
-        # Este método adiciona informações de proveniência ao objeto TimeSerie para 
-        # uma transformação específica. Ele recebe como parâmetros o nome da transformação 
+        # Este método adiciona informações de proveniência ao objeto TimeSerie para
+        # uma transformação específica. Ele recebe como parâmetros o nome da transformação
         # e um dicionário com os parâmetros usados na transformação.
         # TODO: Implementar add_provenance()
         pass
 
     def get_provenances(self) -> list[dict[str, Any]]:
-        # Este método retorna uma lista de dicionários com as informações de 
+        # Este método retorna uma lista de dicionários com as informações de
         # proveniência de todas as transformações realizadas no objeto TimeSerie.
         # TODO: Implementar get_provenances()
         return []
 
     def get_provenance_by_transformation(self, transformation: str) -> dict[str, Any]:
-        # Este método retorna as informações de proveniência de uma dada transformação 
+        # Este método retorna as informações de proveniência de uma dada transformação
         # realizadas no objeto TimeSerie.
         # TODO: Implementar get_provenance_by_transformation()
         return {}
 
     def get_last_transformation(self, transformation: str) -> dict[str, Any]:
         # TODO: Implementar get_provenance_by_transformation()
         return {}
 
-    def apply_transformation(self, transformation: str, **kwargs) -> Optional['TimeSerie']: 
-        """Este método aplica uma transformação ao objeto TimeSerie e retorna um novo 
-        objeto TimeSerie com as informações de proveniência atualizadas. Ele recebe como 
+    def apply_transformation(self, transformation: str, **kwargs) -> Optional['TimeSerie']:
+        """Este método aplica uma transformação ao objeto TimeSerie e retorna um novo
+        objeto TimeSerie com as informações de proveniência atualizadas. Ele recebe como
         parâmetros o nome da transformação e os parâmetros específicos da transformação."""
         # TODO: Implementar apply_transformation()
         return TimeSerie.empty()
-    
+
     ### ------------------------- Outros Métodos Estáticos da classe -----------------------------
 
     @staticmethod
     def empty() -> Any:
         return TimeSerie(format='long', features_qty=0, data={})
```

### Comparing `t8s-0.1.7/src/t8s/ts_builder.py` & `t8s-0.1.8/src/t8s/ts_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 # from __future__ import annotations usado apenas nas versões anteriores a 3.7
 from abc import ABC, abstractmethod
 from typing import Any, Optional
 from pathlib import Path
 from datetime import datetime
 from t8s.log_config import LogConfig
-from t8s.ts import TimeSerie # , ITimeSerie, ITimeSeriesProcessor, IProvenancable
+from t8s.ts import TimeSerie  # , ITimeSerie, ITimeSeriesProcessor, IProvenancable
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 logger = LogConfig().getLogger()
 
+
 class ReadStrategy(ABC):
     """
     The Strategy interface declares operations common to all supported versions
     of some algorithm.
 
     The Context uses this interface to call the algorithm defined by Concrete
     Strategies.
@@ -28,15 +29,16 @@
 
 
 """
 Concrete Strategies implement the algorithm while following the base Strategy
 interface. The interface makes them interchangeable in the Context.
 """
 
-class TSBuilder():
+
+class TSBuilder:
     """
     The Context defines the interface of interest to clients.
     """
 
     def __init__(self, strategy: ReadStrategy) -> None:
         """
         Usually, the Context accepts a strategy through the constructor, but
@@ -97,14 +99,15 @@
         # ...
         return result
 
     @staticmethod
     def empty() -> TimeSerie:
         return TimeSerie.empty()
 
+
 class ReadParquetFile(ReadStrategy):
     def do_read(self, data: Path) -> Optional['TimeSerie']:
         logger.info('Using ReadParquetFile strategy to read data from: ' + str(data))
         assert isinstance(data, Path), "path must be a Path object"
         assert (str(data)).endswith('.parquet'), "path must be a Path object"
         # Lê os metadados do arquivo Parquet
         metadata: pq.FileMetaData = pq.read_metadata(data)
@@ -133,16 +136,17 @@
         # Leia o arquivo Parquet
         parquet_file = pq.ParquetFile(data)
         logger.debug('\ntype(parquet_file): ' + str(type(parquet_file)) + '\n' + str(parquet_file))
         logger.debug('\n-------------------------------')
         df = pd.read_parquet(data)
         # TODO: garantir que a primeira coluna seja um Timestamp quando o formato for long ou wide
         logger.debug('\ndf:\n' + str(df))
-        # Cria o objeto 
+        # Cria o objeto
         ts = TimeSerie(df, format=format, features_qty=features_qty)
         logger.debug('\nts:\n' + str(ts))
         return ts
 
+
 class ReadCsvFile(ReadStrategy):
     def do_read(self, data: list) -> Optional['TimeSerie']:
         logger.info('Using ReadCsvFile strategy')
         return TSBuilder.empty()
```

### Comparing `t8s-0.1.7/src/t8s/ts_writer.py` & `t8s-0.1.8/src/t8s/ts_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from t8s.log_config import LogConfig
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 logger = LogConfig().getLogger()
 
+
 class Strategy(ABC):
     """
     The Strategy interface declares operations common to all supported versions
     of some algorithm.
 
     The Context uses this interface to call the algorithm defined by Concrete
     Strategies.
@@ -29,15 +30,16 @@
 
 
 """
 Concrete Strategies implement the algorithm while following the base Strategy
 interface. The interface makes them interchangeable in the Context.
 """
 
-class TSWriter():
+
+class TSWriter:
     """
     The Context defines the interface of interest to clients.
     """
 
     def __init__(self, strategy: Strategy) -> None:
         """
         Usually, the Context accepts a strategy through the constructor, but
@@ -75,58 +77,65 @@
         logger.info("Context: write")
         result = self._strategy.do_write(path, ts)
         # logger.info('result type from do_write() is: ' + str(type(result)))
 
         # ...
         return result
 
+
 class WriteParquetFile(Strategy):
     # O método do_write é VOID, pois o resultado é gravado em disco. Caso ocorra
     # algum problema uma `Exception` é lançada.
     def do_write(self, path: Path, ts: TimeSerie) -> None:
         logger.info('Using WriteParquetFile strategy')
         # Grava os dados em formato Parquet com metadados do objeto TimeSerie
         # to_parquet(path, df, self.format, self.features)
         table = pa.Table.from_pandas(ts.df)
         # table = table.replace_schema_metadata({'format': self.format, 'features': self.features})
-        table = table.replace_schema_metadata({
-            b'format': str(ts.format).encode(),
-            b'features': str(ts.features).encode()})
+        table = table.replace_schema_metadata(
+            {b'format': str(ts.format).encode(), b'features': str(ts.features).encode()}
+        )
         result = pq.write_table(table, path)
-        return result      
+        return result
+
 
 class WriteCsvFile(Strategy):
     # O método do_write é VOID, pois o resultado é gravado em disco. Caso ocorra
     # algum problema uma `Exception` é lançada.
     def do_write(self, path: Path, ts: TimeSerie) -> None:
         logger.info('Using WriteCsvFile strategy')
         return None
 
+
 if __name__ == "__main__":
     from logging import INFO, DEBUG
     import numpy as np
     import pandas as pd
     import subprocess
+
     LogConfig().initialize_logger(DEBUG)
     path_str: str = 'ts_01.parquet'
     path = Path(path_str)
     # Cria uma série temporal multivariada com três atributos: timestamp, temperatura e velocidade
     data = {
         'timestamp': [
-            datetime(2022, 1, 1, 0, 0, 0), datetime(2022, 1, 1, 1, 0, 0),
-            datetime(2022, 1, 1, 2, 0, 0), datetime(2022, 1, 1, 3, 0, 0)],
+            datetime(2022, 1, 1, 0, 0, 0),
+            datetime(2022, 1, 1, 1, 0, 0),
+            datetime(2022, 1, 1, 2, 0, 0),
+            datetime(2022, 1, 1, 3, 0, 0),
+        ],
         'temperatura': np.array([25.0, 26.0, 27.0, 23.2], dtype=np.float32),
-        'velocidade': np.array([2000, 1100, 1200, 4000], dtype=np.int32)
+        'velocidade': np.array([2000, 1100, 1200, 4000], dtype=np.int32),
     }
-    # Cria uma série temporal multivariada 
-    ts = TimeSerie(data, format='wide', features_qty = 3)
+    # Cria uma série temporal multivariada
+    ts = TimeSerie(data, format='wide', features_qty=3)
     # Grava a série temporal em parquet
     print(f'Grava a série temporal (formato {ts.format}) em um arquivo parquet {path}')
     (TSWriter(WriteParquetFile())).write(Path(path_str), ts)
     print(f'Arquivo {str(path)} gerado à partir da TimeSerie fornecida')
     #  Supondo o arquivo /usr/local/bin/lsla existindo no sistema com o conteudo abaixo:
     #  #!/bin/bash
-    # 
+    #
     #  ls -lA *.parquet
     #
     result = subprocess.run(['lsla'], capture_output=True, text=True)
     print(result.stdout)
```

### Comparing `t8s-0.1.7/tests/test_build_from_file.py` & `t8s-0.1.8/tests/test_build_from_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from datetime import datetime
 import numpy as np
 import pandas as pd
 from t8s.ts import TimeSerie
 from t8s.ts_builder import TSBuilder
 from t8s.ts_builder import ReadParquetFile
 
+
 def test_build_from_file():
     path_str: str = 'ts_01.parquet'
     path = Path(path_str)
     print('path: ', path)
     context = TSBuilder(ReadParquetFile())
     print("Client: Strategy is set to read Parquet file.")
     ts: TimeSerie = context.build_from_file(Path(path_str))
     assert int(ts.features) == 3
     assert ts.format == 'wide'
     assert ts.df.__len__() == 4
-     # pd._libs.tslibs.timestamps.Timestamp é privado e devo usar pd.Timestamp
+    # pd._libs.tslibs.timestamps.Timestamp é privado e devo usar pd.Timestamp
     assert type(ts.df['timestamp'][0]) == pd.Timestamp
     assert type(ts.df['temperatura'][0]) == np.float32
-    assert type(ts.df['velocidade'][0]) == np.int32
+    assert type(ts.df['velocidade'][0]) == np.int32
```

### Comparing `t8s-0.1.7/tests/test_to_parquet.py` & `t8s-0.1.8/tests/test_to_parquet.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 from pathlib import Path
 from datetime import datetime
 import numpy as np
 import pandas as pd
 from t8s.ts import TimeSerie
 from t8s.ts_writer import TSWriter, WriteParquetFile
 
+
 def test_to_parquet():
     path_str: str = 'ts_01.parquet'
     path = Path(path_str)
     # Cria uma série temporal multivariada com três atributos: timestamp, temperatura e velocidade
     data = {
         'timestamp': [
-            datetime(2022, 1, 1, 0, 0, 0), 
+            datetime(2022, 1, 1, 0, 0, 0),
             datetime(2022, 1, 1, 1, 0, 0),
-            datetime(2022, 1, 1, 2, 0, 0), 
-            datetime(2022, 1, 1, 3, 0, 0)],
+            datetime(2022, 1, 1, 2, 0, 0),
+            datetime(2022, 1, 1, 3, 0, 0),
+        ],
         'temperatura': [25.0, 26.0, 27.0, 23.2],
-        'velocidade': [2000, 1100, 1200, 4000]
+        'velocidade': [2000, 1100, 1200, 4000],
     }
-    # Convertendo os tipos de dado para temperatura e velocidade para 
+    # Convertendo os tipos de dado para temperatura e velocidade para
     # np.float32 e np.int32 respectivamente, pois o padrão é np.float64 e np.int64
     data['temperatura'] = np.array(data['temperatura'], dtype=np.float32)
     data['velocidade'] = np.array(data['velocidade'], dtype=np.int32)
     ts = TimeSerie(data, format='wide', features_qty=len(data))
     df = ts.df
     cols_str = [name for name in sorted(df.columns)]
     print('cols_str :', ', '.join(cols_str))
```

### Comparing `t8s-0.1.7/LICENSE.txt` & `t8s-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `t8s-0.1.7/README.md` & `t8s-0.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # t8s
 
 [![PyPI - Stable Version](https://img.shields.io/pypi/v/t8s.svg)](https://pypi.org/project/t8s)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/t8s.svg)](https://pypi.org/project/t8s)
-
 [![Downloads](https://img.shields.io/pypi/dm/t8s)](https://pypistats.org/packages/t8s)
 [![Build Status](https://github.com/joao-parana/t8s/actions/workflows/test.yml/badge.svg)](https://github.com/joao-parana/t8s/actions)
 [![Documentation Status](https://readthedocs.org/projects/t8s/badge/?version=latest)](https://t8s.readthedocs.io/en/latest/?badge=latest)
 
 -----
 
 **Table of Contents**
@@ -24,22 +23,23 @@
 
 Check Linter rules using **PyRight** (https://microsoft.github.io/pyright)
 
 ```bash
 pyright --level warning .
 ```
 
-## Testing
+## Testing and publishing
 
-```console
+```batch
 # Para inspecionar a configuração do ambiente de testes:
 hatch config show
 hatch clean
 hatch build
 # Edit your main.py code
 hatch run python3 main.py
 ./test-all.sh
+hatch publish
 ```
 
 ## License
 
 `t8s` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `t8s-0.1.7/pyproject.toml` & `t8s-0.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,26 @@
   "keyring",
   "keyrings.google-artifactregistry-auth",
   "pyyaml",
   "pyarrow",
   "pandas",
 ]
 
+[project.optional-dependencies]
+dev = [
+  "bandit",
+  "black",
+  "flake8",
+  "hatch",
+  "isort",
+  "pylint",
+  "pytest",
+  "pytest-timeout"
+]
+
 [project.urls]
 Documentation = "https://github.com/joao-parana/t8s#README.md"
 Issues = "https://github.com/joao-parana/t8s/issues"
 Source = "https://github.com/joao-parana/t8s"
 
 [tool.pyright]
 include = ["src"]
@@ -100,20 +112,20 @@
 ]
 all = [
   "style",
   "typing",
 ]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py310"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py310"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
```

### Comparing `t8s-0.1.7/PKG-INFO` & `t8s-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t8s
-Version: 0.1.7
+Version: 0.1.8
 Project-URL: Documentation, https://github.com/joao-parana/t8s#README.md
 Project-URL: Issues, https://github.com/joao-parana/t8s/issues
 Project-URL: Source, https://github.com/joao-parana/t8s
 Author-email: João Antonio Ferreira <joao.parana@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -15,21 +15,29 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: keyring
 Requires-Dist: keyrings-google-artifactregistry-auth
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
+Provides-Extra: dev
+Requires-Dist: bandit; extra == 'dev'
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
+Requires-Dist: pylint; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-timeout; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # t8s
 
 [![PyPI - Stable Version](https://img.shields.io/pypi/v/t8s.svg)](https://pypi.org/project/t8s)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/t8s.svg)](https://pypi.org/project/t8s)
-
 [![Downloads](https://img.shields.io/pypi/dm/t8s)](https://pypistats.org/packages/t8s)
 [![Build Status](https://github.com/joao-parana/t8s/actions/workflows/test.yml/badge.svg)](https://github.com/joao-parana/t8s/actions)
 [![Documentation Status](https://readthedocs.org/projects/t8s/badge/?version=latest)](https://t8s.readthedocs.io/en/latest/?badge=latest)
 
 -----
 
 **Table of Contents**
@@ -47,22 +55,23 @@
 
 Check Linter rules using **PyRight** (https://microsoft.github.io/pyright)
 
 ```bash
 pyright --level warning .
 ```
 
-## Testing
+## Testing and publishing
 
-```console
+```batch
 # Para inspecionar a configuração do ambiente de testes:
 hatch config show
 hatch clean
 hatch build
 # Edit your main.py code
 hatch run python3 main.py
 ./test-all.sh
+hatch publish
 ```
 
 ## License
 
 `t8s` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

