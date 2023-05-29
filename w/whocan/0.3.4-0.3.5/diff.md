# Comparing `tmp/whocan-0.3.4.tar.gz` & `tmp/whocan-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whocan-0.3.4.tar", max compression
+gzip compressed data, was "whocan-0.3.5.tar", max compression
```

## Comparing `whocan-0.3.4.tar` & `whocan-0.3.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1398 2022-05-01 01:06:56.968293 whocan-0.3.4/README.md
--rw-r--r--   0        0        0      492 2022-10-22 23:16:01.156262 whocan-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      597 2022-10-16 03:59:59.430643 whocan-0.3.4/whocan/__init__.py
--rw-r--r--   0        0        0      266 2022-10-16 00:38:35.174545 whocan-0.3.4/whocan/_environment.py
--rw-r--r--   0        0        0      242 2022-04-30 22:32:30.732180 whocan-0.3.4/whocan/_errors.py
--rw-r--r--   0        0        0    12861 2022-10-22 23:15:16.737835 whocan-0.3.4/whocan/_policies.py
--rw-r--r--   0        0        0     3365 2022-10-16 03:32:42.110736 whocan-0.3.4/whocan/_policy_sets.py
--rw-r--r--   0        0        0     2121 2022-10-22 23:17:00.374171 whocan-0.3.4/setup.py
--rw-r--r--   0        0        0     2034 2022-10-22 23:17:00.374475 whocan-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1398 2022-05-01 01:06:56.968293 whocan-0.3.5/README.md
+-rw-r--r--   0        0        0      492 2023-05-29 17:57:56.862933 whocan-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      597 2022-10-16 03:59:59.430643 whocan-0.3.5/whocan/__init__.py
+-rw-r--r--   0        0        0      266 2022-10-16 00:38:35.174545 whocan-0.3.5/whocan/_environment.py
+-rw-r--r--   0        0        0      242 2022-04-30 22:32:30.732180 whocan-0.3.5/whocan/_errors.py
+-rw-r--r--   0        0        0    12518 2023-05-29 17:56:07.342966 whocan-0.3.5/whocan/_policies.py
+-rw-r--r--   0        0        0     3365 2022-10-16 03:32:42.110736 whocan-0.3.5/whocan/_policy_sets.py
+-rw-r--r--   0        0        0     2121 2023-05-29 17:58:34.622454 whocan-0.3.5/setup.py
+-rw-r--r--   0        0        0     2034 2023-05-29 17:58:34.622768 whocan-0.3.5/PKG-INFO
```

### Comparing `whocan-0.3.4/README.md` & `whocan-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `whocan-0.3.4/whocan/__init__.py` & `whocan-0.3.5/whocan/__init__.py`

 * *Files identical despite different names*

### Comparing `whocan-0.3.4/whocan/_policies.py` & `whocan-0.3.5/whocan/_policies.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 from whocan import _errors
 from whocan import _environment
 
 DEFAULT_ENV = _environment.PolicyEnvironment({})
 
 
-def _force_to_list(
-        value: typing.Union[typing.List[str], str]
-) -> typing.List[str]:
+def _force_to_list(value: typing.Union[typing.List[str], str]) -> typing.List[str]:
     """Force the value to a list."""
     if isinstance(value, str):
         return [value]
     return value
 
 
 def _policy_check(raise_issue: bool, message: str):
@@ -26,114 +24,107 @@
         raise _errors.PolicyYamlInvalidError(message)
 
 
 def _validate_yaml(raw_yaml: typing.Any):
     """Validate the yaml or raise an error if it is invalid."""
     if not isinstance(raw_yaml, dict):
         raise _errors.PolicyYamlInvalidError(
-            'Top level of policy must be a dictionary.'
+            "Top level of policy must be a dictionary."
         )
+    _policy_check("statements" not in raw_yaml, 'Missing required field "statements".')
     _policy_check(
-        'statements' not in raw_yaml,
-        'Missing required field "statements".'
-    )
-    _policy_check(
-        not isinstance(raw_yaml['statements'], list),
-        '"statements" must be a list.'
+        not isinstance(raw_yaml["statements"], list), '"statements" must be a list.'
     )
 
