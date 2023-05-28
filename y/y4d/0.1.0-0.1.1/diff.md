# Comparing `tmp/y4d-0.1.0.tar.gz` & `tmp/y4d-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y4d-0.1.0.tar", max compression
+gzip compressed data, was "y4d-0.1.1.tar", max compression
```

## Comparing `y4d-0.1.0.tar` & `y4d-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      580 2023-05-27 20:21:25.146819 y4d-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      106 2023-05-27 19:34:50.001818 y4d-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.0/y4d/__init__.py
--rw-r--r--   0        0        0     1568 2023-05-27 20:05:04.914421 y4d-0.1.0/y4d/checkAPI.py
--rw-r--r--   0        0        0    14925 2023-05-27 19:56:35.338217 y4d-0.1.0/y4d/codeParser.py
--rw-r--r--   0        0        0     8205 2023-05-27 20:35:11.728151 y4d-0.1.0/y4d/commentController.py
--rw-r--r--   0        0        0     6413 2023-05-27 20:35:23.254615 y4d-0.1.0/y4d/isolator.py
--rw-r--r--   0        0        0    35898 2023-05-27 20:35:46.942835 y4d-0.1.0/y4d/restrictor.py
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 y4d-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      580 2023-05-28 22:50:51.549371 y4d-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-05-27 19:34:50.001818 y4d-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.1/y4d/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-28 22:40:01.005087 y4d-0.1.1/y4d/checkAPI.py
+-rw-r--r--   0        0        0    15423 2023-05-28 22:39:33.928475 y4d-0.1.1/y4d/codeParser.py
+-rw-r--r--   0        0        0     8205 2023-05-28 22:40:55.151188 y4d-0.1.1/y4d/commentController.py
+-rw-r--r--   0        0        0     6413 2023-05-28 22:41:16.788704 y4d-0.1.1/y4d/isolator.py
+-rw-r--r--   0        0        0    35699 2023-05-28 22:41:39.466605 y4d-0.1.1/y4d/restrictor.py
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 y4d-0.1.1/PKG-INFO
```

### Comparing `y4d-0.1.0/pyproject.toml` & `y4d-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "y4d"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["BahouA <antonbahou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 checkAPI = "y4d.checkAPI:app"
 restrict = "y4d.restrictor:app"
```

### Comparing `y4d-0.1.0/y4d/checkAPI.py` & `y4d-0.1.1/y4d/checkAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 app = typer.Typer()
 
 #Function to restrict a single (private/public/protected) function, no need for the YAML file, further explanation available exactly below function definition.
 @app.command("")
 def main(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
         compare: str = typer.Argument(..., help="The path of the .cpp or .h file the user wants the source file to be compared to."),
         restriction: str = typer.Argument(..., help="The restriction type used for 2 ways of checking:\n\nat_least: Everything being checked must exist (It can be with other functions/classes).\n\nexactly: Everything being checked must only exist (It can not be with other functions/classes)."),
-        output: str  = typer.Option("n", "-o", help="If # this will make checkAPI print the number of missing functions/classes then extra functions/classes, Input V if you want a list of violations to be printed and more information (default is #) (Takes only v or V or #)."),
+        output: str  = typer.Option("n", "-o", help="If n this will make checkAPI print the number of missing functions/classes then extra functions/classes, Input V if you want a list of violations to be printed and more information (default is n) (Takes only v or V or n or N)."),
         hide:bool = typer.Argument(False, hidden=True, help="A hidden variable for developers use, used to return extra functions and classes found in the code.")):
     """
     This tool will compare two files together, the source and compare file, it will check if the function prototypes and class names match then return true or false accordingly.
     """
     restrictor.checkAPI(source, restriction, compare, output, hide)
```

### Comparing `y4d-0.1.0/y4d/codeParser.py` & `y4d-0.1.1/y4d/codeParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 pos += [start, end, type, item['access_type']] 
     if type == "decstructor":
         for item in data['nodes']:
             if item['kind'] == "DESTRUCTOR" and item['spelling'].replace(" ", "") == name:
                 end = item['end']
                 start = item['start']
                 pos += [start, end, type, item['access_type']] 
-        
+    
     return pos
 
 def findLocationClass(data, prototype: str, source, type: str, iteration = 0):
     #classes list stores all classes that inherits from\friend with main class in order to parse their member functions and nested classes  
     classes =  [prototype]
     pos=[]
     for class_i in classes:
@@ -165,14 +165,20 @@
                 if item['mangled_name'].startswith('?'):
                     mangledName= item['mangled_name'].split("@")
                     if len(mangledName) > 1 and mangledName[1] == name:
                         if item['kind'] == "CXX_METHOD":
                             returnType = item['prototype'].split(" ")[0]
                             func_prototype = returnType +" " + name + "::" +item['displayname']
                             pos+= findLocationFunction(data, func_prototype, source)
+                    if (item['kind'] == "CONSTRUCTOR" or item['kind'] == "DESTRUCTOR" )and item['parent_class'] == "class "+ name:
+                        returnType = item['prototype'].split(" ")[0]
+                        func_prototype = name + "::" +item['displayname']
+                        if item["initializer_list"] == "true":
+                            func_prototype += "("
+                        pos+= findLocationFunction(data, func_prototype, source)
             #check template member functions  
             if item["kind"] == "FUNCTION_TEMPLATE":
                 start_line = item['start']
                 j = i+1
                 template_node = data['nodes'][j]
                 while  j < len(data['nodes']) and template_node['start'] == start_line:
                     if template_node['kind'] == "TEMPLATE_TYPE_PARAMETER":
@@ -209,21 +215,21 @@
     return False
 def prepareData (source: str, hide: bool):
     
     index = clang.cindex.Index.create()
     tu = index.parse(source)
     
     #check if source code compiles
-    if len(tu.diagnostics) > 0:
-        print("Error: " + source + " doesn't compile successfully")
-        return ["error"]
+    if hide:
+        if len(tu.diagnostics) > 0:
+            print("Error: " + source + " doesn't compile successfully")
+            return ["error"]
 
     #comment out libraries and include in source file
-    if hide:
-        commentController.includePreparer(source)
+    commentController.includePreparer(source)
     
     #Call again with code without libraries and using namespace
     index = clang.cindex.Index.create()
     tu = index.parse(source)
     
     output = {"nodes": []}
     friendFlag = False
@@ -235,40 +241,41 @@
         #Check if the constructor has an expression initializer list
         if node.kind == clang.cindex.CursorKind.CONSTRUCTOR:
             if hasInitializerList(node):
                 initializer_list = "true"
                 
         #Save access type of member functions, anything else will have value "invalid"              
         access_type = str(node.access_specifier).split(".")[1]
+        
         #Save name of parent class
         if access_type == "INVALID":
             parent_class = ""
         else:
             parent = node.semantic_parent
             if parent is None:
                 parent_class=""
             elif parent.kind == clang.cindex.CursorKind.CLASS_DECL:
                 parent_class = "class " + str(parent.spelling)
             elif parent.kind == clang.cindex.CursorKind.STRUCT_DECL:
                 parent_class = "struct " + str(parent.spelling)
             
-        if node.kind == clang.cindex.CursorKind.CLASS_DECL:
+        if node.kind == clang.cindex.CursorKind.CLASS_DECL or node.kind == clang.cindex.CursorKind.STRUCT_DECL:
             classPointer = 0
             friendFlag = False
             
         elif node.kind == clang.cindex.CursorKind.CXX_BASE_SPECIFIER:
             inh = node.spelling
             output["nodes"][classPointer]["inherits_from"].append(inh)
 
         elif node.kind == clang.cindex.CursorKind.FRIEND_DECL:
             friendFlag = True
 
         elif friendFlag:
             friend = node.spelling
-            if len(friend.split("class")) == 1: #check this: or len(friend.split("struct")):
+            if len(friend.split("class")) == 1 and len(friend.split("struct")) == 1:
                 friend = node.type.spelling.split('(')[0] + node.displayname
             output["nodes"][classPointer]["friend_with"].append(friend)
             friendFlag = False
 
         classPointer = classPointer - 1
         node_dict = {
             "kind": str(node.kind.name),
@@ -292,18 +299,17 @@
             "parent_class" : parent_class,
             "initializer_list" : initializer_list,
         }
         output["nodes"].append(node_dict)
     
     jsonFormat = json.dumps(output, indent=4)
     data = json.loads(jsonFormat)
-
+    
     # Revert commenting changes done before
-    if hide:
-        commentController.includeRevert(source)
+    commentController.includeRevert(source)
     return data
 
 def positions ( source: str, type: str, prototype: str, option = 0):
     source_path = Path(source)
     if source_path.exists() == False:
         print("Error: " + source + " doesn't exist")
         return ["error"]
@@ -327,8 +333,7 @@
     if type == "class" or type == "struct":
         pos = findLocationClass(data, prototype , source, type, option)  
         
     if type == "function":
         pos = findLocationFunction( data, prototype, source)  
         
     return pos
-
```

### Comparing `y4d-0.1.0/y4d/commentController.py` & `y4d-0.1.1/y4d/commentController.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.0/y4d/isolator.py` & `y4d-0.1.1/y4d/isolator.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.0/y4d/restrictor.py` & `y4d-0.1.1/y4d/restrictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,29 +59,25 @@
     """
     #Used to control the style of output
     if output not in ["n", "N", "V", "v"]:
         print("Invalid -o input")
         return False
     
     outputBool = False
-    if output == "#":
+    if output == "n" or output == "N":
         outputBool = True
 
-    #Just to increase speed of code, this is explained in prepare data in codeparser
-    if not hide2:
-        commentController.includePreparer(source)
-
     with open(rules) as file:
         yamlFile = yaml.load(file, Loader=yaml.FullLoader)
     jsonFormat = json.dumps(yamlFile, indent=4)
     jsonData = json.loads(jsonFormat)
 
     #Used to remove comments from file, important for all restrictors (library only one that needs to work without it)
     newSource = "commentDeletedFileForRestrictor.cpp"
-    commentController.delete_comments(source, newSource)
+    commentController.deleteComments(source, newSource)
 
     #Following variables are needed to print everything in a readable manner for the user and for the loop to function correctly
     critOld = "start"
     critAns = True
     exactCount = 0
     compareCount = 0
     parentCheck = []
@@ -183,23 +179,23 @@
                             if not hide:
                                 print("Missing class: " + cls)
                             else:
                                 print("Extra class: " + cls)
                     exactCount += 1
                     if exactCount == 1:
                         if critData['scope'].lower() == "global" or critData['scope'] == "":
-                            data = codeParser.prepareData(newSource, False)
+                            data = codeParser.prepareData(newSource, True)
                             if data == ["error"]:
                                 return False
                         else:
                             scopeG = scopeGetter(newSource, critData['scope'])
                             file = open("restrictorGen.cpp", "w")
                             file.write(scopeG)
                             file.close()
-                            data = codeParser.prepareData("restrictorGen.cpp", False)
+                            data = codeParser.prepareData("restrictorGen.cpp", True)
                             if data == ["error"]:
                                 return False
                         for decl in data['nodes']:
                             if decl['kind'] == "CLASS_DECL" and decl['start'] != decl['end']:
                                 compareCount += 1
 
         #Handles functions in YAML file
@@ -224,23 +220,23 @@
                             if not hide:
                                 print("Missing function: " + func)
                             else:
                                 print("Extra function: " + func)
                     exactCount += 1
                     if exactCount == 1:
                         if critData['scope'].lower() == "global" or critData['scope'] == "":
-                             data = codeParser.prepareData(newSource, False)
+                             data = codeParser.prepareData(newSource, True)
                              if data == ["error"]:
                                 return False
                         else:
                             scopeG = scopeGetter(newSource, critData['scope'])
                             file = open("restrictorGen.cpp", "w")
                             file.write(scopeG)
                             file.close()
-                            data = codeParser.prepareData("restrictorGen.cpp", False)
+                            data = codeParser.prepareData("restrictorGen.cpp", True)
                             if data == ["error"]:
                                 return False
                         for decl in data['nodes']:
                             if decl['kind'] == "FUNCTION_DECL" and decl['start'] != decl['end']:
                                 compareCount += 1
 
         #Handles (private/public/protected) functions in YAML file
@@ -266,23 +262,23 @@
                             if not hide:
                                 print("Missing " + access + " function: " + func)
                             else:
                                 print("Extra " + access + " function: " + func)
                     exactCount += 1
                     if exactCount == 1:
                         if critData['scope'].lower() == "global" or critData['scope'] == "":
-                             data = codeParser.prepareData(newSource, False)
+                             data = codeParser.prepareData(newSource, True)
                              if data == ["error"]:
                                 return False
                         else:
                             scopeG = scopeGetter(newSource, critData['scope'])
                             file = open("restrictorGen.cpp", "w")
                             file.write(scopeG)
                             file.close()
-                            data = codeParser.prepareData("restrictorGen.cpp", False)
+                            data = codeParser.prepareData("restrictorGen.cpp", True)
                             if data == ["error"]:
                                 return False
                         for decl in data['nodes']:
                             if decl['kind'] == "CXX_METHOD" and decl['access_type'] == access and (decl['start'] != decl['end'] or decl['is_virtual_method'] == True):
                                 if decl['is_virtual_method'] == True:
                                     if decl['parent_class'] in parentCheck:
                                         compareCount -= 1
@@ -294,17 +290,14 @@
     if exactCount != 0 and compareCount != exactCount:
         critAns = critAns & False
     if critData['restriction'].lower() == "exactly" and not critAns and not outputBool and not hide:
         print(critOld + " are not exactly the same.")
     if outputBool:
         print(violationCount)
     
-    #Just to increase speed of code, this is explained in prepare data in codeparser
-    if not hide2:
-        commentController.includeRevert(source)
 
 
 
 #Function to restrict a single library, no need for the YAML file, further explanation available exactly below function definition
 @app.command("l")
 def libRestrict(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
                  restriction: str = typer.Argument(..., help="The restriction type used for 3 ways of checking:\n\nat_least: The library being checked must exist (It can be with other libraries).\n\nexactly: The library being checked must only exist (It can not be with other libraries).\n\nforbidden: The library being checked must not exist."),
@@ -427,21 +420,23 @@
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user
     if scope.lower() == "global" or scope == "":
-        data = codeParser.prepareData(source, False)
+        data = codeParser.prepareData(source, True)
         if data == ["error"]:
             return False
         with open(source, 'r') as f:
             scopeG = f.read()
     else:
         scopeG = scopeGetter(source, scope)
+        if scopeG == ["error"]:
+            return False
         file = open("restrictorGen.cpp", "w")
         file.write(scopeG)
         file.close()
         data = codeParser.prepareData("restrictorGen.cpp", False)
         if data == ["error"]:
             return False
 
@@ -492,21 +487,23 @@
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user
     if scope.lower() == "global" or scope == "":
-        data = codeParser.prepareData(source, False)
+        data = codeParser.prepareData(source, True)
         if data == ["error"]:
             return False
         with open(source, 'r') as f:
             scopeG = f.read()
     else:
         scopeG = scopeGetter(source, scope)
+        if scopeG == ["error"]:
+            return False
         file = open("restrictorGen.cpp", "w")
         file.write(scopeG)
         file.close()
         data = codeParser.prepareData("restrictorGen.cpp", False)
         if data == ["error"]:
             return False
     
@@ -515,15 +512,15 @@
     prototypeName = prototype.split("(")[0] + "\s*"
     prototypeName += '('
     prototypeVars = prototype.split("(")[1].split(")")[0].split(",")
     prototypeRegex = "(?:(?<=\s)|(?<=^))" + prototypeName
     for p in prototypeVars:
         prototypeRegex += ".*" + p.strip().split(' ')[0] + ".*,"
     prototypeRegex = prototypeRegex[:-1] + ').*\n*.*{[\s\S]*}(?=\s|$)'
-    
+
     empty = []
     #Check if function exists and print true or false according to restriction
     if codeParser.findLocationFunction(data, prototype, source) != empty:
         if restriction.lower() == "exactly":
             if len(re.findall(r"\b[a-zA-Z_][a-zA-Z0-9_]*\s+[a-zA-Z_][a-zA-Z0-9_]*\s*\([^)]*\)\s*\{[^{}]*\}", scopeG, flags=re.MULTILINE)) > 1:
                 if not hide:
                     print("False")
@@ -566,21 +563,23 @@
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user as well as preparing data for access_type search
     if scope.lower() == "global" or scope == "":
-        data = codeParser.prepareData(source, False)
+        data = codeParser.prepareData(source, True)
         if data == ["error"]:
             return False
     else:
-        data = scopeGetter(source, scope)
+        scopeG = scopeGetter(source, scope)
+        if scopeG == ["error"]:
+            return False
         file = open("restrictorGen.cpp", "w")
-        file.write(data)
+        file.write(scopeG)
         file.close()
         data = codeParser.prepareData("restrictorGen.cpp", False)
         if data == ["error"]:
             return False
 
     #Variables used in the following if statement to find if function is private
     if len(prototype.split("virtual")) == 1 and len(prototype.split("static")) == 1:
@@ -607,74 +606,72 @@
     """
     This tool will compare two files together, the source and compare file, it will check if the function prototypes and class names match then return true or false accordingly.
     """
     #Used to control the style of output
     if output not in ["n", "N", "V", "v"]:
         print("Invalid -o input")
         return False
-    
-    #Just to increase speed of code, this is explained in prepare data in codeparser
-    commentController.includePreparer(source)
-    
+
+    data = codeParser.prepareData(compare, True)
+    if data == ["error"]:
+        return False
+
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Varibales and loop used to create the YAML file needed to run restrictor, YAML file made from compare file.
     allPrivFunctions = []
     allPublicFunctions =[]
     allProtectedFunctions = []
     allFunctions = []
     allClasses = []
-    data = codeParser.prepareData(compare, True)
-    if data == ["error"]:
-        return False
-    if data == 'error':
-        return False
     virtual = ""
     const = ""
+    unsigned = ""
     for decl in data['nodes']:
+        if decl['prototype'].split(' ')[0] == "unsigned":
+            unsigned = " " + decl['prototype'].split(' ')[1]
+        else:
+            unsigned = ""
         if decl['kind'] == "CXX_METHOD":
             if decl['is_virtual_method'] == True:
                 virtual = "virtual "
             else:
                 virtual = ""
             if decl['is_const_method'] == True:
                 const = " const"
             else:
                 const = ""
             if decl['access_type'] == "":
-                allFunctions.append(decl['prototype'].split(' ')[0] + " " + decl['displayname'] + const)
+                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " " + decl['displayname'] + const)
             elif decl['access_type'] == 'PRIVATE':
-                allPrivFunctions.append(virtual + decl['prototype'].split(' ')[0] + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const)
+                allPrivFunctions.append(virtual + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const)
             elif decl['access_type'] == 'PUBLIC':
-                allPublicFunctions.append(virtual + decl['prototype'].split(' ')[0] + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const)
+                allPublicFunctions.append(virtual + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const)
             elif decl['access_type'] == 'PROTECTED':
-                allProtectedFunctions.append(virtual + decl['prototype'].split(' ')[0] + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const )
+                allProtectedFunctions.append(virtual + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const )
         elif decl['kind'] == "FUNCTION_DECL":
-            if len(decl['prototype'].split(' ')[0].split('**')) == 1 and len(decl['prototype'].split(' ')[0].split('*')) == 1:
-                allFunctions.append(decl['prototype'].split(' ')[0] + " " + decl['displayname'] + const)
+            if len(decl['prototype'].split('(')[0].split('**')) == 1 and len(decl['prototype'].split('(')[0].split('*')) == 1:
+                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " " + decl['displayname'] + const)
             elif len(decl['prototype'].split('**')) > 1:
-                allFunctions.append(decl['prototype'].split('**')[0] + "**" + " " + decl['displayname'] + const)
+                allFunctions.append(decl['prototype'].split('**')[0] + unsigned + "** " + decl['displayname'] + const)
             else:
-                allFunctions.append(decl['prototype'].split(' ')[0] + "*" + " " + decl['displayname' + const])
+                allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " * " + decl['displayname' + const])
         if decl['kind'] == "CLASS_DECL":
             allClasses.append("class " + decl['prototype'])
     
     #Write the YAML file
     file_yaml = {'classes': {'restriction': f'{restriction}', 'scope': 'global', 'names': list(set(allClasses))}, 'functions': {'restriction': f'{restriction}', 'scope': 'global', 'names': list(set(allFunctions))}, 'public_functions': {'restriction': f'{restriction}', 'scope': 'global', 'names': list(set(allPublicFunctions))}, 'private_functions': {'restriction': f'{restriction}', 'scope': 'global', 'names': list(set(allPrivFunctions))}, 'protected_functions': {'restriction': f'{restriction}', 'scope': 'global', 'names': list(set(allProtectedFunctions))}}
     with open("checkAPI.yaml", 'w') as file:
         yaml.dump(file_yaml, file)
     
     restrict(source, "checkAPI.YAML", output, hide)
 
     if not hide:
         checkAPI(compare, restriction, source, output, True)
 
-    #Just to increase speed of code, this is explained in prepare data in codeparser
-    commentController.includeRevert(source)
-
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `y4d-0.1.0/PKG-INFO` & `y4d-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y4d
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: BahouA
 Author-email: antonbahou@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

