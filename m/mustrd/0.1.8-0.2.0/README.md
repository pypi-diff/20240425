# Comparing `tmp/mustrd-0.1.8.tar.gz` & `tmp/mustrd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mustrd-0.1.8.tar", max compression
+gzip compressed data, was "mustrd-0.2.0.tar", max compression
```

## Comparing `mustrd-0.1.8.tar` & `mustrd-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1099 2024-02-26 13:34:46.564344 mustrd-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2024-03-28 15:41:42.375415 mustrd-0.1.8/mustrd/__init__.py
--rw-r--r--   0        0        0     1630 2024-03-28 15:41:42.377427 mustrd-0.1.8/mustrd/logger_setup.py
--rw-r--r--   0        0        0      386 2024-04-03 15:10:48.653712 mustrd-0.1.8/mustrd/model/catalog-v001.xml
--rw-r--r--   0        0        0     9709 2024-03-28 15:41:42.379427 mustrd-0.1.8/mustrd/model/mustrdShapes.ttl
--rw-r--r--   0        0        0     2034 2024-04-15 09:12:19.357864 mustrd-0.1.8/mustrd/model/mustrdTestOntology.ttl
--rw-r--r--   0        0        0      842 2024-04-15 14:03:22.329614 mustrd-0.1.8/mustrd/model/mustrdTestShapes.ttl
--rw-r--r--   0        0        0    17303 2024-04-03 16:12:05.425128 mustrd-0.1.8/mustrd/model/ontology.ttl
--rw-r--r--   0        0        0     1558 2024-03-28 15:41:42.381426 mustrd-0.1.8/mustrd/model/test-resources/resources.ttl
--rw-r--r--   0        0        0     6199 2024-04-03 16:11:22.263000 mustrd-0.1.8/mustrd/model/triplestoreOntology.ttl
--rw-r--r--   0        0        0     1876 2024-04-16 14:08:01.101076 mustrd-0.1.8/mustrd/model/triplestoreshapes.ttl
--rw-r--r--   0        0        0    35099 2024-04-17 14:58:51.079865 mustrd-0.1.8/mustrd/mustrd.py
--rw-r--r--   0        0        0    11822 2024-03-28 15:41:42.398480 mustrd-0.1.8/mustrd/mustrdAnzo.py
--rw-r--r--   0        0        0     5599 2024-03-28 15:41:42.399480 mustrd-0.1.8/mustrd/mustrdGraphDb.py
--rw-r--r--   0        0        0     2129 2024-03-28 15:41:42.400481 mustrd-0.1.8/mustrd/mustrdRdfLib.py
--rw-r--r--   0        0        0    15035 2024-04-18 08:48:16.471480 mustrd-0.1.8/mustrd/mustrdTestPlugin.py
--rw-r--r--   0        0        0     3765 2024-04-17 13:27:21.126688 mustrd-0.1.8/mustrd/namespace.py
--rw-r--r--   0        0        0    11995 2024-04-03 09:39:22.688671 mustrd-0.1.8/mustrd/README.adoc
--rw-r--r--   0        0        0     4380 2024-04-17 12:56:01.295904 mustrd-0.1.8/mustrd/run.py
--rw-r--r--   0        0        0    32546 2024-04-17 13:39:30.911945 mustrd-0.1.8/mustrd/spec_component.py
--rw-r--r--   0        0        0     7555 2024-04-17 13:40:53.882724 mustrd-0.1.8/mustrd/steprunner.py
--rw-r--r--   0        0        0      526 2024-03-28 15:41:42.440938 mustrd-0.1.8/mustrd/templates/md_ResultList_leaf_template.jinja
--rw-r--r--   0        0        0      211 2024-03-28 15:41:42.445469 mustrd-0.1.8/mustrd/templates/md_ResultList_template.jinja
--rw-r--r--   0        0        0      157 2024-03-28 15:41:42.450987 mustrd-0.1.8/mustrd/templates/md_stats_template.jinja
--rw-r--r--   0        0        0      129 2024-04-12 16:21:29.119938 mustrd-0.1.8/mustrd/test/test_mustrd.py
--rw-r--r--   0        0        0     4986 2024-03-28 15:41:42.458004 mustrd-0.1.8/mustrd/TestResult.py
--rw-r--r--   0        0        0     1424 2024-03-28 15:41:42.462005 mustrd-0.1.8/mustrd/utils.py
--rw-r--r--   0        0        0     1493 2024-04-18 09:37:19.554639 mustrd-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2724 2024-02-26 13:34:46.565338 mustrd-0.1.8/README.adoc
--rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 mustrd-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-02-26 13:34:46.564344 mustrd-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-28 15:41:42.375415 mustrd-0.2.0/mustrd/__init__.py
+-rw-r--r--   0        0        0     1630 2024-03-28 15:41:42.377427 mustrd-0.2.0/mustrd/logger_setup.py
+-rw-r--r--   0        0        0      386 2024-04-03 15:10:48.653712 mustrd-0.2.0/mustrd/model/catalog-v001.xml
+-rw-r--r--   0        0        0     9709 2024-03-28 15:41:42.379427 mustrd-0.2.0/mustrd/model/mustrdShapes.ttl
+-rw-r--r--   0        0        0     2034 2024-04-15 09:12:19.357864 mustrd-0.2.0/mustrd/model/mustrdTestOntology.ttl
+-rw-r--r--   0        0        0      842 2024-04-15 14:03:22.329614 mustrd-0.2.0/mustrd/model/mustrdTestShapes.ttl
+-rw-r--r--   0        0        0    17303 2024-04-03 16:12:05.425128 mustrd-0.2.0/mustrd/model/ontology.ttl
+-rw-r--r--   0        0        0     1558 2024-03-28 15:41:42.381426 mustrd-0.2.0/mustrd/model/test-resources/resources.ttl
+-rw-r--r--   0        0        0     6199 2024-04-03 16:11:22.263000 mustrd-0.2.0/mustrd/model/triplestoreOntology.ttl
+-rw-r--r--   0        0        0     1876 2024-04-16 14:08:01.101076 mustrd-0.2.0/mustrd/model/triplestoreshapes.ttl
+-rw-r--r--   0        0        0    35081 2024-04-18 13:48:56.648531 mustrd-0.2.0/mustrd/mustrd.py
+-rw-r--r--   0        0        0    10632 2024-04-24 13:42:49.104879 mustrd-0.2.0/mustrd/mustrdAnzo.py
+-rw-r--r--   0        0        0     5599 2024-03-28 15:41:42.399480 mustrd-0.2.0/mustrd/mustrdGraphDb.py
+-rw-r--r--   0        0        0     6357 2024-04-25 13:16:41.281038 mustrd-0.2.0/mustrd/mustrdQueryProcessor.py
+-rw-r--r--   0        0        0     2129 2024-03-28 15:41:42.400481 mustrd-0.2.0/mustrd/mustrdRdfLib.py
+-rw-r--r--   0        0        0    15035 2024-04-18 08:48:16.471480 mustrd-0.2.0/mustrd/mustrdTestPlugin.py
+-rw-r--r--   0        0        0     3765 2024-04-17 13:27:21.126688 mustrd-0.2.0/mustrd/namespace.py
+-rw-r--r--   0        0        0    12620 2024-04-18 16:48:29.451303 mustrd-0.2.0/mustrd/README.adoc
+-rw-r--r--   0        0        0     4380 2024-04-17 12:56:01.295904 mustrd-0.2.0/mustrd/run.py
+-rw-r--r--   0        0        0    33304 2024-04-18 17:10:15.150833 mustrd-0.2.0/mustrd/spec_component.py
+-rw-r--r--   0        0        0     7555 2024-04-17 13:40:53.882724 mustrd-0.2.0/mustrd/steprunner.py
+-rw-r--r--   0        0        0      526 2024-03-28 15:41:42.440938 mustrd-0.2.0/mustrd/templates/md_ResultList_leaf_template.jinja
+-rw-r--r--   0        0        0      211 2024-03-28 15:41:42.445469 mustrd-0.2.0/mustrd/templates/md_ResultList_template.jinja
+-rw-r--r--   0        0        0      157 2024-03-28 15:41:42.450987 mustrd-0.2.0/mustrd/templates/md_stats_template.jinja
+-rw-r--r--   0        0        0      129 2024-04-12 16:21:29.119938 mustrd-0.2.0/mustrd/test/test_mustrd.py
+-rw-r--r--   0        0        0     4986 2024-03-28 15:41:42.458004 mustrd-0.2.0/mustrd/TestResult.py
+-rw-r--r--   0        0        0     1424 2024-03-28 15:41:42.462005 mustrd-0.2.0/mustrd/utils.py
+-rw-r--r--   0        0        0     1493 2024-04-25 13:20:42.207156 mustrd-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2724 2024-02-26 13:34:46.565338 mustrd-0.2.0/README.adoc
+-rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 mustrd-0.2.0/PKG-INFO
```

### Comparing `mustrd-0.1.8/LICENSE` & `mustrd-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/logger_setup.py` & `mustrd-0.2.0/mustrd/logger_setup.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/model/mustrdShapes.ttl` & `mustrd-0.2.0/mustrd/model/mustrdShapes.ttl`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/model/mustrdTestOntology.ttl` & `mustrd-0.2.0/mustrd/model/mustrdTestOntology.ttl`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/model/mustrdTestShapes.ttl` & `mustrd-0.2.0/mustrd/model/mustrdTestShapes.ttl`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/model/ontology.ttl` & `mustrd-0.2.0/mustrd/model/ontology.ttl`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/model/test-resources/resources.ttl` & `mustrd-0.2.0/mustrd/model/test-resources/resources.ttl`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/model/triplestoreOntology.ttl` & `mustrd-0.2.0/mustrd/model/triplestoreOntology.ttl`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/model/triplestoreshapes.ttl` & `mustrd-0.2.0/mustrd/model/triplestoreshapes.ttl`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/mustrd.py` & `mustrd-0.2.0/mustrd/mustrd.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,16 +300,15 @@
     results = []
     # https://github.com/Semantic-partners/mustrd/issues/115
     for specification in specs:
         results.append(run_spec(specification))
     return results
 
 def get_spec_file(spec_uri: URIRef, spec_graph: Graph):
-    test =  str(spec_graph.value(subject = spec_uri, predicate = MUST.specFileName, default = "default.mustrd.ttl"))
-    return test
+    return str(spec_graph.value(subject = spec_uri, predicate = MUST.specFileName, default = "default.mustrd.ttl"))
 
 def get_spec(spec_uri: URIRef, spec_graph: Graph, run_config: dict, mustrd_triple_store: dict = None) -> Specification:
     try:
         if mustrd_triple_store is None:
             mustrd_triple_store = {"type": TRIPLESTORE.RdfLib}
         components = []
         for predicate in MUST.given, MUST.when, MUST.then:
```

