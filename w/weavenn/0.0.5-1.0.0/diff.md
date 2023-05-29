# Comparing `tmp/weavenn-0.0.5.tar.gz` & `tmp/weavenn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weavenn-0.0.5.tar", last modified: Wed Apr  6 08:51:31 2022, max compression
+gzip compressed data, was "weavenn-1.0.0.tar", last modified: Mon May 29 12:55:50 2023, max compression
```

## Comparing `weavenn-0.0.5.tar` & `weavenn-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-04-06 08:51:31.689527 weavenn-0.0.5/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       31 2022-03-04 17:26:53.000000 weavenn-0.0.5/MANIFEST.in
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      377 2022-04-06 08:51:31.689527 weavenn-0.0.5/PKG-INFO
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      260 2022-02-21 10:01:01.000000 weavenn-0.0.5/README.md
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       38 2022-04-06 08:51:31.689527 weavenn-0.0.5/setup.cfg
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      900 2022-04-06 08:40:53.000000 weavenn-0.0.5/setup.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-04-06 08:51:31.689527 weavenn-0.0.5/src/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     4166 2022-04-06 08:24:48.000000 weavenn-0.0.5/src/algorithm.cpp
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      637 2022-04-06 08:40:50.000000 weavenn-0.0.5/src/algorithm.hpp
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      303 2022-03-18 10:54:35.000000 weavenn-0.0.5/src/bindings.cpp
--rw-rw-r--   0 maixent   (1000) maixent   (1000)    16716 2022-03-31 17:33:45.000000 weavenn-0.0.5/src/louvain.cpp
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     2320 2022-03-08 09:56:02.000000 weavenn-0.0.5/src/louvain.hpp
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-04-06 08:51:31.689527 weavenn-0.0.5/weavenn/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       50 2022-04-06 08:51:01.000000 weavenn-0.0.5/weavenn/__init__.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     1338 2022-03-07 08:56:41.000000 weavenn-0.0.5/weavenn/ann.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     2697 2022-03-31 16:40:43.000000 weavenn-0.0.5/weavenn/score.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     6620 2022-04-06 08:39:42.000000 weavenn-0.0.5/weavenn/weavenn.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2022-04-06 08:51:31.689527 weavenn-0.0.5/weavenn.egg-info/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      377 2022-04-06 08:51:31.000000 weavenn-0.0.5/weavenn.egg-info/PKG-INFO
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      340 2022-04-06 08:51:31.000000 weavenn-0.0.5/weavenn.egg-info/SOURCES.txt
--rw-rw-r--   0 maixent   (1000) maixent   (1000)        1 2022-04-06 08:51:31.000000 weavenn-0.0.5/weavenn.egg-info/dependency_links.txt
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       28 2022-04-06 08:51:31.000000 weavenn-0.0.5/weavenn.egg-info/requires.txt
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       17 2022-04-06 08:51:31.000000 weavenn-0.0.5/weavenn.egg-info/top_level.txt
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 12:55:50.648534 weavenn-1.0.0/
+-rw-r--r--   0 maixent   (1000) maixent   (1000)       31 2022-03-04 17:26:53.000000 weavenn-1.0.0/MANIFEST.in
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      149 2023-05-29 12:55:50.648534 weavenn-1.0.0/PKG-INFO
+-rw-r--r--   0 maixent   (1000) maixent   (1000)      260 2022-02-21 10:01:01.000000 weavenn-1.0.0/README.md
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       38 2023-05-29 12:55:50.648534 weavenn-1.0.0/setup.cfg
+-rw-r--r--   0 maixent   (1000) maixent   (1000)      703 2023-05-29 12:54:31.000000 weavenn-1.0.0/setup.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 12:55:50.648534 weavenn-1.0.0/src/
+-rw-r--r--   0 maixent   (1000) maixent   (1000)     5193 2022-08-03 08:50:43.000000 weavenn-1.0.0/src/algorithm.cpp
+-rw-r--r--   0 maixent   (1000) maixent   (1000)      894 2022-06-28 12:20:50.000000 weavenn-1.0.0/src/algorithm.hpp
+-rw-r--r--   0 maixent   (1000) maixent   (1000)      303 2023-05-29 12:42:25.000000 weavenn-1.0.0/src/bindings.cpp
+-rw-r--r--   0 maixent   (1000) maixent   (1000)    16478 2023-05-29 12:42:37.000000 weavenn-1.0.0/src/louvain.cpp
+-rw-r--r--   0 maixent   (1000) maixent   (1000)     2205 2022-04-22 10:21:26.000000 weavenn-1.0.0/src/louvain.hpp
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 12:55:50.648534 weavenn-1.0.0/weavenn/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       52 2023-05-29 12:50:06.000000 weavenn-1.0.0/weavenn/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     1476 2023-05-29 12:41:20.000000 weavenn-1.0.0/weavenn/louvain.py
+-rw-r--r--   0 maixent   (1000) maixent   (1000)    10406 2023-05-29 12:53:15.000000 weavenn-1.0.0/weavenn/weavenn.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 12:55:50.648534 weavenn-1.0.0/weavenn.egg-info/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      149 2023-05-29 12:55:50.000000 weavenn-1.0.0/weavenn.egg-info/PKG-INFO
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      327 2023-05-29 12:55:50.000000 weavenn-1.0.0/weavenn.egg-info/SOURCES.txt
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)        1 2023-05-29 12:55:50.000000 weavenn-1.0.0/weavenn.egg-info/dependency_links.txt
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       42 2023-05-29 12:55:50.000000 weavenn-1.0.0/weavenn.egg-info/requires.txt
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       17 2023-05-29 12:55:50.000000 weavenn-1.0.0/weavenn.egg-info/top_level.txt
```

### Comparing `weavenn-0.0.5/src/louvain.cpp` & `weavenn-1.0.0/src/louvain.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 using GraphNeighbors = std::vector<Nodes>;
 using Weight = float;
 using Weights = std::vector<Weight>;
 using GraphWeights = std::vector<Weights>;
 using WeightMap = std::unordered_map<Node, Weight>;
 using NodeSet = std::unordered_set<Node>;
 