-    for i, statement in enumerate(raw_yaml['statements']):
-        required = ['effect', 'actions']
+    for i, statement in enumerate(raw_yaml["statements"]):
+        required = ["effect", "actions"]
         for r in required:
             _policy_check(
-                r not in statement,
-                f'Missing required field "statements[{i}].{r}".'
+                r not in statement, f'Missing required field "statements[{i}].{r}".'
             )
         _policy_check(
-            not ('principals' in statement or 'resources' in statement),
+            not ("principals" in statement or "resources" in statement),
             (
                 f'Missing required field in "statements[{i}]". Must include '
                 'either "resources" or "principals".'
-            )
+            ),
         )
         _policy_check(
-            statement['effect'] not in {'allow', 'deny'},
+            statement["effect"] not in {"allow", "deny"},
             f'Missing required field "statements[{i}].effect"'
-            ' must be "allow" or "deny".'
+            ' must be "allow" or "deny".',
         )
         _policy_check(
             (
-                'resources' in statement
-                and not isinstance(statement['resources'], (str, list))
+                "resources" in statement
+                and not isinstance(statement["resources"], (str, list))
             ),
-            f'"statements[{i}].resources" must be a string or list.'
+            f'"statements[{i}].resources" must be a string or list.',
         )
         _policy_check(
             (
-                'principals' in statement
-                and not isinstance(statement['principals'], (str, list))
+                "principals" in statement
+                and not isinstance(statement["principals"], (str, list))
             ),
-            f'"statements[{i}].principals" must be a string or list.'
+            f'"statements[{i}].principals" must be a string or list.',
         )
         _policy_check(
-            not isinstance(statement['actions'], (str, list)),
+            not isinstance(statement["actions"], (str, list)),
             f'Missing required field "statements[{i}].actions"'
-            ' must be a string or list.'
+            " must be a string or list.",
         )
-        key = 'resources'
+        key = "resources"
         if key in statement and isinstance(statement[key], list):
             _policy_check(
-                any(not isinstance(r, str) for r in statement['resources']),
-                f'All members of "statements[{i}].resources" must be strings.'
+                any(not isinstance(r, str) for r in statement["resources"]),
+                f'All members of "statements[{i}].resources" must be strings.',
             )
-        key = 'principals'
+        key = "principals"
         if key in statement and isinstance(statement[key], list):
             _policy_check(
-                any(not isinstance(r, str) for r in statement['principals']),
-                f'All members of "statements[{i}].principals" must be strings.'
+                any(not isinstance(r, str) for r in statement["principals"]),
+                f'All members of "statements[{i}].principals" must be strings.',
             )
-        if isinstance(statement['actions'], list):
+        if isinstance(statement["actions"], list):
             _policy_check(
-                any(not isinstance(a, str) for a in statement['actions']),
-                f'All members of "statements[{i}].actions" must be strings.'
+                any(not isinstance(a, str) for a in statement["actions"]),
+                f'All members of "statements[{i}].actions" must be strings.',
             )
 
 
 def _form_regex(
-        base: str,
-        arguments: typing.Dict[str, str],
-        strict: bool,
+    base: str,
+    arguments: typing.Dict[str, str],
+    strict: bool,
 ) -> str:
     """Form a regex from the given base value and arguments."""
     previous = 0
     processed = []
-    for m in re.finditer(r'((?:\${\s*(\w+)\s*})|\*+)', base):
+    for m in re.finditer(r"((?:\${\s*(\w+)\s*})|\*+)", base):
         if m.start() != previous:
-            processed.append(re.escape(base[previous:m.start()]))
-        if m.group(1) == '*':
-            processed.append('[^/]*')
-        if m.group(1).startswith('**'):
-            processed.append('.*')
+            processed.append(re.escape(base[previous : m.start()]))
+        if m.group(1) == "*":
+            processed.append("[^/]*")
+        if m.group(1).startswith("**"):
+            processed.append(".*")
         if m.group(2):
             parameter = m.group(2)
             if parameter not in arguments and strict:
-                raise _errors.PolicyEvaluationError(
-                    f'"{parameter}" unknown variable.'
-                )
-            processed.append(str(arguments.get(parameter, '')))
+                raise _errors.PolicyEvaluationError(f'"{parameter}" unknown variable.')
+            processed.append(str(arguments.get(parameter, "")))
         previous = m.end()
     processed.append(re.escape(base[previous:]))
-    pattern = ''.join(processed)
-    return f'^{pattern}$'
+    pattern = "".join(processed)
+    return f"^{pattern}$"
 
 
 def _conditions_meet(
-        env: _environment.PolicyEnvironment,
-        conditions: typing.Optional[typing.List['Condition']],
-        arguments: typing.Dict[str, str],
+    env: _environment.PolicyEnvironment,
+    conditions: typing.Optional[typing.List["Condition"]],
+    arguments: typing.Dict[str, str],
 ) -> bool:
     """Determine if the conditions have been meet."""
     return all(
         env.condition_functions[c.operator](arguments.get(c.key), c.value)
         for c in conditions or []
     )
 
@@ -153,63 +144,63 @@
 
     raw_line: str
     arguments: typing.Dict[str, str]
     strict: bool = True
 
     def is_match(self, value: str) -> bool:
         """Determine if the given value is a match for the line."""
-        if self.line == '*':
+        if self.line == "*":
             return True
-        values = value.split(':')
-        pieces = self.line.split(':')
+        values = value.split(":")
+        pieces = self.line.split(":")
         if len(values) != len(pieces):
             return False
         for piece, incoming in zip(pieces, values):
             pattern = _form_regex(piece, self.arguments, self.strict)
             if not re.fullmatch(pattern, incoming):
                 return False
         return True
 
     @property
     def line(self) -> str:
         """Get the line with arguments rendered in."""
         previous = 0
         processed = []
-        for m in re.finditer(r'((?:\${\s*(\w+)\s*}))', self.raw_line):
+        for m in re.finditer(r"((?:\${\s*(\w+)\s*}))", self.raw_line):
             if m.start() != previous:
-                processed.append(self.raw_line[previous:m.start()])
+                processed.append(self.raw_line[previous : m.start()])
             if m.group(2):
                 parameter = m.group(2)
                 if parameter not in self.arguments and self.strict:
                     raise _errors.PolicyEvaluationError(
                         f'"{parameter}" unknown variable.'
                     )
-                processed.append(str(self.arguments.get(parameter, '')))
+                processed.append(str(self.arguments.get(parameter, "")))
             previous = m.end()
         processed.append(self.raw_line[previous:])