### Comparing `mustrd-0.1.8/mustrd/mustrdAnzo.py` & `mustrd-0.2.0/mustrd/mustrdAnzo.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,100 +24,100 @@
 
 import requests
 from pyanzo import AnzoClient
 from rdflib import Graph, ConjunctiveGraph, Literal, URIRef
 from requests import ConnectTimeout, Response, HTTPError, RequestException, ConnectionError
 from bs4 import BeautifulSoup
 import logging
-from .namespace import MUST
 
 
 # https://github.com/Semantic-partners/mustrd/issues/73
 def manage_anzo_response(response: Response) -> str:
     content_string = response.content.decode("utf-8")
     if response.status_code == 200:
         return content_string
     elif response.status_code == 403:
         html = BeautifulSoup(content_string, 'html.parser')
         title_tag = html.title.string
         raise HTTPError(f"Anzo authentication error, status code: {response.status_code}, content: {title_tag}")
     else:
         raise RequestException(f"Anzo error, status code: {response.status_code}, content: {content_string}")
 
-
 def query_with_bindings(bindings: dict, when: str) -> str:
     values = ""
     for key, value in bindings.items():
         values += f"VALUES ?{key} {{{value.n3()}}} "
     split_query = when.lower().split("where {", 1)
     return f"{split_query[0].strip()} WHERE {{ {values} {split_query[1].strip()}"
 
 def execute_select (triple_store: dict,  when: str, bindings: dict = None) -> str:
+    if bindings:
+        when = query_with_bindings(bindings, when)
+    # Just remove ${fromSources} if we are executing a query step; the sources are defined using http parameters 
+    when = when.replace("${fromSources}", "")
+    return execute_sparql(triple_store, False, when, triple_store['input_graph'])
+
+PARAMS = {
+    # Update parameters for INSERT / DELETE
+    True: {
+        "default-graph-param": "using-graph-uri",
+        "named-graph-param":"using-named-graph-uri",
+        "Content-Type": "application/sparql-update"
+    },
+    # Query parameters for SELECT / CONSTRUCT  
+    False: {
+        "default-graph-param": "default-graph-uri",
+        "named-graph-param":"named-graph-uri",
+        "Content-Type": "application/sparql-query"
+    }
+}
+def execute_sparql(triple_store: dict, is_update: bool, sparql, graph: str, format: str = "application/sparql-results+json"):
+    params = {
+        "format" : format,
+        "datasourceURI" : triple_store['gqe_uri'],
+        "skipCache": "true",
+        # Default and named datasets have different query param for query and update
+        PARAMS[is_update]["default-graph-param"] : graph,
+        PARAMS[is_update]["named-graph-param"] : graph
+    }
+    headers={"Content-Type": PARAMS[is_update]["Content-Type"]}
     try:
-        if bindings:
-            when = query_with_bindings(bindings, when)
-        when = when.replace("${fromSources}", f"FROM <{triple_store['input_graph']}>\nFROM <{triple_store['output_graph']}>").replace(
-        "${targetGraph}", f"<{triple_store['output_graph']}>")
-        data = {'datasourceURI': triple_store['gqe_uri'], 'query': when,
-                 'skipCache': 'true'}
-        url = f"https://{triple_store['url']}:{triple_store['port']}/sparql?format=application/sparql-results+json"
-        return manage_anzo_response(requests.post(url=url,
-                                                  auth=(triple_store['username'], triple_store['password']),
-                                                  data=data,
-                                                  verify=False))
-    except (ConnectionError, TimeoutError, HTTPError, ConnectTimeout):
+        response = manage_anzo_response(requests.post(url=f"https://{triple_store['url']}:{triple_store['port']}/sparql",
+                                                    params=params,
+                                                    auth=(triple_store['username'], triple_store['password']),
+                                                    headers=headers,
+                                                    data=sparql,
+                                                    verify=False))
+        logging.debug(f'response {response}')
+        return response
+    except (ConnectionError, TimeoutError, HTTPError, ConnectTimeout) as e:
+        logging.error(f'response {e}')
         raise
 
 def execute_update(triple_store: dict, when: str, bindings: dict = None) -> Graph:
     logging.debug(f"updating in anzo! {triple_store=} {when=}")
-    input_graph = triple_store['input_graph']
-    output_graph = triple_store['output_graph']
 
-    substituted_query = when.replace("${usingSources}", f"USING <{triple_store['input_graph']}> \nUSING <{triple_store['output_graph']}>").replace(
-        "${targetGraph}", f"<{output_graph}>")
-   
-    data = {'datasourceURI': triple_store['gqe_uri'], 'update': substituted_query,
-                'default-graph-uri': input_graph, 'skipCache': 'true'}
-    url = f"https://{triple_store['url']}:{triple_store['port']}/sparql?format=ttl"
-    response = manage_anzo_response(requests.post(url=url,
-            auth=(triple_store['username'],
-                triple_store['password']),
-            data=data,
-            verify=False))
-    logging.debug(f'response {response}')
-    check_data = {'datasourceURI': triple_store['gqe_uri'], 'query': "construct {?s ?p ?o} { ?s ?p ?o }",
-                'default-graph-uri': output_graph, 'skipCache': 'true'}
-    everything_response = manage_anzo_response(requests.post(url=url,
-            auth=(triple_store['username'],
-                triple_store['password']),
-            data=check_data,
-            verify=False))
-    # todo deal with error responses
-    new_graph = Graph().parse(data=everything_response)
+    # FIXME If query doesn't contain ${targetGraph}, then graph should be defined explicitly in the query
+    substituted_query = when.replace("${usingSources}", "").replace(
+        "${targetGraph}", f"<{triple_store['output_graph']}>")
+    
+    execute_sparql(triple_store, True, substituted_query, triple_store['input_graph'], "ttl")
+    
+    new_graph = execute_construct(triple_store, "construct {?s ?p ?o} { ?s ?p ?o }")
+    
     logging.debug(f"new_graph={new_graph.serialize(format='ttl')}")
+    
     return new_graph
 
 
 def execute_construct(triple_store: dict, when: str, bindings: dict = None) -> Graph:
