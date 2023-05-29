# Comparing `tmp/fake_session_maker-0.0.1.tar.gz` & `tmp/fake_session_maker-0.0.2.tar.gz`

## Comparing `fake_session_maker-0.0.1.tar` & `fake_session_maker-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.flake8
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/build_requirements.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/requirements_py310.txt
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/requirements_py311.txt
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/requirements_py37.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/requirements_py38.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/requirements_py39.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.idea/fake_session_maker.iml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.idea/sqldialects.xml
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0    15074 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0    46150 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.idea/dataSources/e04919d0-934c-4abf-96f0-ebb1da792c46.xml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/src/fake_session_maker/__init__.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/src/fake_session_maker/fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/src/fake_session_maker/py.typed
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/tests/test_fsm.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/AUTHORS.rst
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/README.md
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 fake_session_maker-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.flake8
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/build_requirements.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/requirements_py310.txt
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/requirements_py311.txt
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/requirements_py37.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/requirements_py38.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/requirements_py39.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.gitlab/merge_request_templates/MERGE_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.idea/fake_session_maker.iml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/src/fake_session_maker/__init__.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/src/fake_session_maker/fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/src/fake_session_maker/py.typed
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/tests/test_fixture_maker.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/tests/test_fsm.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/AUTHORS.rst
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/README.md
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 fake_session_maker-0.0.2/PKG-INFO
```

### Comparing `fake_session_maker-0.0.1/.gitlab-ci.yml` & `fake_session_maker-0.0.2/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -82,20 +82,20 @@
 
 requirements_py311:
   image: python:3.11
   stage: requirements
   script:
     - *requirements_script
 
-requirements_py312:
-  image: python:3.12-rc
-  stage: requirements
-  allow_failure: true
-  script:
-    - *requirements_script
+#requirements_py312:
+#  image: python:3.12-rc
+#  stage: requirements
+#  allow_failure: true
+#  script:
+#    - *requirements_script
 
 py37:
   image: python:3.7
   stage: test
   needs: ["requirements_py37"]
   before_script:
     - *install_test
@@ -134,16 +134,16 @@
   stage: test
   needs: ["requirements_py311"]
   before_script:
     - *install_test
   script:
     - pytest
 
-py312:
-  image: python:3.12-rc
-  stage: test
-  needs: ["requirements_py312"]
-  allow_failure: true
-  before_script:
-    - *install_test
-  script:
-    - pytest
+#py312:
+#  image: python:3.12-rc
+#  stage: test
+#  needs: ["requirements_py312"]
+#  allow_failure: true
+#  before_script:
+#    - *install_test
+#  script:
+#    - pytest
```

### Comparing `fake_session_maker-0.0.1/src/fake_session_maker/fsm.py` & `fake_session_maker-0.0.2/src/fake_session_maker/fsm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import contextlib
 import typing
 
 import pytest
 import sqlalchemy.orm
 
 
