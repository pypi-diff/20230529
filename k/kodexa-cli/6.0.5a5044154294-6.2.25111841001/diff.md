# Comparing `tmp/kodexa_cli-6.0.5a5044154294.tar.gz` & `tmp/kodexa_cli-6.2.25111841001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa_cli-6.0.5a5044154294.tar", max compression
+gzip compressed data, was "kodexa_cli-6.2.25111841001.tar", max compression
```

## Comparing `kodexa_cli-6.0.5a5044154294.tar` & `kodexa_cli-6.2.25111841001.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/LICENSE
--rw-r--r--   0        0        0     2707 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/README.md
--rw-r--r--   0        0        0       64 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/__init__.py
--rw-r--r--   0        0        0    25616 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/cli.py
--rw-r--r--   0        0        0    10054 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/documentation.py
--rw-r--r--   0        0        0      134 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/action.jinja2
--rw-r--r--   0        0        0     1356 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/assistant.jinja2
--rw-r--r--   0        0        0     1021 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/content-taxon.jinja2
--rw-r--r--   0        0        0      328 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/data-store.jinja2
--rw-r--r--   0        0        0      707 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/document-store.jinja2
--rw-r--r--   0        0        0       30 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/extension-pack.jinja2
--rw-r--r--   0        0        0      818 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/header.jinja2
--rw-r--r--   0        0        0      343 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/index.jinja2
--rw-r--r--   0        0        0       30 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/model-runtime.jinja2
--rw-r--r--   0        0        0     2999 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/model.jinja2
--rw-r--r--   0        0        0     1137 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/options.jinja2
--rw-r--r--   0        0        0        0 2023-05-22 09:31:20.275894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/overview.jinja2
--rw-r--r--   0        0        0      922 2023-05-22 09:31:20.279894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/processing-taxon.jinja2
--rw-r--r--   0        0        0       30 2023-05-22 09:31:20.279894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/project-template.jinja2
--rw-r--r--   0        0        0       30 2023-05-22 09:31:20.279894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/store.jinja2
--rw-r--r--   0        0        0      492 2023-05-22 09:31:20.279894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/taxon.jinja2
--rw-r--r--   0        0        0      273 2023-05-22 09:31:20.279894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/taxonomy-labels.jinja2
--rw-r--r--   0        0        0      534 2023-05-22 09:31:20.279894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/taxonomy-structure.jinja2
--rw-r--r--   0        0        0      269 2023-05-22 09:31:20.279894 kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/taxonomy.jinja2
--rw-r--r--   0        0        0      783 2023-05-22 09:31:35.036119 kodexa_cli-6.0.5a5044154294/pyproject.toml
--rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 kodexa_cli-6.0.5a5044154294/setup.py
--rw-r--r--   0        0        0     3392 1970-01-01 00:00:00.000000 kodexa_cli-6.0.5a5044154294/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-29 12:23:36.528296 kodexa_cli-6.2.25111841001/LICENSE
+-rw-r--r--   0        0        0     2707 2023-05-29 12:23:36.528296 kodexa_cli-6.2.25111841001/README.md
+-rw-r--r--   0        0        0       64 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/__init__.py
+-rw-r--r--   0        0        0    23500 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/cli.py
+-rw-r--r--   0        0        0     7641 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/documentation.py
+-rw-r--r--   0        0        0      134 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/action.jinja2
+-rw-r--r--   0        0        0     1356 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/assistant.jinja2
+-rw-r--r--   0        0        0     1021 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/content-taxon.jinja2
+-rw-r--r--   0        0        0      328 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/data-store.jinja2
+-rw-r--r--   0        0        0      707 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/document-store.jinja2
+-rw-r--r--   0        0        0       30 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/extension-pack.jinja2
+-rw-r--r--   0        0        0      818 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/header.jinja2
+-rw-r--r--   0        0        0      343 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/index.jinja2
+-rw-r--r--   0        0        0       30 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/model-runtime.jinja2
+-rw-r--r--   0        0        0     2999 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/model.jinja2
+-rw-r--r--   0        0        0     1137 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/options.jinja2
+-rw-r--r--   0        0        0        0 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/overview.jinja2
+-rw-r--r--   0        0        0      922 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/processing-taxon.jinja2
+-rw-r--r--   0        0        0       30 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/project-template.jinja2
+-rw-r--r--   0        0        0       30 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/store.jinja2
+-rw-r--r--   0        0        0      492 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/taxon.jinja2
+-rw-r--r--   0        0        0      273 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/taxonomy-labels.jinja2
+-rw-r--r--   0        0        0      534 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/taxonomy-structure.jinja2
+-rw-r--r--   0        0        0      269 2023-05-29 12:23:36.532296 kodexa_cli-6.2.25111841001/kodexa_cli/templates/taxonomy.jinja2
+-rw-r--r--   0        0        0      780 2023-05-29 12:23:57.812385 kodexa_cli-6.2.25111841001/pyproject.toml
+-rw-r--r--   0        0        0     3665 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25111841001/setup.py
+-rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25111841001/PKG-INFO
```

### Comparing `kodexa_cli-6.0.5a5044154294/LICENSE` & `kodexa_cli-6.2.25111841001/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.0.5a5044154294/README.md` & `kodexa_cli-6.2.25111841001/README.md`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.0.5a5044154294/kodexa_cli/cli.py` & `kodexa_cli-6.2.25111841001/kodexa_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,25 +95,24 @@
     info.verbose = verbose
 
 
 @cli.command
 @click.argument('project_id', required=True)
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
 @pass_info
-def project(_: Info, project_id: str, token: str, url: str, profile: Optional[str] = None):
+def project(_: Info, project_id: str, token: str, url: str):
     """
     Get details for a specific project.
 
     project_id is the ID of the project to get details for.
 
     """
 
-    client = KodexaClient(url=url, access_token=token) if not profile else KodexaClient(profile=profile)
+    client = KodexaClient(url=url, access_token=token)
     project_instance = client.get_project(project_id)
     print(f"Name: [bold]{project_instance.name}[/bold]")
     print(f"Description: [bold]{project_instance.description}[/bold]\n")
 
     print("[bold]Document Stores[/bold]")
     project_instance.document_stores.print_table()
     print("[bold]Data Stores[/bold]")
@@ -125,25 +124,24 @@
 
 
 @cli.command()
 @click.argument('ref', required=True)
 @click.argument('paths', required=True, nargs=-1)
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
 @pass_info
-def upload(_: Info, ref: str, paths: list[str], token: str, url: str, profile: Optional[str] = None):
+def upload(_: Info, ref: str, paths: list[str], token: str, url: str):
     """
     Upload a file to the Kodexa platform.
 
     ref is the reference to the document store to upload to.
     path is the path to the file to upload, it can be many files.
     """
-    client = KodexaClient(url=url, access_token=token) if not profile else KodexaClient(profile=profile)
 
+    client = KodexaClient(url=url, access_token=token)
     document_store = client.get_object_by_ref('store', ref)
 
     from kodexa.platform.client import DocumentStoreEndpoint
 
     print(f"Uploading {len(paths)} files to {ref}\n")
     if isinstance(document_store, DocumentStoreEndpoint):
         from rich.progress import track
@@ -169,23 +167,22 @@
 @click.option('--file', help='The path to the file containing the object to apply')
 @click.option('--update/--no-update', help='The path to the file containing the object to apply',
               default=False)
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
 @click.option('--format', default=None, help='The format to input if from stdin (json, yaml)')
 @click.option('--overlay', default=None, help='A JSON or YAML file that will overlay the metadata')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
 @pass_info
 def deploy(_: Info, org: Optional[str], file: str, url: str, token: str, format=None, update: bool = False,
-           version=None, overlay: Optional[str] = None, profile: Optional[str] = None, slug=None):
+           version=None, overlay: Optional[str] = None, slug=None):
     """
     Deploy a component to a Kodexa platform instance from a file or stdin
     """
 
-    client = KodexaClient(url=url, access_token=token) if not profile else KodexaClient(profile=profile)
+    client = KodexaClient(access_token=token, url=url)
 
     obj = None
     if file is None:
         print("Reading from stdin")
         if format == 'yaml' or format == 'yml':
             obj = yaml.safe_load(sys.stdin.read())
         elif format == 'json':
@@ -249,49 +246,47 @@
     print("Deployed :tada:")
 
 
 @cli.command()
 @click.argument('execution_id', required=True)
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
 @pass_info
-def logs(_: Info, execution_id: str, url: str, token: str, profile: Optional[str] = None):
+def logs(_: Info, execution_id: str, url: str, token: str):
     """
     Get the logs for a specific execution
 
     execution_id is the id of the execution to get the logs for
     """
-    client = KodexaClient(url=url, access_token=token) if not profile else KodexaClient(profile=profile)
+    client = KodexaClient(url=url, access_token=token)
     client.executions.get(execution_id).logs()
 
 
 @cli.command()
 @click.argument('object_type', required=True)
 @click.argument('ref', required=False)
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
 @click.option('--query', default="*", help='Limit the results using a query')
 @click.option('--path', default=None, help='JQ path to content you want')
 @click.option('--format', default=None, help='The format to output (json, yaml)')
 @click.option('--page', default=1, help='Page number')
 @click.option('--pageSize', default=10, help='Page size')
 @click.option('--sort', default=None, help='Sort by (ie. startDate:desc)')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
 @pass_info
 def get(_: Info, object_type: str, ref: Optional[str], url: str, token: str, query: str, path: str = None, format=None,
-        page: int = 1, pagesize: int = 10, sort: str = None, profile: Optional[str] = None):
+        page: int = 1, pagesize: int = 10, sort: str = None):
     """
     List the instances of the component or entity type
 
     object_type is the type of object to list (component, document, execution, etc.)
     ref is the reference to the object
     """
 
-    client = KodexaClient(url=url, access_token=token) if not profile else KodexaClient(profile=profile)
+    client = KodexaClient(url=url, access_token=token)
 
     from kodexa.platform.client import resolve_object_type
     object_name, object_metadata = resolve_object_type(object_type)
 
     if 'global' in object_metadata and object_metadata['global']:
         objects_endpoint = client.get_object_type(object_type)
         if ref and not ref.isspace():
@@ -357,40 +352,39 @@
                 row.append("")
         table.add_row(*row, style='yellow')
 
     from rich.console import Console
     console = Console()
     console.print(table)
     console.print(
-        f"Page [bold]{page_of_object_endpoints.number}[/bold] of [bold]{page_of_object_endpoints.total_pages}[/bold] "
+        f"Page [bold]{page_of_object_endpoints.number + 1}[/bold] of [bold]{page_of_object_endpoints.total_pages}[/bold] "
         f"(total of {page_of_object_endpoints.total_elements} objects)")
 
 
 @cli.command()
 @click.argument('ref', required=True)
 @click.argument('query', default="*")
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
 @click.option('--download/--no-download', default=False, help='Download the KDDB for the latest in the family')
 @click.option('--download-native/--no-download-native', default=False, help='Download the native file for the family')
 @click.option('--page', default=1, help='Page number')
 @click.option('--pageSize', default=10, help='Page size')
 @click.option('--sort', default=None, help='Sort by ie. name:asc')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
 @pass_info
 def query(_: Info, query: str, ref: str, url: str, token: str, download: bool, download_native: bool, page: int,
-          pagesize: int, sort: None, profile: Optional[str] = None):
+          pagesize: int, sort: None):
     """
     Query the documents in a given document store
 
     ref is the reference to the document store
     query is the query to run
 
     """
-    client = KodexaClient(url=url, access_token=token) if not profile else KodexaClient(profile=profile)
+    client = KodexaClient(url=url, access_token=token)
     from kodexa.platform.client import DocumentStoreEndpoint
 
     document_store: DocumentStoreEndpoint = client.get_object_by_ref('store', ref)
     if isinstance(document_store, DocumentStoreEndpoint):
         results = document_store.query(query, page, pagesize, sort)
 
     else:
@@ -398,46 +392,43 @@
 
 
 @cli.command()
 @click.argument('project_id', required=True)
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
 @click.option('--output', help='The path to export to')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
 @pass_info
-def export_project(_: Info, project_id: str, url: str, token: str, output: str, profile: Optional[str] = None):
+def export_project(_: Info, project_id: str, url: str, token: str, output: str):
     """
     Export a project, and associated resources to a local zip file
 
     project_id is the id of the project to export
     """
-
-    client = KodexaClient(url=url, access_token=token) if not profile else KodexaClient(profile=profile)
+    client = KodexaClient(url, token)
     project_endpoint = client.projects.get(project_id)
     client.export_project(project_endpoint, output)
 
 
 @cli.command()
 @click.argument('org_slug', required=True)
 @click.argument('path', required=True)
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
 @pass_info
-def import_project(_: Info, org_slug: str, url: str, token: str, path: str, profile: Optional[str] = None):
+def import_project(_: Info, org_slug: str, url: str, token: str, path: str):
     """
     Import a project, and associated resources from a local zip file
 
     org_slug is the slug of the organization to import into
     path is the path to the zip file
 
     """
     print("Importing project from {}".format(path))
 
-    client = KodexaClient(url=url, access_token=token) if not profile else KodexaClient(profile=profile)
+    client = KodexaClient(url, token)
     organization = client.organizations.find_by_slug(org_slug)
 
     print("Organization: {}".format(organization.name))
     client.import_project(organization, path)
 
     print("Project imported")
 
@@ -445,27 +436,25 @@
 @cli.command()
 @click.argument('project_id', required=True)
 @click.argument('assistant_id', required=True)
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
 @click.option('--file', help='The path to the file containing the event to send')
 @click.option('--format', default=None, help='The format to use if from stdin (json, yaml)')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
 @pass_info
-def send_event(_: Info, project_id: str, assistant_id: str, url: str, file: str, event_format: str, token: str,
-               profile: Optional[str] = None):
+def send_event(_: Info, project_id: str, assistant_id: str, url: str, file: str, event_format: str, token: str):
     """
     Send an event to an assistant
 
     project_id is the id of the project to send the event to
     assistant_id is the id of the assistant to send the event to
 
     """
 
-    client = KodexaClient(url=url, access_token=token) if not profile else KodexaClient(profile=profile)
+    client = KodexaClient(url, token)
 
     obj = None
     if file is None:
         print("Reading from stdin")
         if event_format == 'yaml':
             obj = yaml.parse(sys.stdin.read())
         elif event_format == 'json':
@@ -488,51 +477,48 @@
     assistant_endpoint.send_event(obj['eventType'], obj['options'])
     print("Event sent :tada:")
 
 
 @cli.command()
 @pass_info
 @click.option('--python/--no-python', default=False, help='Print out the header for a Python file')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
-def platform(_: Info, python: bool, profile: Optional[str] = None):
+def platform(_: Info, python: bool):
     """
     Get the details for the Kodexa instance we are logged into
     """
-    platform_url = KodexaPlatform.get_url(profile)
+    platform_url = KodexaPlatform.get_url()
 
     if platform_url is not None:
-        print(f"Kodexa URL: {KodexaPlatform.get_url(profile)}")
-        print(f"Access Token: {KodexaPlatform.get_access_token(profile)}")
+        print(f"Kodexa URL: {KodexaPlatform.get_url()}")
+        print(f"Access Token: {KodexaPlatform.get_access_token()}")
         kodexa_version = KodexaPlatform.get_server_info()
         print(f"Version: {kodexa_version['version']}")
         print(f"Release: {kodexa_version['release']}")
         if python:
             print("\nPython example:\n\n")
             print(f"from kodexa import *")
-            print(f"client = KodexaClient('{KodexaPlatform.get_url(profile)}', "
-                  f"'{KodexaPlatform.get_access_token(profile)}')")
+            print(f"client = KodexaClient('{KodexaPlatform.get_url()}', '{KodexaPlatform.get_access_token()}')")
     else:
         print("Kodexa is not logged in")
 
 
 @cli.command()
 @click.argument('object_type')
 @click.argument('ref')
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
-@click.option('--profile', default=None, help='The profile to used to access url and token')
 @pass_info
-def delete(_: Info, object_type: str, ref: str, url: str, token: str, profile: Optional[str] = None):
+def delete(_: Info, object_type: str, ref: str, url: str, token: str):
     """
     Delete the given resource (based on ref)
 
     object_type is the type of object to delete (e.g. 'project', 'assistant', 'store')
     ref is the ref of the object to delete
     """
-    client = KodexaClient(url=url, access_token=token) if not profile else KodexaClient(profile=profile)
+    client = KodexaClient(url, token)
     client.get_object_by_ref(object_type, ref).delete()
 
 
 @cli.command()
 @pass_info
 def login(_: Info):
     """Logs into the specified platform environment using the email address and password provided,
@@ -545,21 +531,18 @@
     try:
         kodexa_url = input("Enter the Kodexa URL (https://platform.kodexa.com): ")
         if kodexa_url == "":
             print("Using default as https://platform.kodexa.com")
             kodexa_url = "https://platform.kodexa.com"
         username = input("Enter your email: ")
         password = getpass("Enter your password: ")
-        profile = input("Login profile name [None]: ")
-        if not profile:
-            profile = None
     except Exception as error:
         print('ERROR', error)
     else:
-        KodexaPlatform.login(kodexa_url, username, password, profile)
+        KodexaPlatform.login(kodexa_url, username, password)
 
 
 @cli.command()
 @click.argument('files', nargs=-1)
 @pass_info
 def mkdocs(_: Info, files: list[str]):
     """
```