-    try:
-        if bindings:
-            when = query_with_bindings(bindings, when)
-        data = {'datasourceURI': triple_store['gqe_uri'], 'query': when,
-                'default-graph-uri': triple_store['input_graph'], 'skipCache': 'true'}
-        url = f"https://{triple_store['url']}:{triple_store['port']}/sparql?format=ttl"
-        response = requests.post(url=url,
-            auth=(triple_store['username'],
-                triple_store['password']),
-            data=data,
-            verify=False)
-        logging.debug(f'response {response}')
-        return Graph().parse(data=manage_anzo_response(response))
-    except (ConnectionError, TimeoutError, HTTPError, ConnectTimeout) as e:
-        logging.error(f'response {e}')
-        raise
+    if bindings:
+        when = query_with_bindings(bindings, when)
+    response = execute_sparql(triple_store, False, when, triple_store['input_graph'], "ttl")
+    return Graph().parse(data=response)
 
 
 # Get Given or then from the content of a graphmart
 def get_spec_component_from_graphmart(triple_store: dict, graphmart: URIRef, layer: URIRef = None) -> ConjunctiveGraph:
     try:
         anzo_client = AnzoClient(triple_store['url'], triple_store['port'], 
                                  username=triple_store['username'],
@@ -203,34 +203,18 @@
                              username=triple_store['username'],
                              password=triple_store['password'])
     return anzo_client.query_journal(query_string=query).as_table_results().as_record_dictionaries()
 
 
 def upload_given(triple_store: dict, given: Graph):
     logging.debug(f"upload_given {triple_store} {given}")
-
-    try:
-        input_graph = triple_store['input_graph']
-        output_graph = triple_store['output_graph']
-        clear_graph(triple_store, input_graph)
-        clear_graph(triple_store, output_graph)
-        serialized_given = given.serialize(format="nt")
-        insert_query = f"INSERT DATA {{graph <{triple_store['input_graph']}>{{{serialized_given}}}}}"
-        data = {'datasourceURI': triple_store['gqe_uri'], 'update': insert_query}
-        response = requests.post(url=f"https://{triple_store['url']}:{triple_store['port']}/sparql",
-                                    auth=(triple_store['username'], triple_store['password']), data=data, verify=False)
-        manage_anzo_response(response)
-    except (ConnectionError, TimeoutError, HTTPError, ConnectTimeout):
-        raise
+    clear_graph(triple_store, triple_store['input_graph'])
+    clear_graph(triple_store, triple_store['output_graph'])
+    serialized_given = given.serialize(format="nt")
+    
+    insert_query = f"INSERT DATA {{graph <{triple_store['input_graph']}>{{{serialized_given}}}}}"
+    execute_sparql(triple_store, True, insert_query, None, None)
 
 
 def clear_graph(triple_store: dict, graph_uri: str):
-    try:
-        clear_query = f"CLEAR GRAPH <{graph_uri}>"
-        data = {'datasourceURI': triple_store['gqe_uri'], 'update': clear_query}
-        url = f"https://{triple_store['url']}:{triple_store['port']}/sparql"
-        response = requests.post(url=url,
-                                 auth=(triple_store['username'], triple_store['password']), data=data, verify=False)
-        manage_anzo_response(response)
-    except (ConnectionError, TimeoutError, HTTPError, ConnectTimeout):
-        raise
+    execute_sparql(triple_store, True, f"CLEAR GRAPH <{graph_uri}>", None, None)
```

### Comparing `mustrd-0.1.8/mustrd/mustrdGraphDb.py` & `mustrd-0.2.0/mustrd/mustrdGraphDb.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/mustrdRdfLib.py` & `mustrd-0.2.0/mustrd/mustrdRdfLib.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/mustrdTestPlugin.py` & `mustrd-0.2.0/mustrd/mustrdTestPlugin.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/namespace.py` & `mustrd-0.2.0/mustrd/namespace.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/README.adoc` & `mustrd-0.2.0/mustrd/README.adoc`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,23 @@
 
 Run `pytest` from the project root.
 
 == Creating your own Test Specifications
 
 If you have got this far then you are probably ready to create your own specifications to test your application SPARQL queries. These will be executed against the default RDFLib triplestore unless you configure one or more alternatives. The instructions for this are included in <<Configuring external triplestores>> below.
 
+=== Paths
+All paths are consired relative. That way mustrd tests can be versionned and shared easily.
+To get absolute path from relative path in a spec file, we prefix it with the first existing result in:
+1) Path where the spec is located
+2) spec_path defined in mustrd test configuration files or cmd line argument
+3) data_path defined in mustrd test configuration files or cmd line argument
+4) Mustrd folder: In case of default resources packaged with mustrd source (will be in venv when mustrd is called as library)
+We intentionally use the same method to build paths in all spec components to avoid confusion.
+
 === Givens
 These are used to specify the dataset against which the SPARQL statement will be run.
 They can be generated from external sources such as an existing graph, or a file or folder containing serialised RDF. It is also possible to specify the dataset as reified RDF directly in the test step. Currently tabular data sources such as csv files or TableDatasets are not supported.
 Multiple given statements can be supplied and data is combined into a single dataset for the test.
 
 * *InheritedDataset* - This is where no data is specified but the existing data in the target graph is retained rather than being replaced with a defined set. This can be used to chain tests together or to perform checks on application data.
 ----
```

