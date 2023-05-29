# Comparing `tmp/graphdisplay-0.4.0.tar.gz` & `tmp/graphdisplay-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.4.0.tar", last modified: Tue May 16 18:18:49 2023, max compression
+gzip compressed data, was "graphdisplay-0.4.1.tar", last modified: Mon May 29 21:05:20 2023, max compression
```

## Comparing `graphdisplay-0.4.0.tar` & `graphdisplay-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.782601 graphdisplay-0.4.0/
--rw-rw-r--   0 beto      (1000) beto      (1000)     6167 2023-05-16 18:18:49.782601 graphdisplay-0.4.0/PKG-INFO
--rw-rw-r--   0 beto      (1000) beto      (1000)     5529 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/README.md
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.778601 graphdisplay-0.4.0/graphdisplay/
--rw-rw-r--   0 beto      (1000) beto      (1000)       98 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/__init__.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     1856 2023-05-16 17:19:06.000000 graphdisplay-0.4.0/graphdisplay/about_win_manager.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     4154 2023-05-16 18:18:44.000000 graphdisplay-0.4.0/graphdisplay/general_config.py
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.778601 graphdisplay-0.4.0/graphdisplay/graphs/
--rw-rw-r--   0 beto      (1000) beto      (1000)       24 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/graphs/__init__.py
--rw-rw-r--   0 beto      (1000) beto      (1000)    17021 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/graphs/graph.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     6977 2023-05-09 11:25:49.000000 graphdisplay-0.4.0/graphdisplay/json_manager.py
--rw-rw-r--   0 beto      (1000) beto      (1000)    27026 2023-05-16 15:34:14.000000 graphdisplay-0.4.0/graphdisplay/main.py
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.778601 graphdisplay-0.4.0/graphdisplay/store/
--rw-rw-r--   0 beto      (1000) beto      (1000)        0 2023-05-06 20:46:34.000000 graphdisplay-0.4.0/graphdisplay/store/__init__.py
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.782601 graphdisplay-0.4.0/graphdisplay/trees/
--rw-rw-r--   0 beto      (1000) beto      (1000)       87 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/trees/__init__.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     3524 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/trees/auto_balance_tree.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     3107 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/trees/binary_search_tree.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     5510 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/trees/binary_tree.py
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.778601 graphdisplay-0.4.0/graphdisplay.egg-info/
--rw-rw-r--   0 beto      (1000) beto      (1000)     6167 2023-05-16 18:18:49.000000 graphdisplay-0.4.0/graphdisplay.egg-info/PKG-INFO
--rw-rw-r--   0 beto      (1000) beto      (1000)      540 2023-05-16 18:18:49.000000 graphdisplay-0.4.0/graphdisplay.egg-info/SOURCES.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)        1 2023-05-16 18:18:49.000000 graphdisplay-0.4.0/graphdisplay.egg-info/dependency_links.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)       13 2023-05-16 18:18:49.000000 graphdisplay-0.4.0/graphdisplay.egg-info/top_level.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)       38 2023-05-16 18:18:49.782601 graphdisplay-0.4.0/setup.cfg
--rw-rw-r--   0 beto      (1000) beto      (1000)     1323 2023-05-16 16:42:51.000000 graphdisplay-0.4.0/setup.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-29 21:05:20.793090 graphdisplay-0.4.1/
+-rw-rw-r--   0 beto      (1000) beto      (1000)     5312 2023-05-29 21:05:20.793090 graphdisplay-0.4.1/PKG-INFO
+-rw-rw-r--   0 beto      (1000) beto      (1000)     4674 2023-05-18 10:09:21.000000 graphdisplay-0.4.1/README.md
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-29 21:05:20.789090 graphdisplay-0.4.1/graphdisplay/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       98 2023-05-14 22:04:49.000000 graphdisplay-0.4.1/graphdisplay/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     2097 2023-05-29 20:23:22.000000 graphdisplay-0.4.1/graphdisplay/about_win_manager.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     4990 2023-05-29 21:04:55.000000 graphdisplay-0.4.1/graphdisplay/general_config.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-29 21:05:20.789090 graphdisplay-0.4.1/graphdisplay/graphs/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       24 2023-05-14 22:04:49.000000 graphdisplay-0.4.1/graphdisplay/graphs/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    22479 2023-05-29 20:54:19.000000 graphdisplay-0.4.1/graphdisplay/graphs/graph.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     7503 2023-05-24 08:02:19.000000 graphdisplay-0.4.1/graphdisplay/json_manager.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    34848 2023-05-29 20:23:22.000000 graphdisplay-0.4.1/graphdisplay/main.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-29 21:05:20.789090 graphdisplay-0.4.1/graphdisplay/store/
+-rw-rw-r--   0 beto      (1000) beto      (1000)        0 2023-05-06 20:46:34.000000 graphdisplay-0.4.1/graphdisplay/store/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    16911 2023-05-29 20:34:03.000000 graphdisplay-0.4.1/graphdisplay/tools_win_manager.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-29 21:05:20.793090 graphdisplay-0.4.1/graphdisplay/trees/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       87 2023-05-14 22:04:49.000000 graphdisplay-0.4.1/graphdisplay/trees/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     3524 2023-05-14 22:04:49.000000 graphdisplay-0.4.1/graphdisplay/trees/auto_balance_tree.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     3160 2023-05-27 19:46:41.000000 graphdisplay-0.4.1/graphdisplay/trees/binary_search_tree.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     6026 2023-05-28 11:58:14.000000 graphdisplay-0.4.1/graphdisplay/trees/binary_tree.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-29 21:05:20.789090 graphdisplay-0.4.1/graphdisplay.egg-info/
+-rw-rw-r--   0 beto      (1000) beto      (1000)     5312 2023-05-29 21:05:20.000000 graphdisplay-0.4.1/graphdisplay.egg-info/PKG-INFO
+-rw-rw-r--   0 beto      (1000) beto      (1000)      574 2023-05-29 21:05:20.000000 graphdisplay-0.4.1/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)        1 2023-05-29 21:05:20.000000 graphdisplay-0.4.1/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)       13 2023-05-29 21:05:20.000000 graphdisplay-0.4.1/graphdisplay.egg-info/top_level.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)       38 2023-05-29 21:05:20.793090 graphdisplay-0.4.1/setup.cfg
+-rw-rw-r--   0 beto      (1000) beto      (1000)     1323 2023-05-16 16:42:51.000000 graphdisplay-0.4.1/setup.py
```

### Comparing `graphdisplay-0.4.0/PKG-INFO` & `graphdisplay-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.4.0
+Version: 0.4.1
 Summary: Librería para representar visualmente grafos de tipo diccionario
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -30,23 +30,23 @@
 ## Método de uso 
 
 Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
 tkinter y math (que muchas veces vienen instaladas por defecto en python). 
 
 Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
 para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