-        return ''.join(processed)
+        return "".join(processed)
 
 
 @dataclasses.dataclass
 class Statement:
     """A singular set of actions and resources."""
 
     effect: str
     actions: typing.List[str]
     resources: typing.Optional[typing.List[str]] = None
     principals: typing.Optional[typing.List[str]] = None
     conditions: typing.Optional[typing.List[Condition]] = None
 
     def evaluate(
-            self,
-            action: str,
-            resource: typing.Optional[str] = None,
-            principal: typing.Optional[str] = None,
-            arguments: typing.Dict[str, str] = None,
-            env: _environment.PolicyEnvironment = DEFAULT_ENV,
+        self,
+        action: str,
+        resource: typing.Optional[str] = None,
+        principal: typing.Optional[str] = None,
+        arguments: typing.Dict[str, str] = None,
+        env: _environment.PolicyEnvironment = DEFAULT_ENV,
     ) -> typing.Optional[str]:
         """
         Evaluate the statement to determine if it allows, denys, or has no
         effect on the specified resource and action.
 
         :param action:
             The action being taken on the specified resource.
@@ -233,79 +224,67 @@
         for incoming, lines in checks:
             if incoming is None and lines is None:
                 results.append(True)
                 continue
             if incoming is None or lines is None:
                 results.append(False)
                 continue
-            results.append(
-                any(Line(l, arguments).is_match(incoming) for l in lines)
-            )
+            results.append(any(Line(l, arguments).is_match(incoming) for l in lines))
         conditions_meet = _conditions_meet(env, self.conditions, arguments)
-        return (
-            self.effect
-            if all(results) and conditions_meet else
-            None
-        )
+        return self.effect if all(results) and conditions_meet else None
 
     def to_jsonable(self) -> dict:
         """Serialize the statement to a JSONable object."""
-        resources = (
-            [r for r in self.resources]
-            if self.resources is not None else
-            None
-        )
+        resources = [r for r in self.resources] if self.resources is not None else None
         principals = (
-            [r for r in self.principals]
-            if self.principals is not None else
-            None
+            [r for r in self.principals] if self.principals is not None else None
         )
         conditions = (
             [dataclasses.asdict(c) for c in self.conditions]
-            if self.conditions is not None else
-            None
+            if self.conditions is not None
+            else None
         )
         base = {
-            'effect': self.effect,
-            'actions': self.actions,
-            'resources': resources,
-            'principals': principals,
-            'conditions': conditions,
+            "effect": self.effect,
+            "actions": self.actions,
+            "resources": resources,
+            "principals": principals,
+            "conditions": conditions,
         }
         return {k: v for k, v in base.items() if v is not None}
 
     @classmethod
     def from_jsonable(cls, jsonable: dict) -> dict:
         """Deserialize the policy set from a JSONable object."""
         conditions = [
-            Condition(c['operator'], c['key'], c['value'])
-            for c in jsonable.get('conditions') or []
+            Condition(c["operator"], c["key"], c["value"])
+            for c in _force_to_list(jsonable.get("conditions")) or []
         ]
         return cls(
-            jsonable['effect'],
-            jsonable['actions'],
-            jsonable.get('resources'),
-            jsonable.get('principals'),
-            conditions if jsonable.get('conditions') is not None else None,
+            jsonable["effect"],
+            _force_to_list(jsonable["actions"]),
+            _force_to_list(jsonable.get("resources")),
+            _force_to_list(jsonable.get("principals")),
+            conditions if jsonable.get("conditions") is not None else None,
         )
 
 
 @dataclasses.dataclass
 class Policy:
     """An policy defining resource access."""
 
     statements: typing.List[Statement]
 
     def is_allowed(
-            self,
-            action: str,
-            resource: str = None,
-            principal: str = None,
-            arguments: typing.Dict[str, str] = None,
-            env: _environment.PolicyEnvironment = DEFAULT_ENV,
+        self,
+        action: str,
+        resource: str = None,
+        principal: str = None,
+        arguments: typing.Dict[str, str] = None,
+        env: _environment.PolicyEnvironment = DEFAULT_ENV,
     ) -> bool:
         """
         Determine if the given policy allows the specified action on the
         specified resource.
 
         :param action:
             The action being taken on the specified resource.
@@ -314,23 +293,23 @@
         :param arguments:
             Arguments to pass into the policy before determining if
             access is allowed.
         :return:
             Whether the action is allowed on the resource.
         """
         result = self.evaluate(action, resource, principal, arguments, env)
-        return 'allow' == result
+        return "allow" == result
 
     def evaluate(
-            self,
-            action: str,
-            resource: str = None,
-            principal: str = None,
-            arguments: typing.Dict[str, str] = None,
-            env: _environment.PolicyEnvironment = DEFAULT_ENV,
+        self,
+        action: str,
+        resource: str = None,
+        principal: str = None,
+        arguments: typing.Dict[str, str] = None,
+        env: _environment.PolicyEnvironment = DEFAULT_ENV,
     ) -> typing.Optional[str]:
         """
         Evaluate the policy to determine if it allows, denys, or makes no
         comment on the specified resource and action.
 
         :param action:
             The action being taken on the specified resource.