### Comparing `mustrd-0.1.8/mustrd/run.py` & `mustrd-0.2.0/mustrd/run.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/spec_component.py` & `mustrd-0.2.0/mustrd/spec_component.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import os
 from dataclasses import dataclass, field
-from itertools import groupby
 from pathlib import Path
 from typing import Tuple, List, Type
 
 import pandas
 import requests
 from rdflib import RDF, Graph, URIRef, Variable, Literal, XSD, util
 from rdflib.exceptions import ParserError
 from rdflib.term import Node
 import logging 
 
 from . import logger_setup
 from .mustrdAnzo import get_queries_for_layer, get_queries_from_templated_step, get_spec_component_from_graphmart, get_query_from_querybuilder, get_query_from_step
 from .namespace import MUST, TRIPLESTORE
 from multimethods import MultiMethod, Default
+from .utils import  get_mustrd_root
 
 log = logger_setup.setup_logger(__name__)
 
 
 @dataclass
 class SpecComponent:
     pass
@@ -80,26 +80,22 @@
     subject: URIRef
     predicate: URIRef
     spec_graph: Graph
     mustrd_triple_store: dict
     spec_component_node: Node
     data_source_type: Node
     run_config: dict
+    root_paths: list
 
-def get_path(path_type: str, run_config: dict) -> Path:
-    try:
-        if str(run_config[path_type]).startswith("/"):
-            return run_config[path_type]
-        else: 
-            return Path(os.path.join(run_config['spec_path'], run_config[path_type]))
-    except(KeyError):
-        if str(run_config['data_path']).startswith("/"):
-            return run_config['data_path']
-        else: 
-            return Path(os.path.join(run_config['spec_path'], run_config['data_path']))
+def get_path(path_type: str, file_name, spec_component_details: SpecComponentDetails) -> Path:
+    if path_type in spec_component_details.run_config:
+        relative_path = os.path.join(spec_component_details.run_config[path_type], file_name)
+    else:
+        relative_path = file_name
+    return get_file_absolute_path(spec_component_details, relative_path)
     
 
 def parse_spec_component(subject: URIRef,
                          predicate: URIRef,
                          spec_graph: Graph,
                          run_config: dict,
                          mustrd_triple_store: dict) -> GivenSpec | WhenSpec | ThenSpec | TableThenSpec:
@@ -113,27 +109,61 @@
             spec_component_details = SpecComponentDetails(
                 subject=subject,
                 predicate=predicate,
                 spec_graph=spec_graph,
                 mustrd_triple_store=mustrd_triple_store,
                 spec_component_node=spec_component_node,
                 data_source_type=data_source_type,
-                run_config=run_config)
+                run_config=run_config, 
+                root_paths=get_components_roots(spec_graph, subject, run_config))
             spec_component = get_spec_component(spec_component_details)
             if type(spec_component) == list:
                 spec_components += spec_component 
             else:
                 spec_components += [spec_component]
 
         # all_data_source_types.extend(data_source_types)
     # return all_data_source_types
     # merge multiple graphs into one, give error if spec config is a TableThen
     # print(f"calling multimethod with {spec_components}")
     return combine_specs(spec_components)
 
