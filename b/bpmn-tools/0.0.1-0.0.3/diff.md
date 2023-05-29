# Comparing `tmp/bpmn-tools-0.0.1.tar.gz` & `tmp/bpmn-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpmn-tools-0.0.1.tar", last modified: Fri May  5 06:48:11 2023, max compression
+gzip compressed data, was "bpmn-tools-0.0.3.tar", last modified: Mon May 29 16:19:35 2023, max compression
```

## Comparing `bpmn-tools-0.0.1.tar` & `bpmn-tools-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,35 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-05 06:48:11.261815 bpmn-tools-0.0.1/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-05 06:48:11.259508 bpmn-tools-0.0.1/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     1048 2023-05-04 19:30:59.000000 bpmn-tools-0.0.1/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.0.1/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.0.1/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1662 2023-05-05 06:48:11.261702 bpmn-tools-0.0.1/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-05 06:48:11.259718 bpmn-tools-0.0.1/bpmn_tools/
--rw-r--r--   0 xtof       (501) staff       (20)       91 2023-04-16 19:01:44.000000 bpmn-tools-0.0.1/bpmn_tools/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     8229 2023-05-04 19:13:15.000000 bpmn-tools-0.0.1/bpmn_tools/diagrams.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-05 06:48:11.260582 bpmn-tools-0.0.1/bpmn_tools.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     1662 2023-05-05 06:48:11.000000 bpmn-tools-0.0.1/bpmn_tools.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-05 06:48:11.000000 bpmn-tools-0.0.1/bpmn_tools.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-05-05 06:48:11.000000 bpmn-tools-0.0.1/bpmn_tools.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       48 2023-05-05 06:48:11.000000 bpmn-tools-0.0.1/bpmn_tools.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       15 2023-05-05 06:48:11.000000 bpmn-tools-0.0.1/bpmn_tools.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       22 2023-05-05 06:48:11.000000 bpmn-tools-0.0.1/bpmn_tools.egg-info/top_level.txt
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-05 06:48:11.261026 bpmn-tools-0.0.1/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.0.1/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.0.1/docs/conf.py
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-05-05 06:48:11.261854 bpmn-tools-0.0.1/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1458 2023-04-16 17:05:11.000000 bpmn-tools-0.0.1/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-05 06:48:11.261423 bpmn-tools-0.0.1/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.0.1/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    11607 2023-05-04 19:39:00.000000 bpmn-tools-0.0.1/tests/test_hello.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.984204 bpmn-tools-0.0.3/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.980168 bpmn-tools-0.0.3/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.0.3/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.0.3/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.0.3/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-05-29 16:19:35.984077 bpmn-tools-0.0.3/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.981713 bpmn-tools-0.0.3/bpmn_tools/
+-rw-r--r--   0 xtof       (501) staff       (20)      670 2023-05-29 16:18:58.000000 bpmn-tools-0.0.3/bpmn_tools/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-05-29 15:02:23.000000 bpmn-tools-0.0.3/bpmn_tools/collaboration.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4422 2023-05-29 15:05:14.000000 bpmn-tools-0.0.3/bpmn_tools/diagrams.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3027 2023-05-29 15:06:20.000000 bpmn-tools-0.0.3/bpmn_tools/flow.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.982517 bpmn-tools-0.0.3/bpmn_tools/layout/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.0.3/bpmn_tools/layout/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3446 2023-05-29 15:19:24.000000 bpmn-tools-0.0.3/bpmn_tools/layout/simple.py
+-rw-r--r--   0 xtof       (501) staff       (20)      632 2023-05-27 14:21:17.000000 bpmn-tools-0.0.3/bpmn_tools/notation.py
+-rw-r--r--   0 xtof       (501) staff       (20)      641 2023-05-26 11:11:01.000000 bpmn-tools-0.0.3/bpmn_tools/util.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.0.3/bpmn_tools/visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3789 2023-05-27 19:24:16.000000 bpmn-tools-0.0.3/bpmn_tools/xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.982333 bpmn-tools-0.0.3/bpmn_tools.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      597 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       48 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       24 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       22 2023-05-29 16:19:35.000000 bpmn-tools-0.0.3/bpmn_tools.egg-info/top_level.txt
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.982893 bpmn-tools-0.0.3/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.0.3/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.0.3/docs/conf.py
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-05-29 16:19:35.984257 bpmn-tools-0.0.3/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.0.3/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-29 16:19:35.983760 bpmn-tools-0.0.3/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.0.3/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    10316 2023-05-29 15:17:23.000000 bpmn-tools-0.0.3/tests/test_hello.py
+-rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.0.3/tests/test_visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.0.3/tests/test_xml.py
```

### Comparing `bpmn-tools-0.0.1/LICENSE.txt` & `bpmn-tools-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.0.1/docs/conf.py` & `bpmn-tools-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.0.1/setup.py` & `bpmn-tools-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   
 ]
 INSTALL_REQUIRES = [
   "fire",
   "xmltodict",
+  "colorama",
   
 ]
 ENTRY_POINTS = {
   "console_scripts" : [
     "bt=bpmn_tools.__main__:cli",
     
   ]
```

### Comparing `bpmn-tools-0.0.1/tests/test_hello.py` & `bpmn-tools-0.0.3/tests/test_hello.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,34 +2,21 @@
   Initial tests to drive development entirely from tests ;-)
   TDD rules 💪
   The tests build towards a complete support to construct the hello.bpmn example
 """
 
 from pathlib import Path
 import xmltodict
-import json
-from difflib import unified_diff
 
-from bpmn_tools.diagrams import Definitions
-from bpmn_tools.diagrams import Process, Start, End, Task, Flow
-from bpmn_tools.diagrams import Collaboration, Participant
-from bpmn_tools.diagrams import Diagram, Plane, Shape, Edge
-
-def show_diff(result, expected):
-  def as_dict(obj):
-    return obj.as_dict()
-  result   = json.dumps(expected, indent=2, sort_keys=True, default=as_dict)
-  expected = json.dumps(result,   indent=2, sort_keys=True, default=as_dict)
-  diff = unified_diff(result.splitlines(keepends=True),
-                      expected.splitlines(keepends=True))
-  print("".join(diff), end="")
-
-def compare(result, expected):
-  show_diff(result, expected)
-  assert result == expected
+from bpmn_tools.notation      import Definitions
+from bpmn_tools.collaboration import Collaboration, Participant
+from bpmn_tools.flow          import Process, Start, End, Task, Flow
+from bpmn_tools.diagrams      import Diagram, Plane, Shape, Edge
+
+from bpmn_tools.util import compare
 
 def test_create_single_step_process():
   """
     Create a single-step process.
     (start) -> (task: Say "Hello!") -> (end)
   
     <bpmn:process id="process" isExecutable="true">