-para una mejor visualización. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
+para una mejor visualización. **Al desplazar los vértices por la pantalla y fijar su posición, si se cierra la ventana y se vuelve a abrir, el grafo seguirá con la forma con la que se ha movido
+antes.**. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
 grafos grandes y complejos:
 + graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
 de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
 implementación de grafos que viene por defecto con el paquete.
 + node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
 + scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
 + scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-+ theme: el tema de la ventana, por defecto es 'brown' y no voy a mencionarlos todos porque hay muchos y me da pereza.
 
 Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
 ```python
 g = Graph([1, 2, 3])
 g.addEdge(1, 2)
 g.addEdge(2, 3)
 
@@ -57,23 +57,16 @@
 GraphGUI(g, 32, 700, 700)
 
 # Para ajustar únicamente el ancho de la pantalla a 200 píxeles
 GraphGUI(g, scr_width=200)
 ```
 
 Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
-argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `addEdge`, con los vértices que conecta la arista además del valor/coste de la arista.
+argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `add_edge`, con los vértices que conecta la arista además del valor/coste de la arista.
 
-## Funcionalidades
-Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
-éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
-instaciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
-Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
-tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón save y nombrando el guardado) para
-después poder cargarlo en cualquier momento.
 ## Ejemplo de uso
 
 Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
 
 ```python
 labels = ['A', 'B', 'C', 'D', 'E']
 g = Graph(labels)
```

### Comparing `graphdisplay-0.4.0/README.md` & `graphdisplay-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 ## Método de uso 
 
 Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
 tkinter y math (que muchas veces vienen instaladas por defecto en python). 
 
 Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
 para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
-para una mejor visualización. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
+para una mejor visualización. **Al desplazar los vértices por la pantalla y fijar su posición, si se cierra la ventana y se vuelve a abrir, el grafo seguirá con la forma con la que se ha movido
+antes.**. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
 grafos grandes y complejos:
 + graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
 de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
 implementación de grafos que viene por defecto con el paquete.
 + node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
 + scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
 + scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-+ theme: el tema de la ventana, por defecto es 'brown' y no voy a mencionarlos todos porque hay muchos y me da pereza.
 
 Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
 ```python
 g = Graph([1, 2, 3])
 g.addEdge(1, 2)
 g.addEdge(2, 3)
 
@@ -40,23 +40,16 @@
 GraphGUI(g, 32, 700, 700)
 
 # Para ajustar únicamente el ancho de la pantalla a 200 píxeles
 GraphGUI(g, scr_width=200)
 ```
 
 Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
-argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `addEdge`, con los vértices que conecta la arista además del valor/coste de la arista.
+argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `add_edge`, con los vértices que conecta la arista además del valor/coste de la arista.
 
-## Funcionalidades
-Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
-éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
-instaciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
-Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
-tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón save y nombrando el guardado) para
-después poder cargarlo en cualquier momento.
 ## Ejemplo de uso
 
 Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
 
 ```python
 labels = ['A', 'B', 'C', 'D', 'E']
 g = Graph(labels)
```

### Comparing `graphdisplay-0.4.0/graphdisplay/about_win_manager.py` & `graphdisplay-0.4.1/graphdisplay/about_win_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     def __init__(self, root, graphgui):
         super().__init__(root)
         self.__graphgui = graphgui
         self.title("About")
         self.geometry("400x430")
         self.resizable(False, False)
         self.configure(bg=self.__graphgui._FRAME_COLOR, width=400, height=430)
+        self.protocol("WM_DELETE_WINDOW", self.__on_close)
 
         buton = tk.Button(self, text="Contribute", bg=self.__graphgui._BUTTON_COLOR, command=self.__open_github, bd=0)
         buton.pack(side=tk.BOTTOM)
 
         self.canvas = tk.Canvas(self, width=400, height=400, bg=self.__graphgui._BACKGROUND_CANVAS_COLOR)
         self.canvas.pack()
         self.turtle = turtle.RawTurtle(self.canvas, visible=False)
@@ -23,21 +24,29 @@
         text = "GraphDisplay v"+VERSION
         self.canvas.create_text(0, -150, text=text, font=("Courier", 20),
                                 fill=self.__graphgui._AUTHOR_NAME_COLOR)
         self.canvas.create_text(0, 147, text="An open source proyect made", font=("Courier", 13),
                                 fill=self.__graphgui._AUTHOR_NAME_COLOR)
         self.canvas.create_text(0, 165, text="by and for students!", font=("Courier", 13),
                                 fill=self.__graphgui._AUTHOR_NAME_COLOR)