+# Here we retrieve all the possible root paths for a specification component.
+# This defines the order of priority between root paths which is:
+# 1) Path where the spec is located
+# 2) spec_path defined in mustrd test configuration files or cmd line argument
+# 3) data_path defined in mustrd test configuration files or cmd line argument
+# 4) Mustrd source folder: In case of default resources packaged with mustrd source (will be in venv when mustrd is called as library)
+# We intentionally don't try for absolute files, but you should feel free to argue that we should do
+def get_components_roots(spec_graph: Graph, subject: URIRef, run_config: dict):
+    where_did_i_load_this_spec_from = spec_graph.value(subject=subject,
+                                                                 predicate=MUST.specSourceFile)
+    roots = [] 
+    if (where_did_i_load_this_spec_from == None):
+        log.error(f"{where_did_i_load_this_spec_from=} was None for test_spec={subject}, we didn't set the test specifications specSourceFile when loading, spec_graph={spec_graph}")
+    else:
+        roots.append(Path(os.path.dirname(where_did_i_load_this_spec_from))) 
+    if run_config and'spec_path' in run_config:
+        roots.append(Path(run_config['spec_path']))
+    if run_config and 'data_path'  in run_config:
+        roots.append(run_config['data_path'])
+    roots.append(get_mustrd_root())
+    
+    return roots
+
+
+# From the list of component potential roots, return the first path that exists
+def get_file_absolute_path(spec_component_details: SpecComponentDetails, relative_file_path: str):
+    if not relative_file_path:
+        raise ValueError("Cannot get absolute path of None")
+    absolute_file_paths = list(map(lambda root_path: Path(os.path.join(root_path, relative_file_path)), spec_component_details.root_paths))
+    for absolute_file_path in absolute_file_paths:
+        if (os.path.exists(absolute_file_path)):
+            return absolute_file_path
+    raise FileNotFoundError(f"Could not find file {relative_file_path=} in any of the {absolute_file_paths=}")
 
 def get_spec_component_type(spec_components: List[SpecComponent]) -> Type[SpecComponent]:
     # Get the type of the first object in the list
     spec_type = type(spec_components[0])
     # Loop through the remaining objects in the list and check their types
     for spec_component in spec_components[1:]:
         if type(spec_component) != spec_type:
@@ -220,15 +250,15 @@
 @get_spec_component.method((MUST.FolderDataset, MUST.given))
 def _get_spec_component_folderdatasource_given(spec_component_details: SpecComponentDetails) -> GivenSpec:
     spec_component = init_spec_component(spec_component_details.predicate)
 
     file_name = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                         predicate=MUST.fileName)
 
-    path = Path(os.path.join(str(get_path('given_path',spec_component_details.run_config)), str(file_name)))
+    path = get_path('given_path', file_name,spec_component_details)
     try:
         spec_component.value = Graph().parse(data=get_spec_component_from_file(path))
     except ParserError as e:
         log.error(f"Problem parsing {path}, error of type {type(e)}")
         raise ValueError(f"Problem parsing {path}, error of type {type(e)}")
     return spec_component
 
@@ -236,59 +266,41 @@
 @get_spec_component.method((MUST.FolderSparqlSource, MUST.when))
 def _get_spec_component_foldersparqlsource_when(spec_component_details: SpecComponentDetails) -> GivenSpec:
     spec_component = init_spec_component(spec_component_details.predicate)
 
     file_name = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                         predicate=MUST.fileName)
 
-    path = Path(os.path.join(str(get_path('when_path',spec_component_details.run_config)), str(file_name)))
+    path = get_path('when_path', file_name,spec_component_details)
     spec_component.value = get_spec_component_from_file(path)
     spec_component.queryType = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                                        predicate=MUST.queryType)
     return spec_component
 
 
 @get_spec_component.method((MUST.FolderDataset, MUST.then))
 def _get_spec_component_folderdatasource_then(spec_component_details: SpecComponentDetails) -> ThenSpec:
     spec_component = init_spec_component(spec_component_details.predicate)
 
     file_name = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                         predicate=MUST.fileName)
-    path = Path(os.path.join(str(get_path('then_path',spec_component_details.run_config)), str(file_name)))
+    path = get_path('then_path', file_name,spec_component_details)
 
     return load_dataset_from_file(path, spec_component)
 
 @get_spec_component.method((MUST.FileDataset, MUST.given))
 @get_spec_component.method((MUST.FileDataset, MUST.then))
 def _get_spec_component_filedatasource(spec_component_details: SpecComponentDetails) -> GivenSpec:
     spec_component = init_spec_component(spec_component_details.predicate)
     return load_spec_component(spec_component_details, spec_component)
 
 def load_spec_component(spec_component_details, spec_component):