@@ -54,15 +41,15 @@
   ]
 
   process = Process(id="process").extend(activities).extend([
     Flow(source=activities[0], target=activities[1]),
     Flow(source=activities[1], target=activities[2])
   ])
 
-  compare(process.as_dict(), {
+  compare(process.as_dict(with_tag=True), {
     "bpmn:process": {
       "@id": "process",
       "bpmn:startEvent": {
         "@id": "start",
         "bpmn:outgoing": "flow_start_hello"
       },
       "bpmn:task": {
@@ -89,38 +76,38 @@
       ]
     }
   })
 
 def test_create_single_participant_collaboration():
   """
     Create a single participant collaboration for Process(id="process")
-  
+
     <bpmn:collaboration id="collaboration">
       <bpmn:participant id="participant" name="lane" processRef="process" />
     </bpmn:collaboration>
   """
   collaboration = Collaboration(id="collaboration").append(
     Participant("participant", Process(id="process"), id="participant")
   )
-  
-  compare(collaboration.as_dict(), {
+
+  compare(collaboration.as_dict(with_tag=True), {
     "bpmn:collaboration": {
       "@id": "collaboration",
       "bpmn:participant": {
         "@id": "participant",
         "@name": "participant",
         "@processRef": "process"
       }
     }
   })
 
 def test_create_definitions_with_process_and_collaboration():
   """
     Create Definitions with both a single-step process and collaboration.
-  
+
     <bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL"
                       xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI"
                       xmlns:dc="http://www.omg.org/spec/DD/20100524/DC"
                       xmlns:di="http://www.omg.org/spec/DD/20100524/DI"
                       xmlns:modeler="http://camunda.org/schema/modeler/1.0"
                       id="definitions">
       <bpmn:collaboration id="collaboration">
@@ -148,25 +135,25 @@
     End(id="end")
   ]
 
   process = Process(id="process").extend(activities).extend([
     Flow(source=activities[0], target=activities[1]),
     Flow(source=activities[1], target=activities[2])
   ])
-  
+
   collaboration = Collaboration(id="collaboration").append(
     Participant("participant", process, id="participant")
   )
-  
+
   definitions = Definitions(id="definitions").extend([
     process,
     collaboration
   ])
-  
-  compare(definitions.as_dict(), {
+
+  compare(definitions.as_dict(with_tag=True), {
     "bpmn:definitions": {
       "@xmlns:bpmn": "http://www.omg.org/spec/BPMN/20100524/MODEL",
       "@xmlns:bpmndi": "http://www.omg.org/spec/BPMN/20100524/DI",
       "@xmlns:dc": "http://www.omg.org/spec/DD/20100524/DC",
       "@xmlns:di": "http://www.omg.org/spec/DD/20100524/DI",
       "@id": "definitions",
       "bpmn:process": {
@@ -215,16 +202,16 @@
 
     <bpmndi:BPMNShape id="shape_start" bpmnElement="start">
       <dc:Bounds x="179" y="99" width="36" height="36" />
     </bpmndi:BPMNShape>
   """
 
   shape = Shape(Start(id="start"))
-  
-  compare(shape.as_dict(), {
+
+  compare(shape.as_dict(with_tag=True), {
     "bpmndi:BPMNShape": {
       "@id": "shape_start",
       "@bpmnElement": "start",
       "dc:Bounds": {
         "@x": "0",
         "@y": "0",
         "@width": "36",
@@ -232,24 +219,24 @@
       }
     }
   })
 
 def test_create_task_shape():
   """
     Create a shape for a Task element, with default bounds
-  
+
     <bpmndi:BPMNShape id="shape_hello" bpmnElement="hello">
       <dc:Bounds x="270" y="77" width="100" height="80" />
       <bpmndi:BPMNLabel />
     </bpmndi:BPMNShape>
   """
 
   shape = Shape(Task(id="hello"))
-  
-  compare(shape.as_dict(), {
+
+  compare(shape.as_dict(with_tag=True), {
     "bpmndi:BPMNShape": {
       "@id": "shape_hello",
       "@bpmnElement": "hello",
       "dc:Bounds": {
         "@x": "0",
         "@y": "0",
         "@width": "100",
@@ -257,26 +244,26 @@
       },
       "bpmndi:BPMNLabel": None
     }
   })
 
 def test_create_edge():
   """
-    Create an edge for a flow between start and 
+    Create an edge for a flow between start and
 
     <bpmndi:BPMNEdge id="edge_flow_start_hello" bpmnElement="flow_start_hello">
       <di:waypoint x="215" y="117" />
       <di:waypoint x="270" y="117" />
     </bpmndi:BPMNEdge>
   """
 
   flow = Flow(source=Start(id="start"), target=Task(id="hello"))
   edge = Edge(flow)
-  
-  compare(edge.as_dict(), {
+
+  compare(edge.as_dict(with_tag=True), {
     "bpmndi:BPMNEdge": {
       "@id": "edge_flow_start_hello",
       "@bpmnElement": "flow_start_hello",
       "di:waypoint": [
         {
           "@x": "36",
           "@y": "18"
@@ -288,49 +275,49 @@
       ]
     }
   })
 
 def test_empty_diagram():
   """
     An empty diagram, always contains a plane.
-  
+
     <bpmndi:BPMNDiagram id="diagram">
       <bpmndi:BPMNPlane id="plane">
       </bpmndi:BPMNPlane>
     </bpmndi:BPMNDiagram>
   """
-  
+
   diagram = Diagram(id="diagram")
 
-  compare(diagram.as_dict(), {
+  compare(diagram.as_dict(with_tag=True), {
     "bpmndi:BPMNDiagram": {
       "@id": "diagram",
       "bpmndi:BPMNPlane": {
         "@id": "plane"
       }
     }
   })
 
 def test_plane_for_collaboration_with_one_participant_without_a_process():
   """
     A plane for a collaboration with on participant.
-  
+
     <bpmndi:BPMNPlane id="plane_collaboration" bpmnElement="collaboration">
       <bpmndi:BPMNShape id="participant_di" bpmnElement="participant" isHorizontal="true">
         <dc:Bounds x="129" y="57" width="600" height="123" />
         <bpmndi:BPMNLabel />
       </bpmndi:BPMNShape>
     </bpmndi:BPMNPlane>
   """
   collaboration = Collaboration(id="collaboration").append(
     Participant("participant", None, id="participant")
   )
   plane = Plane(id="plane", element=collaboration)
 
-  compare(plane.as_dict(), {
+  compare(plane.as_dict(with_tag=True), {
     "bpmndi:BPMNPlane": {
       "@id": "plane_collaboration",
       "@bpmnElement": "collaboration",
       "bpmndi:BPMNShape": {
         "@id": "shape_participant",
         "@bpmnElement": "participant",
         "@isHorizontal": "true",
@@ -340,50 +327,16 @@
           "@width": "600",
           "@height": "125"
         }
       }
     }
   })
 
-def test_participants_elements_and_flows():
-  activities = [
-    Start(id="start"),
-    Task('Say "Hello!"', id="hello"),
-    End(id="end")
-  ]
-  
-  flows = [
-    Flow(source=activities[0], target=activities[1]),
-    Flow(source=activities[1], target=activities[2])
-  ]
-
-  process = Process(id="process").extend(activities).extend(flows)
-
-  participant = Participant("participant", process, id="participant")
-  
-  compare(participant.elements, activities)
-  compare(participant.flows, flows)
-
-def test_collaboration_passing_through_elements ():
-  activities = [
-    Start(id="start"),
-    Task('Say "Hello!"', id="hello"),
-    End(id="end")
-  ]
-  
-  process = Process(id="process").extend(activities)
-
-  participant = Participant("participant", process, id="participant")
-  
-  collaboration = Collaboration(id="collaboration").append(participant)
-  
-  compare(collaboration.elements, [ participant ] + activities)
-  
 def test_hello():
-  with open(Path(__file__).resolve().parent / ".." / "examples" / "hello.bpmn") as fp:
+  with open(Path(__file__).resolve().parent / "hello.bpmn") as fp:
     expected = xmltodict.parse(fp.read())
 
   activities = [
     Start(id="start"),
     Task('Say "Hello!"', id="hello"),
     End(id="end")
   ]
@@ -398,15 +351,17 @@
   )
 
   definitions = Definitions(id="definitions").extend([
     process,
     collaboration,
   ])
 
-  definitions.diagrams.append(
+  definitions.append(
     Diagram(
       id="diagram",
       plane=Plane(id="plane", element=collaboration)
     )
   )
 
-  compare(definitions.as_dict(), expected)
+  result = definitions.as_dict(with_tag=True)
+  
+  compare(result, expected)
```