### Comparing `kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/assistant.jinja2` & `kodexa_cli-6.2.25111841001/kodexa_cli/templates/assistant.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/content-taxon.jinja2` & `kodexa_cli-6.2.25111841001/kodexa_cli/templates/content-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/document-store.jinja2` & `kodexa_cli-6.2.25111841001/kodexa_cli/templates/document-store.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/header.jinja2` & `kodexa_cli-6.2.25111841001/kodexa_cli/templates/header.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/model.jinja2` & `kodexa_cli-6.2.25111841001/kodexa_cli/templates/model.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/options.jinja2` & `kodexa_cli-6.2.25111841001/kodexa_cli/templates/options.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/processing-taxon.jinja2` & `kodexa_cli-6.2.25111841001/kodexa_cli/templates/processing-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.0.5a5044154294/kodexa_cli/templates/taxonomy-structure.jinja2` & `kodexa_cli-6.2.25111841001/kodexa_cli/templates/taxonomy-structure.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.0.5a5044154294/pyproject.toml` & `kodexa_cli-6.2.25111841001/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "kodexa-cli"
-version = "6.0.5a5044154294"
+version = "6.2.25111841001"
 description = "Command Line Tools for Kodexa"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>", "John Patrick Sese <jp@kodexa.com>"]
 readme = "README.md"
 packages = [{include = "kodexa_cli"}]
 
 [tool.poetry.scripts]
 kodexa = 'kodexa_cli:cli'
 
 [tool.poetry.dependencies]
 python = "^3.9"