-        for i in range(92):
+        self.running = True
+        i = 0
+        self.turtle.color(self.__graphgui._VERTEX_COLOR)
+        while self.running and i<92:
             if i % 2 == 0:
                 self.turtle.penup()
             else:
                 self.turtle.pendown()
-                self.turtle.color(self.__graphgui._VERTEX_COLOR)
-            self.turtle.forward(i+1+5)
-            self.turtle.right(91)
+            if self.running:
+                self.turtle.forward(i + 1 + 5)
+                self.turtle.right(91)
+            i += 1
+
+    def __on_close(self):
+        self.running = False
+        self.destroy()
 
     def __open_github(self):
         webbrowser.open("https://github.com/seniorbeto/graphdisplay")
 
     def __open_twitter(self):
         webbrowser.open("https://twitter.com/seniorbeto__")
```

### Comparing `graphdisplay-0.4.0/graphdisplay/json_manager.py` & `graphdisplay-0.4.1/graphdisplay/json_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -162,8 +162,23 @@
             self.__manager.add_permanent(word)
             messagebox.showinfo("Confirmación", f"Guardado : {word}")
         else:
             messagebox.showerror("Error", "You must enter a name")
         self.destroy()
 
     def __on_cancel(self):
-        self.destroy()
+        self.destroy()
+
+if __name__ == "__main__":
+    confirmation = input("WARNING: eliminating store. Do you want to proceed? [Y/N]: ")
+    if confirmation == "Y":
+        path = os.getcwd()
+
+        if os.path.exists(os.path.join(path, "permanent.json")):
+            os.remove(os.path.join(path, "permanent.json"))
+
+        store_path = os.path.join(path, "store/")
+
+        for file in os.listdir(store_path):
+            if file.endswith(".json"):
+                removing = os.path.join(store_path, file)
+                os.remove(removing)
```

### Comparing `graphdisplay-0.4.0/graphdisplay/main.py` & `graphdisplay-0.4.1/graphdisplay/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,81 @@
 """
 graphdisplay module created by Alberto Penas Díaz (https://github.com/seniorbeto).
 
 WARNING: modifying this file may cause the program to stop working or work incorrectly.
 """
+# Libraries
 import tkinter as tk
 import math
+import copy
+import time
 import queue
 import platform
 import multiprocessing as mp
+
+# Modules
 from .json_manager import JsonManager
 from .about_win_manager import AboutWindow
+from .tools_win_manager import ToolWindow
+from .graphs import Graph
+from .trees import AVLTree, BinarySearchTree
 from .general_config import *
 
+
 class GraphGUI:
+    """
+    Creates a GraphGUI object, which will display the graph in a external window. Nodes can be moved with the mouse.
+    :param graph: The graph/tree to be displayed.
+    :param node_radius: The radius of the nodes.
+    :param scr_width: The width of the window.
+    :param scr_height: The height of the window.
+    :param theme: color scheme of the node display.
+    """
 
+    # Using a instance-counter will determine how many GraphGUI objects are wanted
     instance = 0
 
     def __new__(cls, graph, node_radius: int = 30, scr_width: int = 600, scr_height: int = 600, theme: str = 'BROWN'):
         GraphGUI.instance += 1
         if GraphGUI.instance > 5:
             raise Exception("For safety reasons, only five instances of GraphGUI can be created")
+
+        # Generate multiprocessing
+
         if platform.system() == "Linux":
             mp.Process(target=cls._generate, args=(graph,
                                                     GraphGUI.instance,
                                                     node_radius,
                                                     scr_width,
                                                     scr_height,
                                                     theme)).start()
         else:
             try:
-                pid = mp.Process(target=cls._generate, args=(graph, GraphGUI.instance, node_radius, scr_width, scr_height, theme))
+                pid = mp.Process(target=cls._generate, args=(graph,
+                                                             GraphGUI.instance,
+                                                             node_radius,
+                                                             scr_width,
+                                                             scr_height,
+                                                             theme))
                 pid.start()
+            except RecursionError:
+                print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "For how GraphGUI works, high-demanding recursion trees are"
+                                                                 " not supported. Sorry for the inconvenience. ")
             except RuntimeError:
-                pass
-                #return GraphGUI.__GraphGUI(graph, GraphGUI.instance, node_radius, scr_width, scr_height, theme)
+
+                # For how multiprocessing works in python, it doesn't allow generating multiple processes
+                # without using a "if __name__ == "__main__":" statement. By implementing a try/expect, we
+                # can temporarily deal with this issue. Nevertheless, by doing this, there is a high chance
+                # to run into code-duplication and zombie processes generations.
+
+                print('\n'+'\033[93m'+"WARNING:"+'\033[0m'+" it is highly recommended to run the program inside a\n\n"
+                      "     if __name__ == \"__name__\":\n\n"
+                      "statement in order to avoid issues and duplicated processes.\n"
+                      "For more information please consider visiting the proyect \n"
+                      "documentation at: https://github.com/seniorbeto/graphdisplay\n")
 
     def __getattr__(self, name):
         return getattr(self.instance, name)
 
     def __setattr__(self, name, value):
         return setattr(self.instance, name, value)
 
