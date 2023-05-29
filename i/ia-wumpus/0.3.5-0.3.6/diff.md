# Comparing `tmp/ia_wumpus-0.3.5.tar.gz` & `tmp/ia_wumpus-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.3.5.tar", max compression
+gzip compressed data, was "ia_wumpus-0.3.6.tar", max compression
```

## Comparing `ia_wumpus-0.3.5.tar` & `ia_wumpus-0.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.5/LICENSE
--rw-r--r--   0        0        0     3921 2023-05-18 15:05:34.982478 ia_wumpus-0.3.5/README.md
--rw-r--r--   0        0        0      636 2023-05-28 14:43:13.018218 ia_wumpus-0.3.5/ia_wumpus/__init__.py
--rw-r--r--   0        0        0     8519 2023-05-28 19:13:54.450734 ia_wumpus-0.3.5/ia_wumpus/agente_reativo_v1.py
--rw-r--r--   0        0        0     8960 2023-05-28 19:01:53.341149 ia_wumpus-0.3.5/ia_wumpus/ambiente.py
--rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.5/ia_wumpus/dinamica_agente_ambiente.py
--rw-r--r--   0        0        0      511 2023-05-28 19:16:32.303392 ia_wumpus-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4575 1970-01-01 00:00:00.000000 ia_wumpus-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.6/LICENSE
+-rw-r--r--   0        0        0     3968 2023-05-29 00:28:22.597635 ia_wumpus-0.3.6/README.md
+-rw-r--r--   0        0        0      636 2023-05-29 00:29:36.243030 ia_wumpus-0.3.6/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     8481 2023-05-28 21:14:28.319582 ia_wumpus-0.3.6/ia_wumpus/agente_reativo_v1.py
+-rw-r--r--   0        0        0     8960 2023-05-28 19:01:53.341149 ia_wumpus-0.3.6/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.6/ia_wumpus/dinamica_agente_ambiente.py
+-rw-r--r--   0        0        0      511 2023-05-29 00:29:07.586488 ia_wumpus-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4622 1970-01-01 00:00:00.000000 ia_wumpus-0.3.6/PKG-INFO
```

### Comparing `ia_wumpus-0.3.5/LICENSE` & `ia_wumpus-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.5/README.md` & `ia_wumpus-0.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Ambiente para estudo de modelos de Apredizagem de Máquina da disciplina de Inteligência Computacional.
 
 <br>
 
 # Versões do Projeto
 
-<img src="https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/blob/main/utils/code_demo.png?raw=true" alt="Ambiente Mundo do Wumpus." style="width:900px">
+<img src="https://raw.githubusercontent.com/Oseiasdfarias/IA_mundo_do_wumpus/340951a7d59c7ce6e3c981455b77638781b23d52/docs/static/img/code_demo.svg" alt="Ambiente Mundo do Wumpus." style="width:900px">
 
 <br>
 
 ## [Link Versão 00](https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/tree/versao_0)
 
 **Etapa 1 - Gerador Aleatório de Ambientes do Mundo do Wumpus.**
```

### Comparing `ia_wumpus-0.3.5/ia_wumpus/__init__.py` & `ia_wumpus-0.3.6/ia_wumpus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # Data: Maio - 2023
 #  ----------------------------------------------------
 
 from .ambiente import Ambiente                   # noqa: F401
 from .agente_reativo_v1 import AgenteReativoV1   # noqa: F401
 
 
-__version__ = "0.3.3"
+__version__ = "0.3.6"
```

### Comparing `ia_wumpus-0.3.5/ia_wumpus/agente_reativo_v1.py` & `ia_wumpus-0.3.6/ia_wumpus/agente_reativo_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     def get_opcoes_mov(self) -> List:
         """
         Método responsável por obter as possíveis obções de movimentação
         do agente no ambiente.
         """
         pos_agente = self.amb.get_pos_objetos()["agente"][0]
         self.__opcoes_mov_agente(pos_agente=pos_agente)
-        print(self.__list_opc_mov_ag)
         return self.__list_opc_mov_ag
 
     def __opcoes_mov_agente(self, pos_agente: Tuple) -> None:
         """
             Verifica as possíveis opções de movimentação do agente
             para a posição atual.
         """
```

### Comparing `ia_wumpus-0.3.5/ia_wumpus/ambiente.py` & `ia_wumpus-0.3.6/ia_wumpus/ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.5/ia_wumpus/dinamica_agente_ambiente.py` & `ia_wumpus-0.3.6/ia_wumpus/dinamica_agente_ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.5/PKG-INFO` & `ia_wumpus-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.3.5
+Version: 0.3.6
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,15 +29,15 @@
 
 Ambiente para estudo de modelos de Apredizagem de Máquina da disciplina de Inteligência Computacional.
 
 <br>
 
 # Versões do Projeto
 
-<img src="https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/blob/main/utils/code_demo.png?raw=true" alt="Ambiente Mundo do Wumpus." style="width:900px">
+<img src="https://raw.githubusercontent.com/Oseiasdfarias/IA_mundo_do_wumpus/340951a7d59c7ce6e3c981455b77638781b23d52/docs/static/img/code_demo.svg" alt="Ambiente Mundo do Wumpus." style="width:900px">
 
 <br>
 
 ## [Link Versão 00](https://github.com/Oseiasdfarias/IA_mundo_do_wumpus/tree/versao_0)
 
 **Etapa 1 - Gerador Aleatório de Ambientes do Mundo do Wumpus.**
```