-kodexa = "^6.0.116"
+kodexa = "^6.2.0"
 click = "8.1.3"
 PyYAML = "^6.0"
-rich = "13.0.1"
+rich = "13.3.5"
 flake8 = "^6.0.0"
-mypy = "^0.991"
-pandas = "^1.5.3"
+mypy = "^1.3.0"
+pandas = "^2.0.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 mkdocs-click = "^0.8.0"
 mkdocs-material = "^9.0.3"
```

### Comparing `kodexa_cli-6.0.5a5044154294/setup.py` & `kodexa_cli-6.2.25111841001/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 package_data = \
 {'': ['*'], 'kodexa_cli': ['templates/*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'click==8.1.3',
  'flake8>=6.0.0,<7.0.0',
- 'kodexa>=6.0.116,<7.0.0',
- 'mypy>=0.991,<0.992',
- 'pandas>=1.5.3,<2.0.0',
- 'rich==13.0.1']
+ 'kodexa>=6.2.0,<7.0.0',
+ 'mypy>=1.3.0,<2.0.0',
+ 'pandas>=2.0.2,<3.0.0',
+ 'rich==13.3.5']
 
 entry_points = \
 {'console_scripts': ['kodexa = kodexa_cli:cli']}
 
 setup_kwargs = {
     'name': 'kodexa-cli',
-    'version': '6.0.5a5044154294',
+    'version': '6.2.25111841001',
     'description': 'Command Line Tools for Kodexa',
     'long_description': '# Kodexa Command Line Tools\n\n[![Kodexa CLI Python Package](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml/badge.svg)](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Command Line Tools\n\nThis repository contains the command line tools for Kodexa. The tools are the primary way to interact with Kodexa. It\nallows you to configure components and manage aspects of your Kodexa Platform installation.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\n**BUILD VERSION FLOW**\n![build-version-flow.png](docs%2Fbuild-version-flow.png)\nBuild version will differ based on the branches that are published to pypi.\n\n**GITHUB PROCESS**\n![github-process.png](docs%2Fgithub-process.png)\nChanges that contain bugs, features, and fixes should first be pushed to the test branch.\nOnce these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa_cli-6.0.5a5044154294/PKG-INFO` & `kodexa_cli-6.2.25111841001/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kodexa-cli
-Version: 6.0.5a5044154294
+Version: 6.2.25111841001
 Summary: Command Line Tools for Kodexa
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (==8.1.3)
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
-Requires-Dist: kodexa (>=6.0.116,<7.0.0)
-Requires-Dist: mypy (>=0.991,<0.992)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: rich (==13.0.1)
+Requires-Dist: kodexa (>=6.2.0,<7.0.0)
+Requires-Dist: mypy (>=1.3.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: rich (==13.3.5)
 Description-Content-Type: text/markdown
 
 # Kodexa Command Line Tools
 
 [![Kodexa CLI Python Package](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml/badge.svg)](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml)
 
 ![img.png](https://docs.kodexa.com/img.png)
```