@@ -52,204 +90,304 @@
             The creation of the window will stop the execution of the program until the window is closed. Thus, it is recommended
             to create the GraphGUI object at the end of the program.
             :param graph: The graph to be displayed
             :param node_radius: The radius of the nodes (default 40)
             :param scr_width: The width of the window (default 600)
             :param scr_height: The height of the window (default 600)
             """
+
+            # Begin time measurement
+            start = time.time()
+
+            # Parameter validation
             if type(node_radius) != int:
                 raise TypeError("The parameter node_radius must be an integer")
             if type(scr_width) != int or type(scr_height) != int:
                 raise TypeError("The parameters scr_width and scr_height must be integers")
             if node_radius < 10 or node_radius > 100:
                 raise ValueError("The parameter node_radius must be a value between 10 and 100")
             if scr_width < 200 or scr_height < 200:
                 raise ValueError("The parameters scr_width and scr_height must be values greater than 200")
             if scr_width > 2000 or scr_height > 2000:
                 raise ValueError("The parameters scr_width and scr_height must be values less than 2000")
 
             self.__ACTUAL_INSTANCE = instance
-            self.__graph = graph
+            self._graph = graph
             self.__node_radius = node_radius
             self.__scr_width = scr_width
             self.__scr_height = scr_height
             self.__XMARGIN = XMARGEN
             self.__YMARGIN = YMARGEN
             self._theme = theme.upper()
             self.nodes = []
             self.edges = []
+            self.__canvas_node_relation = {}
             try:
                 self._BACKGROUND_CANVAS_COLOR = THEMES[theme.upper()]['BACKGROUND_CANVAS_COLOR']
                 self._BUTTON_COLOR = THEMES[theme.upper()]['BUTTON_COLOR']
+                self._SELECTED_VERTEX_COLOR = THEMES[theme.upper()]['SELECTED_VERTEX_COLOR']
                 self._FRAME_COLOR = THEMES[theme.upper()]['FRAME_COLOR']
                 self._VERTEX_COLOR = THEMES[theme.upper()]['VERTEX_COLOR']
                 self._AUTHOR_NAME_COLOR = THEMES[theme.upper()]['AUTHOR_NAME_COLOR']
             except KeyError:
                 raise ValueError("The theme must be one of the following: " + str(list(THEMES.keys())))
 
+            # We will transform the graph type into our own prototype, so that future changes are easier
+            # to implement. Beyond this point, code will be implemented based on this prototypes.
             try:
                 self.__tree_root = graph._root
-                self.__is_tree = True
+                self._is_tree = True
+
+                vertices = list(self.__levelorder(self.__tree_root).keys())
+                if type(graph) == AVLTree:
+                    self._graph = AVLTree()
+                else:
+                    self._graph = BinarySearchTree()
+
+                for i in vertices:
+                    self._graph.insert(i)
+
             except AttributeError:
-                self.__is_tree = False
+                self._is_tree = False
+
+                vertices = list(graph._vertices.keys())
+                self._graph = Graph(vertices)
 
-            # create the main window and start the GUI
+                for vertex in graph._vertices:
+                    for adj in graph._vertices[vertex]:
+                        self._graph.addEdge(vertex, adj._vertex, adj._weight)
+
+            # Create the main window
             self.root = tk.Tk()
             self.root.title('GraphGUI')
             self.root.resizable(False, False)
             self.root.configure(bg=self._FRAME_COLOR, border=0, width=self.__scr_width, height=self.__scr_height)
 
-            self.json_manager = JsonManager(self.root, self)
-
             # Closing protocol
             self.root.protocol("WM_DELETE_WINDOW", self.__on_closing)
 
+            # Canvas creation and placement
             self.canvas = tk.Canvas(self.root, bg=self._BACKGROUND_CANVAS_COLOR, bd=0)
             self.canvas.place(x=self.__XMARGIN,
                               y=self.__YMARGIN,
                               width=self.__scr_width - self.__XMARGIN * 2,
                               height=self.__scr_height - self.__YMARGIN * 2 - BUTTON_HEIGHT)
 
+            # Buttons display
+            self.__display_buttons()
+
+            # Main display
+            self.json_manager = JsonManager(self.root, self)
+            data = self.json_manager.get_data('__last_store_'+str(self.__ACTUAL_INSTANCE))
+            self.__display(data)
+
+            # We will store each canvas TAGorID with each associated node object in order
+            # to reduce movement complexity to O(1)
+            for node in self.nodes:
+                self.__canvas_node_relation[node.circle] = node
+                self.__canvas_node_relation[node.text] = node
+
+
+            # Tag_bind for movable canvas objects
+            self.canvas.tag_bind("movil", "<ButtonPress-1>", self.on_press)
+            if self._is_tree and platform.system() != "Linux":
+                self.canvas.tag_bind("movil", "<Button-3>", self.on_press_left)
+            self.canvas.tag_bind("movil", "<Button1-Motion>", self.move)
+            self.selected_node = None
+
+            # End time measurement
+            end = time.time()
+            print("Displayed in:", round(end-start, 4))
+
+            # Main display protocol
+            self.root.mainloop()
+
+        def __display_buttons(self):
             # Reset button
             self.reset_button = tk.Button(self.root, text="Reset", bg=self._BUTTON_COLOR, command=self.display_reset,
                                           bd=0)
             self.reset_button.place(x=self.__XMARGIN,
-                                    y=self.__scr_height-self.__YMARGIN//2-BUTTON_HEIGHT,
+                                    y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
                                     width=BUTTON_WIDTH,
                                     height=BUTTON_HEIGHT)
 
             # Load button
-            self.load_button = tk.Button(self.root, text="Load", bg=self._BUTTON_COLOR, command=self.__call_manager_load,
+            self.load_button = tk.Button(self.root, text="Load", bg=self._BUTTON_COLOR,
+                                         command=self.__call_manager_load,
                                          bd=0)
             self.load_button.place(x=self.__XMARGIN + BUTTON_WIDTH + self.__XMARGIN,
                                    y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
                                    width=BUTTON_WIDTH,
                                    height=BUTTON_HEIGHT)
 
             # Save button
-            self.save_button = tk.Button(self.root, text="Save", bg=self._BUTTON_COLOR, command=self.__call_manager_save,
+            self.save_button = tk.Button(self.root, text="Save", bg=self._BUTTON_COLOR,
+                                         command=self.__call_manager_save,
                                          bd=0)
-            self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN)*2,
+            self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 2,
                                    y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
                                    width=BUTTON_WIDTH,
                                    height=BUTTON_HEIGHT)
 
             # Delete button
             self.save_button = tk.Button(self.root, text="Delete", bg=self._BUTTON_COLOR,
                                          command=self.__call_manager_delete, bd=0)
-            self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN)*3,
+            self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 3,
                                    y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
                                    width=BUTTON_WIDTH,
                                    height=BUTTON_HEIGHT)
 
             # About button
             self.save_button = tk.Button(self.root, text="About", bg=self._BUTTON_COLOR,
                                          command=self.__call_about_window, bd=0)
             self.save_button.place(x=self.__scr_width - self.__XMARGIN - BUTTON_WIDTH,
                                    y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
                                    width=BUTTON_WIDTH,
                                    height=BUTTON_HEIGHT)
 
-            # Main display
-            data = self.json_manager.get_data('__last_store_'+str(self.__ACTUAL_INSTANCE))
-            self.__display(data)
-
-            self.canvas.tag_bind("movil", "<ButtonPress-1>", self.on_press)
-            self.canvas.tag_bind("movil", "<Button1-Motion>", self.move)
-            self.selected_node = None
+            # Tools button
+            self.save_button = tk.Button(self.root, text="Tools", bg=self._BUTTON_COLOR,
+                                         command=self.__call_tools_window, bd=0)
+            self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 4,
+                                   y=self.__scr_height - self.__YMARGIN // 2 - BUTTON_HEIGHT,
+                                   width=BUTTON_WIDTH,
+                                   height=BUTTON_HEIGHT)
 
-            self.root.mainloop()
+        def __call_tools_window(self):
+            """Generator of ToolWindow"""
+            ToolWindow(self.root, self)
 
         def __call_about_window(self):
+            """Generator of AboutWindow"""
             AboutWindow(self.root, self)
 
         def __call_manager_delete(self):
-            if not self.__is_tree:
+            """Generator of Delete Window"""
+            if not self._is_tree:
                 self.json_manager.generate_delete_window()
             else:
                 tk.messagebox.showerror("Error", "This function is not yet available for trees")
 
         def __call_manager_load(self):
-            if not self.__is_tree:
+            """Generator of Load Window"""
+            if not self._is_tree:
                 new_position = self.json_manager.generate_load_window()
                 if new_position:
                     self.display_reset(new_position)
             else:
                 tk.messagebox.showerror("Error", "This function is not yet available for trees")
 
         def __call_manager_save(self):
-            if not self.__is_tree:
+            """Generator of Save Window"""
+            if not self._is_tree:
                 curr_pos = {}
                 for node in self.nodes:
                     curr_pos[node.id] = (node.pos_x, node.pos_y)
                 self.json_manager.generate_save_window(curr_pos)
             else:
                 tk.messagebox.showerror("Error", "This function is not yet available for trees")
 
         def display_reset(self, new_data: dict = None):
+            """
+            Sets the main display to default by deleting all objects in canvas and displaying them
+            in the position stored in new_data.
+            """
             self.canvas.delete("all")
             self.__display(new_data)
 
         def __display(self, data: dict = None):
-            if not self.__is_tree:
+            """
+            Main display for all nodes in the canvas. Whose position is determined in "data".
+            If data is None, the default display will be showed. This is, in case of a simple graph,
+            the first vertex in the middle of the screen and the rest surrounding it in a polygon shape.
+            In case of a tree, it is always display in a tree-like structure.
+
+            This function also checks if some node position has been stored outside the frames of the window,
+            in which case will correct.
+            """
+            if not self._is_tree:
                 # Preparation for the nodes display
                 scr_center = ((self.__scr_width - 14) // 2, (self.__scr_height - 30) // 2)
                 display_radius = min(self.__scr_width - 30 - self.__node_radius, self.__scr_height - 14 - self.__node_radius) // 2 - self.__node_radius - 10
-                arch_angle = 360 / len(self.__graph._vertices)
+                arch_angle = 360 / len(self._graph._vertices)
                 first_node_pos = (scr_center[0] - self.__node_radius, scr_center[1] - self.__node_radius)
 
                 # Display the nodes
                 self.nodes = []
                 i = 0
                 angle = 0
-                for vertex in self.__graph._vertices:
+                for vertex in self._graph._vertices:
+                    # The first vertex will be displayed in the screen center
                     if i == 0:
                         if data and str(vertex) in data and \
                                 data[str(vertex)][0] < self.__scr_width and \
                                 data[str(vertex)][1] < self.__scr_height - 30 and \
                                 data[str(vertex)][0] + self.__node_radius*2 > 0 and \
                                 data[str(vertex)][1] + self.__node_radius*2 > 0:
                             self.nodes.append(
-                                Node(self.canvas, self.__node_radius, data[str(vertex)][0], data[str(vertex)][1], text=vertex, bg=self._VERTEX_COLOR))
+                                Node(self.canvas,
+                                     self.__node_radius,
+                                     data[str(vertex)][0],
+                                     data[str(vertex)][1],
+                                     text=vertex,
+                                     bg=self._VERTEX_COLOR))
                         else:
                             self.nodes.append(
-                                Node(self.canvas, self.__node_radius, first_node_pos[0], first_node_pos[1], text=vertex, bg=self._VERTEX_COLOR))
+                                Node(self.canvas,
+                                     self.__node_radius,
+                                     first_node_pos[0],
+                                     first_node_pos[1],
+                                     text=vertex,
+                                     bg=self._VERTEX_COLOR))
                     else:
+                        # Those vertices that are not the first, will surround the screen center, scrolling
+                        # around an imaginary circumference.
                         if data and str(vertex) in data and \
                                 data[str(vertex)][0] < self.__scr_width and \
                                 data[str(vertex)][1] < self.__scr_height - 30 and \
                                 data[str(vertex)][0] + self.__node_radius*2 > 0 and \
                                 data[str(vertex)][1] + self.__node_radius*2 > 0:
                             self.nodes.append(
-                                Node(self.canvas, self.__node_radius, data[str(vertex)][0], data[str(vertex)][1], text=vertex, bg=self._VERTEX_COLOR))
+                                Node(self.canvas,
+                                     self.__node_radius,
+                                     data[str(vertex)][0],
+                                     data[str(vertex)][1],
+                                     text=vertex,
+                                     bg=self._VERTEX_COLOR))
                         else:
                             self.nodes.append(Node(self.canvas,
                                                    self.__node_radius,
                                                    int(scr_center[0] - self.__node_radius - display_radius * math.sin(
                                                        math.radians(angle))),
                                                    int(scr_center[1] - self.__node_radius - display_radius * math.cos(
                                                        math.radians(angle))),
                                                    text=vertex, bg=self._VERTEX_COLOR))
                     i += 1
                     angle += arch_angle
 
                 # Create the edges
                 i = 0
                 self.edges = []
-                for vertex in self.__graph._vertices:
-                    for adj in self.__graph._vertices[vertex]:
+                for vertex in self._graph._vertices:
+                    for adj in self._graph._vertices[vertex]:
                         for node in self.nodes:
                             if node.id == adj._vertex:
-                                self.edges.append(Edge(self.canvas, self.nodes[i], node, adj._weight if adj._weight else 1, window_color=self._BACKGROUND_CANVAS_COLOR))
+                                self.edges.append(Edge(self.canvas,
+                                                       self.nodes[i],
+                                                       node,
+                                                       adj._weight,
+                                                       window_color=self._BACKGROUND_CANVAS_COLOR))
                                 node.asociated_edges_IN.append(self.edges[-1])
                                 self.nodes[i].asociated_edges_OUT.append(self.edges[-1])
                     i += 1
 
-                # Display the edges
-                if self.__graph._directed:
+                # While displaying the edges, we first have to check if it is needed to display the weight
+                # in an edge side (instead of the center) in case that to vertices are pointing to each other,
+                # since this would result in an overlap between those to weights
+                if self._graph._directed:
                     for edge in self.edges:
                         edge_start_node = edge.start_node
                         edge_end_node = edge.end_node
                         found = False
                         for i in edge_start_node.asociated_edges_IN:
                             if i.start_node == edge_end_node:
                                 found = True
@@ -258,33 +396,35 @@
                                 break
                         if not found:
                             edge.show()
                 else:
                     for edge in self.edges:
                         edge.show()
 
-            elif self.__is_tree:
+            elif self._is_tree:
+                # The tree display is slightly more complicated (it was a complete nightmare for a one man job
+                # to be honest). For information on how it works, please consider visiting: #TODO
                 self.nodes = []
                 self.edges = []
                 root_position = ((self.__scr_width - self.__node_radius*2) // 2, self.__YMARGIN + 33)
                 self.nodes.append(Node(self.canvas,
                                        self.__node_radius,
                                        root_position[0],
                                        root_position[1],
-                                       text=self.__graph._root.elem,
+                                       text=self._graph._root.elem,
                                        bg=self._VERTEX_COLOR))
 
                 # We display the rest of the nodes in a tree-like structure by
                 # dividing the screen in levels and displaying the nodes in each level
-                level_order = self.__levelorder(self.__graph._root)
+                level_order = self.__levelorder(self._graph._root)
                 levels = max(level_order.values()) + 1
                 level_height = (self.__scr_height - self.__YMARGIN - 60) // levels
 
                 # We determine how many nodes are in each level
-                last_nodes = [self.__graph._root.elem]
+                last_nodes = [self._graph._root.elem]
                 for i in range(levels - 1):
                     if i != 0:
                         last_nodes = nodes_in_level
                     nodes_in_level = []
                     for node in level_order:
                         if level_order[node] == i + 1:
                             nodes_in_level.append(node)
@@ -351,21 +491,21 @@
 
 
             # Display author
             self.__autor = self.canvas.create_text(self.__scr_width // 2, self.__YMARGIN + 3, text="by @seniorbeto",
                                                    fill=self._AUTHOR_NAME_COLOR, font=("Courier", 10))
 
         def __get_children(self, elem) -> tuple:
-            """returns a tuple with the children of node"""
+            """returns a tuple with the children of node with element = elem"""
             node = self.__search_node(elem)
             return node.left.elem if node.left else None, node.right.elem if node.right else None
 
         def __search_node(self, elem):
             """returns the node with the given element"""
-            return self.__search_node_aux(self.__graph._root, elem)
+            return self.__search_node_aux(self._graph._root, elem)
 
         def __search_node_aux(self, node, elem):
             """returns the node with the given element"""
             if node == None:
                 return None
             if node.elem == elem:
                 return node
@@ -390,65 +530,63 @@
                 if current.right != None:
                     q.put(current.right)
                     register[current.right.elem] = value + 1
 
             return register
 
         def __on_closing(self):
+            """Store the current data at closing protocol"""
             data = {}
             for node in self.nodes:
                 data[node.id] = (node.pos_x, node.pos_y)
             self.json_manager.save_data('__last_store_'+str(self.__ACTUAL_INSTANCE), data)
             self.root.destroy()
 
+        def on_press_left(self, event):
+            """
+            If, in a tree, a node is left-clicked, it will generate a display of the subtree
+            """
+            if self._is_tree:
+                node = self.canvas.find_withtag(tk.CURRENT)
+                for nd in self.nodes:
+                    if nd.circle == node[0] or nd.text == node[0]:
+                        root = self.__search_node(nd.id)
+                        vertices = self.__levelorder(root)
+                        new_tree = copy.copy(self._graph)
+                        new_tree.remove_all()
+                        for i in list(vertices.keys()):
+                            new_tree.insert(i)
+                GraphGUI(new_tree,
+                         self.__node_radius,
+                         self.__scr_width,
+                         self.__scr_height,
+                         self._theme)
+
         def on_press(self, event):
+            """Right mouse click protocol"""
+            # Store the node if it has been right-clicked
             node = self.canvas.find_withtag(tk.CURRENT)
             self.selected_node = (node, event.x, event.y)
 
         def move(self, event):
+            """
+            It moves a node if it has been selected on the right mouse click protocol. After moving it, it updates
+            automatically all edges attached to the node.
+            """
             x, y = event.x, event.y
             node, x0, y0 = self.selected_node
-            for i in self.nodes:
-                if i.circle == node[0] or i.text == node[0]:
-                    self.canvas.move(i.circle, x - x0, y - y0)
-                    self.canvas.move(i.text, x - x0, y - y0)
-                    i.pos_x += x - x0
-                    i.pos_y += y - y0
-                    for edge in i.asociated_edges_IN:
-                        edge_start = edge.start_node
-                        weight = edge.weight
-                        color = edge.window_color
-                        overlaped = edge.overlaped
-                        i.asociated_edges_IN.remove(edge)
-                        edge.terminate()
-                        new_edge = Edge(self.canvas, edge_start, i, weight, overlaped=overlaped, window_color=color)
-                        new_edge.show()
-                        i.asociated_edges_IN.append(new_edge)
-                        for nd in self.nodes:
-                            if edge in nd.asociated_edges_OUT:
-                                nd.asociated_edges_OUT.remove(edge)
-                                nd.asociated_edges_OUT.append(new_edge)
-                                break
-                    for edge in i.asociated_edges_OUT:
-                        edge_end = edge.end_node
-                        weight = edge.weight
-                        color = edge.window_color
-                        overlaped = edge.overlaped
-                        i.asociated_edges_OUT.remove(edge)
-                        edge.terminate()
-                        new_edge = Edge(self.canvas, i, edge_end, weight, overlaped=overlaped, window_color=color)
-                        new_edge.show()
-                        i.asociated_edges_OUT.append(new_edge)
-                        for nd in self.nodes:
-                            if edge in nd.asociated_edges_IN:
-                                nd.asociated_edges_IN.remove(edge)
-                                nd.asociated_edges_IN.append(new_edge)
-                                break
-
-
+            node_obj = self.__canvas_node_relation[node[0]]
+            self.canvas.move(node_obj.circle, x - x0, y - y0)
+            self.canvas.move(node_obj.text, x - x0, y - y0)
+            node_obj.pos_x += x - x0
+            node_obj.pos_y += y - y0
+            for edge in node_obj.asociated_edges_IN:
+                edge.update_position()
+            for edge in node_obj.asociated_edges_OUT:
+                edge.update_position()
             self.selected_node = (node, x, y)
 
 class Node:
     def __init__(self, canvas: tk.Canvas, radius:int, posx: int, posy: int, text: str, bg: str = "white"):
         self.asociated_edges_IN = []
         self.asociated_edges_OUT = []
         self.canvas = canvas
@@ -475,29 +613,52 @@
         self.start_node = start
         self.end_node = end
         self.weight = weight
         self.window_color = window_color
         self.start = self.__calculate_start(start, end)
         self.end = self.__calculate_end(start, end)
 
+    def update_position(self):
+        self.__recalculate()
+        self.canvas.coords(self.line, self.start[0], self.start[1], self.end[0], self.end[1])
+        if self.weight:
+            if not self.overlaped:
+                self.canvas.coords(self.window, (self.start[0] + self.end[0]) // 2, (self.start[1] + self.end[1]) // 2)
+            else:
+                self.canvas.coords(self.window, self.start[0] * 0.2 + self.end[0] * 0.8, self.start[1] * 0.2 + self.end[1] * 0.8)
+
     def terminate(self):
         self.canvas.delete(self.line)
         if self.weight:
             self.canvas.delete(self.window)
 
     def show(self):
-        self.line = self.canvas.create_line(self.start[0], self.start[1], self.end[0], self.end[1], arrow=tk.LAST, width=1.5)
+        self.line = self.canvas.create_line(self.start[0],
+                                            self.start[1],
+                                            self.end[0],
+                                            self.end[1],
+                                            arrow=tk.LAST,
+                                            width=1.5)
         if self.weight:
             if not self.overlaped:
-                self.window = self.canvas.create_window((self.start[0] + self.end[0]) // 2, (self.start[1] + self.end[1]) // 2,
-                                                   window=tk.Label(self.canvas,bg=self.window_color ,text=str(self.weight)))
+                self.window = self.canvas.create_window((self.start[0] + self.end[0]) // 2,
+                                                        (self.start[1] + self.end[1]) // 2,
+                                                        window=tk.Label(self.canvas,
+                                                                        bg=self.window_color,
+                                                                        text=str(self.weight)))
             else:
                 self.window = self.canvas.create_window((self.start[0] * 0.2 + self.end[0] * 0.8),
-                                                   (self.start[1] * 0.2 + self.end[1] * 0.8),
-                                                   window=tk.Label(self.canvas, bg=self.window_color, text=str(self.weight)))
+                                                        (self.start[1] * 0.2 + self.end[1] * 0.8),
+                                                        window=tk.Label(self.canvas,
+                                                                        bg=self.window_color,
+                                                                        text=str(self.weight)))
+
+    def __recalculate(self):
+        self.start = self.__calculate_start(self.start_node, self.end_node)
+        self.end = self.__calculate_end(self.start_node, self.end_node)
 
     def __calculate_start(self, start: Node, end: Node) -> tuple:
         """
         It calculates the initial position of the arrow that connects the nodes "start" and "end"
         :param start: Node
         :param end: Node
         :return: tuple with the initial position of the arrow