-bool sort_by_increase(const std::tuple<Node, Node, float, Weight> &a,
-                      const std::tuple<Node, Node, float, Weight> &b)
+bool sort_by_increase(
+    const std::tuple<Node, Node, Node, float, Weight, Weight> &a,
+    const std::tuple<Node, Node, Node, float, Weight, Weight> &b)
 {
     return (std::get<2>(a) > std::get<2>(b));
 }
 
 std::tuple<Nodes, Weights, Weights, Weights, Weights, float> init_status(
     GraphNeighbors const &graph_neighbors,
     GraphWeights const &graph_weights)
@@ -47,23 +48,37 @@
 
         Nodes neighbors = graph_neighbors[node];
         Weights neighbors_weight = graph_weights[node];
         for (size_t i = 0; i < neighbors.size(); i++)
         {
             Node neighbor = neighbors[i];
             Weight weight = neighbors_weight[i];
+            // if (neighbor == node)
+            // {
+            //     internals[node] += weight;
+            //     loops[node] += weight;
+            //     weight *= 2;
+            // }
+            // degrees[node] += weight;
+            // gdegrees[node] += weight;
+            // total_weight += weight;
             if (neighbor == node)
             {
                 internals[node] += weight;
                 loops[node] += weight;
-                weight *= 2;
+                degrees[node] += 2 * weight;
+                gdegrees[node] += 2 * weight;
+                total_weight += 2 * weight;
+            }
+            else
+            {
+                degrees[node] += weight;
+                gdegrees[node] += weight;
+                total_weight += weight;
             }
-            degrees[node] += weight;
-            gdegrees[node] += weight;
-            total_weight += weight;
         }
     }
     total_weight /= 2;
     return std::make_tuple(
         node2com,
         internals,
         loops,
@@ -72,31 +87,22 @@
         total_weight);
 }
 
 float modularity(
     Weights const &internals,
     Weights const &degrees,
     float total_weight,
-    float resolution,
-    bool z_modularity)
+    float resolution)
 {
     float result = 0;
     float m = 2. * total_weight;
     for (Node com = 0; com < degrees.size(); com++)
     {
-        float Q_c = resolution * internals[com] / total_weight;
-        float ratio = degrees[com] / m;
-        ratio *= ratio;
-
-        Q_c -= ratio;
-        if (z_modularity)
-        {
-            Q_c /= sqrt(ratio * (1 - ratio));
-        }
-        result += Q_c;
+        result += resolution * internals[com] / total_weight;
+        result -= pow(degrees[com] / m, 2);
     }
     return result;
 }
 
 WeightMap neighcom(
     GraphNeighbors const &graph_neighbors,
     GraphWeights const &graph_weights,
@@ -124,23 +130,21 @@
     GraphWeights const &graph_weights,
     Nodes &node2com,
     Weights &internals,
     Weights const &loops,
     Weights &degrees,
     Weights const &gdegrees,
     float total_weight,
-    float resolution,
-    bool z_modularity)
+    float resolution)
 {
     bool modified = true;
     float cur_mod = modularity(internals,
                                degrees,
                                total_weight,
-                               resolution,
-                               z_modularity);
+                               resolution);
     float new_mod = cur_mod;
     size_t n_nodes = graph_neighbors.size();
     float m = 2 * total_weight;
     while (modified)
     {
         modified = false;
         cur_mod = new_mod;
@@ -164,21 +168,14 @@
             {
                 if (weight <= 0)
                     continue;
 
                 float increase = resolution * weight;
                 increase -= degrees[com] * node_gdegree / m;
 
-                if (z_modularity)
-                {
-                    float ratio = degrees[com] / m;
-                    ratio *= ratio;
-                    increase /= sqrt(ratio * (1 - ratio));
-                }
-
                 if (increase > best_increase)
                 {
                     best_increase = increase;
                     best_com = com;
                 }
             }
 
@@ -189,32 +186,30 @@
             if (best_com != node_com)
                 modified = true;
         }
 
         new_mod = modularity(internals,
                              degrees,
                              total_weight,
-                             resolution,
-                             z_modularity);
+                             resolution);
         if (new_mod - cur_mod < 0.0000001)
             break;
     }
 }
 
 void one_level_prune(
     GraphNeighbors const &graph_neighbors,
     GraphWeights const &graph_weights,
     Nodes &node2com,
     Weights &internals,
     Weights const &loops,
     Weights &degrees,
     Weights const &gdegrees,
     float total_weight,
-    float resolution,
-    bool z_modularity)
+    float resolution)
 {
     size_t n_nodes = graph_neighbors.size();
     float m = 2 * total_weight;
 
     NodeSet P;
     for (Node i = 0; i < n_nodes; i++)
     {
@@ -241,19 +236,14 @@
         {
             if (weight <= 0)
                 continue;
 
             float increase = resolution * weight;
             increase -= degrees[com] * gdegrees[node] / m;
 
-            if (z_modularity)
-            {
-                float ratio = degrees[com] / m;
-                increase /= sqrt(ratio * ratio * (1 - ratio * ratio));
-            }
             if (increase > best_increase)
             {
                 best_increase = increase;
                 best_com = com;
             }
         }
 
@@ -282,69 +272,77 @@
     GraphWeights const &graph_weights,
     Nodes &node2com,
     Weights &internals,
     Weights const &loops,
     Weights &degrees,
     Weights const &gdegrees,
     float total_weight,
-    float resolution,
-    bool z_modularity)
+    float resolution)
 {
     size_t n_nodes = graph_neighbors.size();
     float m = 2 * total_weight;
 
-    std::vector<std::tuple<Node, Node, float, Weight>> best_moves;
+    Node best_move_node;
+    Node best_move_com;
+    Node old_move_com;
+    WeightMap best_neighbor_weight;
+
+    float best_increase = -INFINITY;
+    bool modified = false;
     for (Node node = 0; node < n_nodes; node++)
     {
         Node node_com = node2com[node];
         WeightMap neighbor_weight = neighcom(
             graph_neighbors, graph_weights, node2com, node);
 
         // remove
         Weight node_gdegree = gdegrees[node];
         Weight node_loop = loops[node];
+        Weight com_weight = neighbor_weight[node_com];
+
         node2com[node] = -1;
         degrees[node_com] -= node_gdegree;
-        internals[node_com] -= neighbor_weight[node_com] + node_loop;
+        internals[node_com] -= com_weight + node_loop;
 
         Node best_com = node_com;
-        float best_increase = -INFINITY;
         for (auto [com, weight] : neighbor_weight)
         {
             if (weight <= 0)
                 continue;
 
-            float increase = resolution * weight - degrees[com] * node_gdegree / m;
-            if (z_modularity)
-            {
-                float ratio = degrees[com] / m;
-                increase /= sqrt(ratio * ratio * (1 - ratio * ratio));
-            }
+            float increase = resolution * weight;
+            increase -= degrees[com] * node_gdegree / m;
             if (increase > best_increase)
             {
                 best_increase = increase;
-                best_com = com;
+                best_move_node = node;
+                best_move_com = com;
+                best_neighbor_weight = neighbor_weight;
+                old_move_com = node_com;
+                modified = true;
             }
         }
 
-        best_moves.push_back(
-            std::make_tuple(
-                node, best_com, best_increase, neighbor_weight[best_com]));
-
         // insert
         node2com[node] = node_com;
         degrees[node_com] += node_gdegree;
-        internals[node_com] += neighbor_weight[node_com] + node_loop;
+        internals[node_com] += com_weight + node_loop;
     }
+    if (!modified)
+        return;
 
-    sort(best_moves.begin(), best_moves.end(), sort_by_increase);
-    auto [node, best_com, best_increase, weight] = best_moves[0];
-    node2com[node] = best_com;
-    degrees[best_com] += gdegrees[node];
-    internals[best_com] += weight + loops[node];
+    // remove
+    node2com[best_move_node] = -1;
+    degrees[old_move_com] -= gdegrees[best_move_node];
+    internals[old_move_com] -= best_neighbor_weight[old_move_com] + loops[best_move_node];
+
+    // insert
+    node2com[best_move_node] = best_move_com;
+    degrees[best_move_com] += gdegrees[best_move_node];
+    internals[best_move_com] += best_neighbor_weight[best_move_com] + loops[best_move_node];
 }
 
 std::tuple<GraphNeighbors, Nodes> renumber(
     GraphNeighbors const &graph_neighbors,
     GraphWeights const &graph_weights,
     Nodes const &node2com)
 {
@@ -419,15 +417,16 @@
             new_graph_neighbors[i].push_back(com_);
             if (com_ == i)
                 new_graph_weights[i].push_back(weight_ / 2);
             else
                 new_graph_weights[i].push_back(weight_);
         }
     }