-    where_did_i_load_this_spec_from = spec_component_details.spec_graph.value(subject=spec_component_details.subject,
-                                                                 predicate=MUST.specSourceFile)
-    if (where_did_i_load_this_spec_from == None):
-        log.error(f"{where_did_i_load_this_spec_from=} was None for test_spec={spec_component_details.subject}, we didn't set the test specifications specSourceFile when loading, spec_graph={spec_component_details.spec_graph}")
     file_path = Path(str(spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                                  predicate=MUST.file)))
-    
-    test_spec_file_path = os.path.dirname(where_did_i_load_this_spec_from)
-
-    # first we try local relative to the test_spec_file_path, then we try relative to the path under test
-    # we intentionally don't try for absolute files, but you should feel free to argue that we should do.
-    paths = [
-        Path(test_spec_file_path, file_path),
-        Path(os.path.join(spec_component_details.run_config['spec_path'], file_path))
-    ]
-    
-    for path in paths:
-        if (os.path.exists(path)):
-            return load_dataset_from_file(path, spec_component)
-
-    raise FileNotFoundError(f"Could not find file {file_path=} in any of the {paths=}")
+    return load_dataset_from_file(get_file_absolute_path(spec_component_details, file_path), spec_component)
     
 
 def load_dataset_from_file(path: Path, spec_component: ThenSpec) -> ThenSpec:
     if path.is_dir():
         raise ValueError(f"Path {path} is a directory, expected a file")
 
     # https://github.com/Semantic-partners/mustrd/issues/94
@@ -316,20 +328,16 @@
 
 
 @get_spec_component.method((MUST.FileSparqlSource, MUST.when))
 def _get_spec_component_filedatasource_when(spec_component_details: SpecComponentDetails) -> SpecComponent:
     spec_component = init_spec_component(spec_component_details.predicate)
 
     file_path = Path(str(spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
-                                                                 predicate=MUST.file)))
-    if str(file_path).startswith("/"): # absolute path
-        path = file_path
-    else: #relative path
-        path = Path(os.path.join(spec_component_details.run_config['spec_path'], file_path))
-    spec_component.value = get_spec_component_from_file(path)
+                                                                 predicate=MUST.file)))    
+    spec_component.value = get_spec_component_from_file(get_file_absolute_path(spec_component_details, file_path))
 
     spec_component.queryType = spec_component_details.spec_graph.value(subject=spec_component_details.spec_component_node,
                                                                        predicate=MUST.queryType)
 
     return spec_component
```

### Comparing `mustrd-0.1.8/mustrd/steprunner.py` & `mustrd-0.2.0/mustrd/steprunner.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/templates/md_ResultList_leaf_template.jinja` & `mustrd-0.2.0/mustrd/templates/md_ResultList_leaf_template.jinja`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/TestResult.py` & `mustrd-0.2.0/mustrd/TestResult.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/mustrd/utils.py` & `mustrd-0.2.0/mustrd/utils.py`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/pyproject.toml` & `mustrd-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mustrd"
-version = "0.1.8"
+version = "0.2.0"
 description = "A Spec By Example framework for RDF and SPARQL, Inspired by Cucumber."
 authors = ["John Placek <john.placek@semanticpartners.com>",
     "Juliane Piñeiro-Winkler <juliane.pineiro-winkler@semanticpartners.com>",
     "Aymeric Picou <aymeric.picou@semanticpartners.com>",
     "Lance Paine <lance.paine@semanticpartners.com>",
     "Andrew Large <andy.large@semanticpartners.com>", ]
 classifiers = [
```

### Comparing `mustrd-0.1.8/README.adoc` & `mustrd-0.2.0/README.adoc`

 * *Files identical despite different names*

### Comparing `mustrd-0.1.8/PKG-INFO` & `mustrd-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mustrd
-Version: 0.1.8
+Version: 0.2.0
 Summary: A Spec By Example framework for RDF and SPARQL, Inspired by Cucumber.
 Home-page: https://github.com/Semantic-partners/mustrd
 License: MIT
 Author: John Placek
 Author-email: john.placek@semanticpartners.com
 Requires-Python: ==3.11.7
 Classifier: Framework :: Pytest
```