@@ -342,48 +321,42 @@
         :return:
             Either "allow", "deny" or None.
         """
         evaluations = [
             statement.evaluate(action, resource, principal, arguments, env)
             for statement in self.statements
         ]
-        if any(v == 'deny' for v in evaluations):
-            return 'deny'
-        if any(v == 'allow' for v in evaluations):
-            return 'allow'
+        if any(v == "deny" for v in evaluations):
+            return "deny"
+        if any(v == "allow" for v in evaluations):
+            return "allow"
         return None
 
     @classmethod
-    def load(cls, policy_input: typing.Union[pathlib.Path, str]) -> 'Policy':
+    def load(cls, policy_input: typing.Union[pathlib.Path, str]) -> "Policy":
         """Load the specified policy from yaml."""
         try:
             body = (
                 policy_input.read_text()
-                if hasattr(policy_input, 'read_text') else
-                policy_input
+                if hasattr(policy_input, "read_text")
+                else policy_input
             )
-            raw_yaml =  yaml.safe_load(body)
+            raw_yaml = yaml.safe_load(body)
         except yaml.YAMLError:
-            raise _errors.PolicyYamlInvalidError('Invalid policy yaml.')
+            raise _errors.PolicyYamlInvalidError("Invalid policy yaml.")
         _validate_yaml(raw_yaml)
         statements = [
-            Statement.from_jsonable(statement)
-            for statement in raw_yaml['statements']
+            Statement.from_jsonable(statement) for statement in raw_yaml["statements"]
         ]
         return Policy(statements)
 
     def to_jsonable(self) -> dict:
         """Serialize the policy to a JSONable object."""
         return {
-            'type': 'policy',
-            'statements': [
-                s.to_jsonable()
-                for s in self.statements
-            ]
+            "type": "policy",
+            "statements": [s.to_jsonable() for s in self.statements],
         }
 
     @classmethod
     def from_jsonable(cls, jsonable: dict) -> dict:
         """Deserialize the policy set from a JSONable object."""
-        return cls(
-            [Statement.from_jsonable(s) for s in jsonable['statements']]
-        )
+        return cls([Statement.from_jsonable(s) for s in jsonable["statements"]])
```

### Comparing `whocan-0.3.4/whocan/_policy_sets.py` & `whocan-0.3.5/whocan/_policy_sets.py`

 * *Files identical despite different names*

### Comparing `whocan-0.3.4/setup.py` & `whocan-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'whocan',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'Library for defining and determining access.',
     'long_description': "# Whocan\n\nLibrary for defining and determining access.\n\n## Usage\n\n### YAML usage\n\n```yaml\nstatements:\n- effect: allow\n  actions:\n  - workspace:Create*\n  - workspace:Delete*\n  - workspace:Get*\n  - workspace:List*\n  - workspace:Update*\n  resources:\n  - workspace:individual-${username}\n```\n\n```python\nimport pathlib\nimport whocan\n\npolicy = whocan.Policy.load(pathlib.Path('path-to-file.yaml'))\npolicy.is_allowed(\n    resource='workspaces:individual-my-username',\n    action='workspace:DeletePage',\n    arguments={'username': 'my-username'},\n)\n# True\npolicy.is_allowed(\n    resource='workspaces:individual-a-different-user',\n    action='workspace:DeletePage',\n    arguments={'username': 'my-username'},\n)\n# False\n```\n\n### Pure python usage\n\n```python\nimport whocan\n\nstatement = whocan.Statement(\n    resources=['workspaces:individual-${username}'],\n    actions=[\n        'workspace:Create*',\n        'workspace:Delete*',\n        'workspace:Get*',\n        'workspace:List*',\n        'workspace:Update*',\n    ],\n    effect='allow',\n)\n\npolicy = whocan.Policy(statements=[statement])\npolicy.is_allowed(\n    resource='workspaces:individual-my-username',\n    action='workspace:DeletePage',\n    arguments={'username': 'my-username'},\n)\n# True\npolicy.is_allowed(\n    resource='workspaces:individual-a-different-user',\n    action='workspace:DeletePage',\n    arguments={'username': 'my-username'},\n)\n# False\n```",
     'author': 'Kevin Schiroo',
     'author_email': 'kjschiroo@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/kjschiroo/whocan',
```

### Comparing `whocan-0.3.4/PKG-INFO` & `whocan-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whocan
-Version: 0.3.4
+Version: 0.3.5
 Summary: Library for defining and determining access.
 Home-page: https://gitlab.com/kjschiroo/whocan
 License: MIT
 Author: Kevin Schiroo
 Author-email: kjschiroo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