-    return std::make_tuple(new_graph_neighbors, new_graph_weights, new_n_nodes);
+    return std::make_tuple(
+        new_graph_neighbors, new_graph_weights, new_n_nodes);
 }
 
 Nodes get_partition(Nodes const &node2com, size_t n_nodes)
 {
     Nodes partition;
     for (size_t i = 0; i < n_nodes; i++)
     {
@@ -437,16 +436,15 @@
 }
 
 std::vector<std::pair<Nodes, float>> generate_dendrogram(
     GraphNeighbors &graph_neighbors,
     GraphWeights &graph_weights,
     float resolution,
     bool prune,
-    bool full,
-    bool z_modularity)
+    bool full)
 {
     float mod;
     float new_mod;
 
     std::vector<std::pair<Nodes, float>> partition_list;
     GraphNeighbors communities;
     size_t n_nodes = graph_neighbors.size();
@@ -454,31 +452,33 @@
     // init_status
     auto [node2com,
           internals,
           loops,
           degrees,
           gdegrees,
           total_weight] = init_status(graph_neighbors, graph_weights);
+
     // one_level
-    if (prune)
-        one_level_prune(graph_neighbors, graph_weights,
-                        node2com, internals, loops, degrees, gdegrees,
-                        total_weight, resolution, z_modularity);
-    else
+    if (!prune)
         one_level(graph_neighbors, graph_weights,
                   node2com, internals, loops, degrees, gdegrees,
-                  total_weight, resolution, z_modularity);
+                  total_weight, resolution);
+    else
+        one_level_prune(graph_neighbors, graph_weights,
+                        node2com, internals, loops, degrees, gdegrees,
+                        total_weight, resolution);
 
     // new_mod
     new_mod = modularity(
-        internals, degrees, total_weight, resolution, z_modularity);
+        internals, degrees, total_weight, resolution);
 
     // renumber
     std::tie(communities, node2com) = renumber(
         graph_neighbors, graph_weights, node2com);