-class ExplicitCommit(Exception):
-    """
-    Raised when a commit is explicitly called on a session.
-    """
-
-
 @contextlib.contextmanager
 def fsm(
     db_url: typing.Union[str, sqlalchemy.engine.url.URL],
     namespace: typing.Any,
     symbol_name: str,
     *,
     create_engine_kwargs: typing.Optional[typing.Mapping] = None,
@@ -31,25 +25,18 @@
 
     engine = sqlalchemy.create_engine(
         url=db_url,
         **create_engine_kwargs,
     )
     session_maker = sqlalchemy.orm.sessionmaker(
         bind=engine,
-        autoflush=False,
     )
 
-    def forbidden_commit() -> typing.NoReturn:
-        raise ExplicitCommit(
-            "To use fake session, rely on autocommit. "
-            "See: method sqlalchemy.engine.Connection.begin() → RootTransaction"
-        )
-
     with session_maker() as session_singleton:
-        session_singleton.commit = forbidden_commit  # type: ignore
+        session_singleton.commit = session_singleton.flush  # type: ignore
 
         class SessionContextManager:
             def __enter__(self) -> sqlalchemy.orm.Session:
                 return session_singleton
 
             def __exit__(
                 self, exc_type: typing.Any, exc_val: typing.Any, exc_tb: typing.Any
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fake_session_maker-0.0.1/tests/test_fsm.py` & `fake_session_maker-0.0.2/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,69 @@
+import pathlib
 import sqlite3
 
 import pytest
-import sqlalchemy
 import sqlalchemy.orm
 
 from fake_session_maker import fsm
 
 
-class Namespace:
-    engine = sqlalchemy.create_engine(
-        "sqlite:///tests/test.db",
-        echo=True,
-    )
-    session_maker = sqlalchemy.orm.sessionmaker(bind=engine)
-
-
 @pytest.fixture(autouse=True, scope="session")
 def db_migrate():
-    with sqlite3.connect("./tests/test.sqlite") as con:
+    db = pathlib.Path("./tests/test.sqlite")
+    with sqlite3.connect(db) as con:
         cur = con.cursor()
         cur.execute("CREATE TABLE IF NOT EXISTS users (id INTEGER PRIMARY KEY, name TEXT)")
         con.commit()
     yield
-    with sqlite3.connect("./tests/test.sqlite") as con:
+    with sqlite3.connect(db) as con:
         cur.execute("DROP TABLE users")
         con.commit()
+    db.unlink()
 
 
 @pytest.fixture
-def fake_session_maker():
+def namespace():
+    class Namespace:
+        engine = sqlalchemy.create_engine(
+            "sqlite:///tests/test.db",
+            echo=True,
+        )
+        session_maker = sqlalchemy.orm.sessionmaker(bind=engine)
+
+    return Namespace
+
+
+class Base(sqlalchemy.orm.DeclarativeBase):
+    pass
+
+
+@pytest.fixture(scope="session")
+def user_model():
+    class User(Base):
+        __tablename__ = "users"
+        id = sqlalchemy.Column(sqlalchemy.Integer, primary_key=True)
+        name = sqlalchemy.Column(sqlalchemy.String)
+
+    return User
+
+
+@pytest.fixture
+def create_user(namespace, user_model):
+    def create_user_(name: str):
+        with namespace.session_maker.begin() as session:
+            session.add(user_model(name=name))
+        return "success"
+
+    return create_user_
+
+
+@pytest.fixture
+def fake_session_maker(namespace) -> sqlalchemy.orm.sessionmaker:
     with fsm(
         db_url="sqlite:///tests/test.sqlite",
-        namespace=Namespace,
+        namespace=namespace,
         symbol_name="session_maker",
-    ) as fake_session_maker:
+    ) as fake_session_maker_:
         # the fake_session_maker won't auto-commit after transaction
         # and rollback after transaction
-        yield fake_session_maker
-
-
-def create_user(name: str):
-    with Namespace.session_maker.begin() as session:
-        session.execute(sqlalchemy.text("INSERT INTO users (name) VALUES (:name)"), {"name": name})
-    return "success"
-
-
-@pytest.mark.parametrize("name", ["Joe", "Jane"])
-def test_isolation(fake_session_maker, name):
-    result = create_user(name)
-    assert result == "success"
-    with fake_session_maker() as session:
-        assert session.execute(sqlalchemy.text("SELECT * FROM users")).fetchall() == [(1, name)]
+        yield fake_session_maker_
```

### Comparing `fake_session_maker-0.0.1/.gitignore` & `fake_session_maker-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fake_session_maker-0.0.1/LICENSE` & `fake_session_maker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_session_maker-0.0.1/pyproject.toml` & `fake_session_maker-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fake_session_maker"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Dorian Turba", email = "contact.5rgbj@8shield.net" },
 ]
 description = "Create a SQLAlchemy session_maker that won't commit to db for testing purposes."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -70,15 +70,15 @@
 disallow_untyped_defs = true
 
 [tool.tox]
 legacy_tox_ini = """
     [tox]
     min_version = 4.0
     env_list =
-        py{37,38,39,310,311,312}
+        py{37,38,39,310,311}
         black
         flake8
         mypy
     isolated_build = true
 
     [testenv]
     deps = pytest
```