@@ -536,8 +697,8 @@
         y = y2 - y1
         edge_angle = math.atan2(y, x) * (180.0 / math.pi)
         x = math.cos(math.radians(edge_angle)) * end.radius
         y = math.sin(math.radians(edge_angle)) * end.radius
         return  (center_end[0] - int(x), center_end[1] - int(y))
 
 if __name__ == "__main__":
-    pass
+    pass
```

### Comparing `graphdisplay-0.4.0/graphdisplay/trees/auto_balance_tree.py` & `graphdisplay-0.4.1/graphdisplay/trees/auto_balance_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.0/graphdisplay/trees/binary_search_tree.py` & `graphdisplay-0.4.1/graphdisplay/trees/binary_search_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         in the subtree node.
         This is the node that is furthest to the left"""
         min_node = node
         while min_node.left is not None:
             min_node = min_node.left
         return min_node
 
+    def remove_all(self):
+        self._root = None
+
     def remove(self, elem: object) -> None:
         # update the root with the new subtree after remove elem
         self._root = self._remove(self._root, elem)
 
     def _remove(self, node: BinaryNode, elem: object) -> BinaryNode:
         """It recursively searches the node. When the node is
         found, the node has to be removed"""
```

### Comparing `graphdisplay-0.4.0/graphdisplay/trees/binary_tree.py` & `graphdisplay-0.4.1/graphdisplay/trees/binary_tree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Implementation of Binary Tree
 
+import queue
 
 class BinaryNode:
 
     def __init__(self, elem: object, node_left: 'BinaryNode' = None, node_right: 'BinaryNode' = None) -> None:
         self.elem = elem
         self.left = node_left
         self.right = node_right
@@ -132,15 +133,29 @@
     def _inorder_list(self, node: BinaryNode, in_list: list) -> None:
         """populates in_list with the inorder traversal of the subtree node"""
         if node is not None:
             self._postorder_list(node.left, in_list)
             in_list.append(node.elem)
             self._postorder_list(node.right, in_list)
 
+    def levelorder_list(self):
+        """returns a list with the level order traversal of the trees"""
+        levelorder = []
+        q = queue.Queue()
+        q.put(self._root)  # enqueue: we save the root
+
+        while q.empty() == False:
+            current = q.get()  # dequeue
+            levelorder.append(current.elem)
+            if current.left != None:
+                q.put(current.left)
+            if current.right != None:
+                q.put(current.right)
 
+        return levelorder
 
     def draw(self) -> None:
         """function to draw a trees. """
         if self._root:
             self._draw('', self._root, False)
         else:
             print('trees is empty')
```

### Comparing `graphdisplay-0.4.0/graphdisplay.egg-info/PKG-INFO` & `graphdisplay-0.4.1/graphdisplay.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.4.0
+Version: 0.4.1
 Summary: Librería para representar visualmente grafos de tipo diccionario
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -30,23 +30,23 @@
 ## Método de uso 
 
 Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
 tkinter y math (que muchas veces vienen instaladas por defecto en python). 
 
 Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
 para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
-para una mejor visualización. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
+para una mejor visualización. **Al desplazar los vértices por la pantalla y fijar su posición, si se cierra la ventana y se vuelve a abrir, el grafo seguirá con la forma con la que se ha movido
+antes.**. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
 grafos grandes y complejos:
 + graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
 de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
 implementación de grafos que viene por defecto con el paquete.
 + node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
 + scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
 + scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-+ theme: el tema de la ventana, por defecto es 'brown' y no voy a mencionarlos todos porque hay muchos y me da pereza.
 
 Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
 ```python
 g = Graph([1, 2, 3])
 g.addEdge(1, 2)
 g.addEdge(2, 3)
 
@@ -57,23 +57,16 @@
 GraphGUI(g, 32, 700, 700)
 
 # Para ajustar únicamente el ancho de la pantalla a 200 píxeles
 GraphGUI(g, scr_width=200)
 ```
 
 Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
-argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `addEdge`, con los vértices que conecta la arista además del valor/coste de la arista.
+argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `add_edge`, con los vértices que conecta la arista además del valor/coste de la arista.
 
-## Funcionalidades
-Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
-éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
-instaciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
-Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
-tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón save y nombrando el guardado) para
-después poder cargarlo en cualquier momento.
 ## Ejemplo de uso
 
 Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
 
 ```python
 labels = ['A', 'B', 'C', 'D', 'E']
 g = Graph(labels)
```

### Comparing `graphdisplay-0.4.0/graphdisplay.egg-info/SOURCES.txt` & `graphdisplay-0.4.1/graphdisplay.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.py
 graphdisplay/__init__.py
 graphdisplay/about_win_manager.py
 graphdisplay/general_config.py
 graphdisplay/json_manager.py
 graphdisplay/main.py
+graphdisplay/tools_win_manager.py
 graphdisplay.egg-info/PKG-INFO
 graphdisplay.egg-info/SOURCES.txt
 graphdisplay.egg-info/dependency_links.txt
 graphdisplay.egg-info/top_level.txt
 graphdisplay/graphs/__init__.py
 graphdisplay/graphs/graph.py
 graphdisplay/store/__init__.py
```

### Comparing `graphdisplay-0.4.0/setup.py` & `graphdisplay-0.4.1/setup.py`

 * *Files identical despite different names*