+
     // partition_list
     partition_list.push_back(
         std::make_pair(get_partition(node2com, n_nodes), new_mod));
 
     mod = new_mod;
     // induced graph
     std::tie(graph_neighbors, graph_weights, n_nodes) = induced_graph(
@@ -490,40 +490,38 @@
              loops,
              degrees,
              gdegrees,
              total_weight) = init_status(graph_neighbors, graph_weights);
 
     while (true)
     {
-        if (prune)
-        {
-            one_level_prune(graph_neighbors, graph_weights,
-                            node2com, internals, loops, degrees, gdegrees,
-                            total_weight, resolution, z_modularity);
-        }
-        else
-        {
+        if (!prune)
             one_level(graph_neighbors, graph_weights,
                       node2com, internals, loops, degrees, gdegrees,
-                      total_weight, resolution, z_modularity);
-        }
+                      total_weight, resolution);
+        else
+            one_level_prune(graph_neighbors, graph_weights,
+                            node2com, internals, loops, degrees, gdegrees,
+                            total_weight, resolution);
+
         new_mod = modularity(
-            internals, degrees, total_weight, resolution, z_modularity);
+            internals, degrees, total_weight, resolution);
+
         if (new_mod - mod < 0.0000001)
-        {
             break;
-        }
 
         std::tie(communities, node2com) = renumber(
             graph_neighbors, graph_weights, node2com);
         mod = new_mod;
         partition_list.push_back(
             std::make_pair(get_partition(node2com, n_nodes), new_mod));
+
         std::tie(graph_neighbors, graph_weights, n_nodes) = induced_graph(
             graph_neighbors, graph_weights, communities, node2com);
+
         std::tie(node2com,
                  internals,
                  loops,
                  degrees,
                  gdegrees,
                  total_weight) = init_status(graph_neighbors, graph_weights);
     }
@@ -532,30 +530,30 @@
     {
         size_t node2com_size = node2com.size();
         while (true)
         {
             // one iteration
             one_step(graph_neighbors, graph_weights,
                      node2com, internals, loops, degrees, gdegrees,
-                     total_weight, resolution, z_modularity);
+                     total_weight, resolution);
             new_mod = modularity(
-                internals, degrees, total_weight, resolution, z_modularity);
+                internals, degrees, total_weight, resolution);
             std::tie(communities, node2com) = renumber(
                 graph_neighbors, graph_weights, node2com);
             partition_list.push_back(
                 std::make_pair(get_partition(node2com, n_nodes), new_mod));
             std::tie(graph_neighbors, graph_weights, n_nodes) = induced_graph(
                 graph_neighbors, graph_weights, communities, node2com);
             std::tie(node2com,
                      internals,
                      loops,
                      degrees,
                      gdegrees,
                      total_weight) = init_status(graph_neighbors, graph_weights);
-            if (node2com.size() == node2com_size)
+            if (node2com.size() == node2com_size || node2com.size() == 1)
                 break;
 
             node2com_size = node2com.size();
         }
     }
     return partition_list;
 }
```

### Comparing `weavenn-0.0.5/src/louvain.hpp` & `weavenn-1.0.0/src/louvain.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     GraphNeighbors const &graph_neighbors,
     GraphWeights const &graph_weights);
 
 float modularity(
     Weights const &internals,
     Weights const &degrees,
     float total_weight,
-    float resolution,
-    bool z_modularity);
+    float resolution);
 
 WeightMap neighcom(
     GraphNeighbors const &graph_neighbors,
     GraphWeights const &graph_weights,
     Nodes const &node2com,
     Node node);
 
@@ -33,40 +32,37 @@
     GraphWeights const &graph_weights,
     Nodes &node2com,
     Weights &internals,
     Weights const &loops,
     Weights &degrees,
     Weights const &gdegrees,
     float total_weight,
-    float resolution,
-    bool z_modularity);
+    float resolution);
 
 void one_level_prune(
     GraphNeighbors const &graph_neighbors,
     GraphWeights const &graph_weights,
     Nodes &node2com,
     Weights &internals,
     Weights const &loops,
     Weights &degrees,
     Weights const &gdegrees,
     float total_weight,
-    float resolution,
-    bool z_modularity);
+    float resolution);
 
 void one_step(
     GraphNeighbors const &graph_neighbors,
     GraphWeights const &graph_weights,
     Nodes &node2com,
     Weights &internals,
     Weights const &loops,
     Weights &degrees,
     Weights const &gdegrees,
     float total_weight,
-    float resolution,
-    bool z_modularity);
+    float resolution);
 
 std::tuple<GraphNeighbors, Nodes> renumber(
     GraphNeighbors const &graph_neighbors,
     GraphWeights const &graph_weights,
     Nodes const &node2com);
 
 std::tuple<GraphNeighbors, GraphWeights, size_t> induced_graph(
@@ -78,9 +74,8 @@
 Nodes get_partition(Nodes const &node2com, size_t n_nodes);
 
 std::vector<std::pair<Nodes, float>> generate_dendrogram(
     GraphNeighbors &graph_neighbors,
     GraphWeights &graph_weights,
     float resolution,
     bool prune,
-    bool full,
-    bool z_modularity);
+    bool full);
```

