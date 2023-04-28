# Comparing `tmp/firestoned-0.2.6.tar.gz` & `tmp/firestoned-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestoned-0.2.6.tar", max compression
+gzip compressed data, was "firestoned-0.2.7.tar", max compression
```

## Comparing `firestoned-0.2.6.tar` & `firestoned-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-04-26 14:03:38.877846 firestoned-0.2.6/LICENSE
--rw-r--r--   0        0        0     9344 2023-04-26 14:03:38.877846 firestoned-0.2.6/README.md
--rw-r--r--   0        0        0        0 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/__init__.py
--rw-r--r--   0        0        0     4872 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/__main__.py
--rw-r--r--   0        0        0     2045 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/resource.py
--rw-r--r--   0        0        0        0 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/schema/__init__.py
--rw-r--r--   0        0        0      322 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/schema/asyncapi.jinja2
--rw-r--r--   0        0        0     5906 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/schema/main.py.jinja2
--rw-r--r--   0        0        0      408 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/schema/openapi.jinja2
--rw-r--r--   0        0        0     2263 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/schema/resource.yaml
--rw-r--r--   0        0        0      175 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/spec/__init__.py
--rw-r--r--   0        0        0      866 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/spec/_base.py
--rw-r--r--   0        0        0    13390 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/spec/asyncapi.py
--rw-r--r--   0        0        0     9184 2023-04-26 14:03:38.881846 firestoned-0.2.6/firestone/spec/cli.py
--rw-r--r--   0        0        0    16137 2023-04-26 14:03:38.885846 firestoned-0.2.6/firestone/spec/openapi.py
--rw-r--r--   0        0        0     1664 2023-04-26 14:03:38.885846 firestoned-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    10553 1970-01-01 00:00:00.000000 firestoned-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-28 01:16:21.996657 firestoned-0.2.7/LICENSE
+-rw-r--r--   0        0        0     9344 2023-04-28 01:16:21.996657 firestoned-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/__init__.py
+-rw-r--r--   0        0        0     4872 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/__main__.py
+-rw-r--r--   0        0        0     2045 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/resource.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/schema/__init__.py
+-rw-r--r--   0        0        0      322 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/schema/asyncapi.jinja2
+-rw-r--r--   0        0        0     6151 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/schema/main.py.jinja2
+-rw-r--r--   0        0        0      408 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/schema/openapi.jinja2
+-rw-r--r--   0        0        0     2263 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/schema/resource.yaml
+-rw-r--r--   0        0        0      175 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/spec/__init__.py
+-rw-r--r--   0        0        0      866 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/spec/_base.py
+-rw-r--r--   0        0        0    13390 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/spec/asyncapi.py
+-rw-r--r--   0        0        0     9184 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/spec/cli.py
+-rw-r--r--   0        0        0    16187 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/spec/openapi.py
+-rw-r--r--   0        0        0     1683 2023-04-28 01:16:22.004658 firestoned-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0    10593 1970-01-01 00:00:00.000000 firestoned-0.2.7/PKG-INFO
```

### Comparing `firestoned-0.2.6/LICENSE` & `firestoned-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.6/README.md` & `firestoned-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.6/firestone/__main__.py` & `firestoned-0.2.7/firestone/__main__.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.6/firestone/resource.py` & `firestoned-0.2.7/firestone/resource.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.6/firestone/schema/main.py.jinja2` & `firestoned-0.2.7/firestone/schema/main.py.jinja2`

 * *Files 8% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             format="# %(asctime)s - [%(threadName)s] %(name)s:%(lineno)d %(levelname)s - %(message)s",
         )
 
     logging.getLogger("asyncio").setLevel(logging.CRITICAL)
     if debug:
         _LOGGER.setLevel(logging.DEBUG)
         logging.getLogger().setLevel(logging.DEBUG)
-        logging.getLogger("addressbook").setLevel(logging.DEBUG)
+        logging.getLogger("{{ pkg }}").setLevel(logging.DEBUG)
         logging.getLogger("aiohttp").setLevel(logging.DEBUG)
         logging.getLogger("urllib3").setLevel(logging.DEBUG)
         logging.getLogger("httplib").setLevel(logging.DEBUG)
 
     config = configuration.Configuration(host=api_url)
     config.debug = debug
     if api_key:
@@ -94,76 +94,76 @@
 
     ctx.obj = {
         "api_client": aclient,
     }
     _LOGGER.debug(f"ctx.obj: {ctx.obj}")
 
 
-{% for rsrc in rsrcs -%}
+{% for rsrc in rsrcs|sort(attribute='name') -%}
 @main.group()
 @click.pass_obj
 def {{ rsrc["name"] }}(ctx_obj):
     """High level command for an {{ rsrc["name"] }}."""
     _LOGGER.debug(f"ctx_obj: {ctx_obj}")
     ctx_obj["api_obj"] = {{ rsrc["name"] }}_api.{{ rsrc["name"].capitalize() }}Api(api_client=ctx_obj["api_client"])
 
 
 # pylint: disable=redefined-builtin
 {# high-level resource operations -#}
-{% for op in rsrc["operations"]["resource"] -%}
+{% for op in rsrc["operations"]["resource"]|sort(attribute='name') -%}
 @{{ rsrc["name"] }}.command("{{ op["name"] }}")
-{% for attr in op["attrs"] -%}
+{% for attr in op["attrs"]|sort(attribute='name') -%}
 @click.option("--{{ attr["name"] }}", help="{{ attr["description"] }}", type={{ attr["type"] }}, required={{ attr["required"] }})
 {% endfor -%}
 @click.pass_obj
 @firestone_utils.click_coro
 @api_exc
-async def {{ op["id"] }}(ctx_obj{% for attr in op["attrs"] -%}{{ ", " + attr["name"].replace("-", "_") }}{% endfor -%}):
+async def {{ op["id"] }}(ctx_obj{% for attr in op["attrs"]|sort(attribute='name') -%}{{ ", " + attr["name"].replace("-", "_") }}{% endfor -%}):
     """{{ op["description"] }}"""
     api_obj = ctx_obj["api_obj"]
     params = {
-        {% for attr in op["attrs"] -%}
+        {% for attr in op["attrs"]|sort(attribute='name') -%}
         "{{ attr["name"] }}":  {{ attr["name"].replace("-", "_") }},
         {% endfor -%}
     }
     {% if op["name"] == "create" %}
-    req_body = {{ rsrc["name"] }}_model.{{ rsrc["name"].capitalize() }}()
-    req_body.from_dict(params)
+    req_body = {{ rsrc["name"] }}_model.{{ rsrc["name"].capitalize() }}(**params)
     resp = await api_obj.{{ op["id"] }}(req_body)
     {% else %}
     resp = await api_obj.{{ op["id"] }}(**params)
     {% endif -%}
     _LOGGER.debug(f"resp: {resp}")
 
     if isinstance(resp, list):
-        print(json.dumps([obj.to_dict() for obj in resp]))
+        click.echo(json.dumps([obj.to_dict() for obj in resp]))
+    elif resp:
+        click.echo(json.dumps(resp.to_dict()))
     else:
-        print(json.dumps(resp.to_dict()))
-
+        click.echo("No data returned")
 
 {% endfor -%}
 
 {# high-level resource instance operations -#}
-{% for op in rsrc["operations"]["instance"] -%}
+{% for op in rsrc["operations"]["instance"]|sort(attribute='name') -%}
 @{{ rsrc["name"] }}.command("{{ op["name"] }}")
-{% for attr in op["attrs"] -%}
+{% for attr in op["attrs"]|sort(attribute='name') -%}
 {% if attr.get("argument") -%}
 @click.argument("{{ attr["name"] }}", type={{ attr["type"] }})
 {% else -%}
 @click.option("--{{ attr["name"] }}", help="{{ attr["description"] }}", type={{ attr["type"] }}, required={{ attr["required"] }})
 {% endif -%}
 {% endfor -%}
 @click.pass_obj
 @firestone_utils.click_coro
 @api_exc
-async def {{ op["id"] }}(ctx_obj{% for attr in op["attrs"] -%}{{ ", " + attr["name"].replace("-", "_") }}{% endfor -%}):
+async def {{ op["id"] }}(ctx_obj{% for attr in op["attrs"]|sort(attribute='name') -%}{{ ", " + attr["name"].replace("-", "_") }}{% endfor -%}):
     """{{ op["description"] }}"""
     api_obj = ctx_obj["api_obj"]
     params = {
-        {% for attr in op["attrs"] -%}
+        {% for attr in op["attrs"]|sort(attribute='name') -%}
         "{{ attr["name"] }}":  {{ attr["name"].replace("-", "_") }},
         {% endfor -%}
     }
     {% if op["name"] == "create" %}
     req_body = {{ rsrc["name"] }}_model.{{ rsrc["name"].capitalize() }}()
     req_body.from_dict(params)
     resp = await api_obj.{{ op["id"] }}(req_body)
```

### Comparing `firestoned-0.2.6/firestone/schema/resource.yaml` & `firestoned-0.2.7/firestone/schema/resource.yaml`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.6/firestone/spec/_base.py` & `firestoned-0.2.7/firestone/spec/_base.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.6/firestone/spec/asyncapi.py` & `firestoned-0.2.7/firestone/spec/asyncapi.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.6/firestone/spec/cli.py` & `firestoned-0.2.7/firestone/spec/cli.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.6/firestone/spec/openapi.py` & `firestoned-0.2.7/firestone/spec/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 # pylint: disable=duplicate-code
 
 import copy
 import http.client
 import logging
 
 import yaml
+import inflect
 
 from firestone.spec import _base as spec_base
 
 # This is a list of all HTTP methods supported on high-level resource base
 RSRC_HTTP_METHODS = ["delete", "get", "head", "patch", "post"]
 
 # This is a list of all HTTP methods supported on an instance of a resource
 RSRC_INST_HTTP_METHODS = ["delete", "get", "head", "patch", "put"]
 
 # This is a list of all HTTP methods supported on attributes of an instance of a resource
 RSRC_ATTR_HTTP_METHODS = ["delete", "get", "head", "put"]
 
+INFLECT_ENGINE = inflect.engine()
+
 _LOGGER = logging.getLogger(__name__)
 
 # TODO add support for JSON Patch: https://www.jvt.me/posts/2022/05/29/openapi-json-patch/
 
 
 def get_responses(
     method: str,
```

### Comparing `firestoned-0.2.6/pyproject.toml` & `firestoned-0.2.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firestoned"
-version = "0.2.6"
+version = "0.2.7"
 description = "Build OpenAPI and AsyncAPI specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/firestoned/firestone"
 packages = [
     { include = "firestone" }
@@ -19,14 +19,15 @@
 jsonschema = "^4.16.0"
 pyyaml = "^6.0"
 jsonref = "^1.0.0.post1"
 firestone-lib = "^0.1.0"
 pydantic = "^1.10.5"
 python-dateutil = "^2.8.2"
 aiohttp = "^3.8.4"
+inflect = "^6.0.4"
 
 [tool.poetry.group.asyncapi.dependencies]
 asyncapi = {extras = ["http"], version = "^0.14.1"}
 requests = "^2.28.1"
 websockets = "^10.4"
 typer = "^0.7.0"
 uvicorn = "^0.19.0"
```

### Comparing `firestoned-0.2.6/PKG-INFO` & `firestoned-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestoned
-Version: 0.2.6
+Version: 0.2.7
 Summary: Build OpenAPI and AsyncAPI specs based off one or more resource json schema files
 Home-page: https://github.com/firestoned/firestone
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: caching
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: firestone-lib (>=0.1.0,<0.2.0)
+Requires-Dist: inflect (>=6.0.4,<7.0.0)
 Requires-Dist: jsonref (>=1.0.0.post1,<2.0.0)
 Requires-Dist: jsonschema (>=4.16.0,<5.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: quart (>=0.18.3,<0.19.0) ; extra == "caching"
 Requires-Dist: setuptools (>=65.5.0,<66.0.0)
```

#### html2text {}

```diff
@@ -1,129 +1,130 @@
-Metadata-Version: 2.1 Name: firestoned Version: 0.2.6 Summary: Build OpenAPI
+Metadata-Version: 2.1 Name: firestoned Version: 0.2.7 Summary: Build OpenAPI
 and AsyncAPI specs based off one or more resource json schema files Home-page:
 https://github.com/firestoned/firestone License: Apache 2.0 Author: Erick
 Bourgeois Author-email: erick@jeb.ca Requires-Python: >=3.8,<4.0 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: caching
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: firestone-lib
-(>=0.1.0,<0.2.0) Requires-Dist: jsonref (>=1.0.0.post1,<2.0.0) Requires-Dist:
-jsonschema (>=4.16.0,<5.0.0) Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: pyyaml
-(>=6.0,<7.0) Requires-Dist: quart (>=0.18.3,<0.19.0) ; extra == "caching"
-Requires-Dist: setuptools (>=65.5.0,<66.0.0) Project-URL: Repository, https://
-github.com/firestoned/firestone Description-Content-Type: text/markdown [![Last
-PR Build ð](https://github.com/firestoned/firestone/actions/workflows/
-pr.yml/badge.svg)](https://github.com/firestoned/firestone/actions/workflows/
-pr.yml)  [Coverage]  # Firestone Resource-Based Approach to Building APIs
-``firestone`` allows you to build OpenAPI, AsyncAPI and gRPC specs based off
-one or more resource json schema files. This allows you to focus on what really
-matters, the resource you are developing! Once you have generated the
-appropriate specification file for your project, you can then use the myriad of
-libraries and frameworks to generate stub code for you. **The primary premise
-of this project is not to introduce any new "language" to describe your
-resources(s), use JSON Schema!** THis makes it easy to come up to speed and
-little to no prior knowledge to get going. Having said that, the schema for a
-resource provides additional helpful functionality, see [schema](#schema)
-section. ## Quick Start You can use pip or poetry to install and run
-``firestone``. We suggest using pip if you wish to install `firestone``
-machine-wide, else, for local use, use poetry. ### pip It's a simple as running
-the following ``pip`` command: ``` sudo pip install firestoned ``` NOTE: yes,
-`firestone**d**`, not `firestone`! This is because there already is a, albeit
-emtpy, repo on pypi.org with the same name... ### poetry [Poetry](https://
-python-poetry.org/) is a great build tool for python that allows you to build
-and run all locally in a virtual environment. This is great for checking out
-the tool and playing around with `firestone` itself. ``` brew install poetry
-poetry install poetry build ``` ## Running Now that you have a copy of
-``firestone``, let's try running it with the example resource provided, an
-addressbook! Note: if running within poetry build, simply prepend commands with
-``poetry run`` For the remainder of this documentation, we will assume you have
-installed firestone. ### Generate an OpenAPI Spec ``` firestone \ generate \ --
-title 'Addressbook resource' \ --description 'A simple addressBook example' \ -
--resources examples/addressBook/resource.yaml \ openapi --security '{"name":
-"bearer_auth", "scheme": "bearer", "type": "http", "bearerFormat": "JWT"}' \
+(>=0.1.0,<0.2.0) Requires-Dist: inflect (>=6.0.4,<7.0.0) Requires-Dist: jsonref
+(>=1.0.0.post1,<2.0.0) Requires-Dist: jsonschema (>=4.16.0,<5.0.0) Requires-
+Dist: pydantic (>=1.10.5,<2.0.0) Requires-Dist: python-dateutil
+(>=2.8.2,<3.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: quart
+(>=0.18.3,<0.19.0) ; extra == "caching" Requires-Dist: setuptools
+(>=65.5.0,<66.0.0) Project-URL: Repository, https://github.com/firestoned/
+firestone Description-Content-Type: text/markdown [![Last PR Build ð](https:
+//github.com/firestoned/firestone/actions/workflows/pr.yml/badge.svg)](https://
+github.com/firestoned/firestone/actions/workflows/pr.yml)  [Coverage]  #
+Firestone Resource-Based Approach to Building APIs ``firestone`` allows you to
+build OpenAPI, AsyncAPI and gRPC specs based off one or more resource json
+schema files. This allows you to focus on what really matters, the resource you
+are developing! Once you have generated the appropriate specification file for
+your project, you can then use the myriad of libraries and frameworks to
+generate stub code for you. **The primary premise of this project is not to
+introduce any new "language" to describe your resources(s), use JSON Schema!**
+THis makes it easy to come up to speed and little to no prior knowledge to get
+going. Having said that, the schema for a resource provides additional helpful
+functionality, see [schema](#schema) section. ## Quick Start You can use pip or
+poetry to install and run ``firestone``. We suggest using pip if you wish to
+install `firestone`` machine-wide, else, for local use, use poetry. ### pip
+It's a simple as running the following ``pip`` command: ``` sudo pip install
+firestoned ``` NOTE: yes, `firestone**d**`, not `firestone`! This is because
+there already is a, albeit emtpy, repo on pypi.org with the same name... ###
+poetry [Poetry](https://python-poetry.org/) is a great build tool for python
+that allows you to build and run all locally in a virtual environment. This is
+great for checking out the tool and playing around with `firestone` itself. ```
+brew install poetry poetry install poetry build ``` ## Running Now that you
+have a copy of ``firestone``, let's try running it with the example resource
+provided, an addressbook! Note: if running within poetry build, simply prepend
+commands with ``poetry run`` For the remainder of this documentation, we will
+assume you have installed firestone. ### Generate an OpenAPI Spec ``` firestone
+\ generate \ --title 'Addressbook resource' \ --description 'A simple
+addressBook example' \ --resources examples/addressBook/resource.yaml \ openapi
+--security '{"name": "bearer_auth", "scheme": "bearer", "type": "http",
+"bearerFormat": "JWT"}' \ ``` Let's quickly dissect this command: - we are
+telling firestone to generate an `openapi` spec, given the ``title``,
+``description`` and the two given resource files. - By default, this will
+output the specification file to stdout, alternatively you can provide the `-O`
+option to output to a specific file. You can also, add the command line `--ui-
+server` tot he end, which will launch a small webserver and run the Swagger UI
+to view this specification file. ``` firestone --debug generate --title
+'Example person and addressBook API' \ --description 'An example API with more
+than one resource' \ --resources examples/addressBook.yaml,examples/person.yaml
+\ openapi \ --security '{"name": "bearer_auth", "scheme": "bearer", "type":
+"http", "bearerFormat": "JWT"}' \ --ui-server # ... * Serving Quart app
+'firestone.__main__' * Environment: production * Please use an ASGI server
+(e.g. Hypercorn) directly in production * Debug mode: False * Running on http:/
+/127.0.0.1:5000 (CTRL + C to quit) [2022-10-31 02:47:17 -0500] [87590] [INFO]
+Running on http://127.0.0.1:5000 (CTRL + C to quit) # 2022-10-31 02:47:17,120 -
+[MainThread] hypercorn.error:102 INFO - Running on http://127.0.0.1:5000 (CTRL
++ C to quit) ``` Now you can use your browser to navigate to `http://127.0.0.1:
+5000/apidocs` ## Schema It all begins with your resource definition! This is
+done using JSON schema and we have provided an example in our `examples`
+directory, called addressBook. We will use this to describe how the schema is
+setup and how you can adapt to your own. Here is the full file: ```yaml name:
+addressBook description: An example of an addressBook resource version: 1.0
+version_in_path: false default_query_params: - name: limit description: Limit
+the number of responses back in: params schema: type: integer - name: offset
+description: The offset to start returning resources in: params schema: type:
+integer descriptions: resource: get: List all addresses in this addressbook.
+head: Determine the existence and size of addresses in this addressbook. patch:
+Patch one or more addresses in this addressbook. post: Create a new address in
+this addressbook, a new address key will be created. delete: Delete all
+addresses from this addressbook. instance: get: Get a specific address from
+this addressbook. head: Determine the existence and size of this address.
+patch: Patch this address in the addressbook. put: Put a new address in this
+addressbook, with the given address key. delete: Delete an address from this
+addressbook. schema: type: array key: name: address_key schema: description: A
+unique identifier for an addressbook entry. type: string #responseCodes: # -
+200 # - 201 query_params: - name: city description: Filter by city name schema:
+type: string methods: - get items: type: object properties: addrtype:
+description: The address type, e.g. work or home type: string enum: - work -
+home street: description: The street and civic number of this address type:
+string city: description: The city of this address type: string state:
+description: The state of this address type: string country: description: The
+country of this address type: string ``` ### Metadata There is a certain amount
+of metadata that all of these specifications use/require, and this is done at
+the top of the resource,yaml; for posterity, they are: ```yaml name:
+addressBook description: An example of an addressBook resource version: 1.0 ```
+#### `name` The name is used in various places, including as the root to API
+URLs, for example in OpenAPI, `/addressBook` #### `description` This is self
+evident, I hope, the description of this resource and is used nt he generated
+specification files. #### `descriptions` This is a map/dict of either
+`resource` and/or `instance`, which itself is a map or methods to descriptions,
+e.g.: ```yaml descriptions: resource: get: List all addresses in this
+addressbook. head: Determine the existence and size of addresses in this
+addressbook. patch: Patch one or more addresses in this addressbook. post:
+Create a new address in this addressbook, a new address key will be created.
+delete: Delete all addresses from this addressbook. ``` #### `methods` This is
+a map/dict of `resource`, and/or `instance`, and/or `instance_attrs` (the
+instance attributes to expose), and a list of methods to explicitly expose,
+e.g.: ```yaml methods: resource: - get - post - put ``` #### `version` The
+version of this resource definition, this cna alternatively be used in the URL
+as well, see below `version_in_path` #### `version_in_path` This attribute
+defines whether to prepend the version defined above in the URL paths, e.g.,
+for the above, you would get: `/v1.0/addressBook`. #### `default_query_params`
+You can provide a list of default query parameters that will be added to all
+HTTP methods, or optionally you can provide a list of the HTTP methods, for
+which `firestone` will add. ### Generate OpenAPI Client Now, to generate your
+OpenAPI client, you will need the `openapi-generator` command, and this can be
+used to generate client code in many languages. For more details on this
+project, see [here](https://openapi-generator.tech/). This client code can then
+be used as an SDK or used by our CLI generation, see below. ``` openapi-
+generator generate \ -i examples/addressbook/openapi.yaml \ -g python-nextgen \
+-o /tmp/addressbook-client \ --skip-validate-spec \ -c examples/addressbook/
+openapi-gen-config.json ``` ### Generate Python CRUD CLI Now that you have
+generated the client code, you can also generate a CRUD, Python Click-based CLI
+around your code. This generator creates a standalone script or as a module to
+be used in your console scripts, as part of your project build. Here is an
+example command we use to generate the example Addressbook. ``` firestone
+generate \ --title 'Addressbook CLI' \ --description 'This is the CLI for the
+example Addressbook' \ --resources examples/addressbook/
+addressbook.yaml,examples/addressbook/person.yaml \ --version 1.0 \ cli \ --pkg
+addressbook \ --client-pkg addressbook.client > examples/addressbook/main.py
 ``` Let's quickly dissect this command: - we are telling firestone to generate
 an `openapi` spec, given the ``title``, ``description`` and the two given
 resource files. - By default, this will output the specification file to
 stdout, alternatively you can provide the `-O` option to output to a specific
-file. You can also, add the command line `--ui-server` tot he end, which will
-launch a small webserver and run the Swagger UI to view this specification
-file. ``` firestone --debug generate --title 'Example person and addressBook
-API' \ --description 'An example API with more than one resource' \ --resources
-examples/addressBook.yaml,examples/person.yaml \ openapi \ --security '{"name":
-"bearer_auth", "scheme": "bearer", "type": "http", "bearerFormat": "JWT"}' \ --
-ui-server # ... * Serving Quart app 'firestone.__main__' * Environment:
-production * Please use an ASGI server (e.g. Hypercorn) directly in production
-* Debug mode: False * Running on http://127.0.0.1:5000 (CTRL + C to quit)
-[2022-10-31 02:47:17 -0500] [87590] [INFO] Running on http://127.0.0.1:5000
-(CTRL + C to quit) # 2022-10-31 02:47:17,120 - [MainThread] hypercorn.error:102
-INFO - Running on http://127.0.0.1:5000 (CTRL + C to quit) ``` Now you can use
-your browser to navigate to `http://127.0.0.1:5000/apidocs` ## Schema It all
-begins with your resource definition! This is done using JSON schema and we
-have provided an example in our `examples` directory, called addressBook. We
-will use this to describe how the schema is setup and how you can adapt to your
-own. Here is the full file: ```yaml name: addressBook description: An example
-of an addressBook resource version: 1.0 version_in_path: false
-default_query_params: - name: limit description: Limit the number of responses
-back in: params schema: type: integer - name: offset description: The offset to
-start returning resources in: params schema: type: integer descriptions:
-resource: get: List all addresses in this addressbook. head: Determine the
-existence and size of addresses in this addressbook. patch: Patch one or more
-addresses in this addressbook. post: Create a new address in this addressbook,
-a new address key will be created. delete: Delete all addresses from this
-addressbook. instance: get: Get a specific address from this addressbook. head:
-Determine the existence and size of this address. patch: Patch this address in
-the addressbook. put: Put a new address in this addressbook, with the given
-address key. delete: Delete an address from this addressbook. schema: type:
-array key: name: address_key schema: description: A unique identifier for an
-addressbook entry. type: string #responseCodes: # - 200 # - 201 query_params: -
-name: city description: Filter by city name schema: type: string methods: - get
-items: type: object properties: addrtype: description: The address type, e.g.
-work or home type: string enum: - work - home street: description: The street
-and civic number of this address type: string city: description: The city of
-this address type: string state: description: The state of this address type:
-string country: description: The country of this address type: string ``` ###
-Metadata There is a certain amount of metadata that all of these specifications
-use/require, and this is done at the top of the resource,yaml; for posterity,
-they are: ```yaml name: addressBook description: An example of an addressBook
-resource version: 1.0 ``` #### `name` The name is used in various places,
-including as the root to API URLs, for example in OpenAPI, `/addressBook` ####
-`description` This is self evident, I hope, the description of this resource
-and is used nt he generated specification files. #### `descriptions` This is a
-map/dict of either `resource` and/or `instance`, which itself is a map or
-methods to descriptions, e.g.: ```yaml descriptions: resource: get: List all
-addresses in this addressbook. head: Determine the existence and size of
-addresses in this addressbook. patch: Patch one or more addresses in this
-addressbook. post: Create a new address in this addressbook, a new address key
-will be created. delete: Delete all addresses from this addressbook. ``` ####
-`methods` This is a map/dict of `resource`, and/or `instance`, and/or
-`instance_attrs` (the instance attributes to expose), and a list of methods to
-explicitly expose, e.g.: ```yaml methods: resource: - get - post - put ``` ####
-`version` The version of this resource definition, this cna alternatively be
-used in the URL as well, see below `version_in_path` #### `version_in_path`
-This attribute defines whether to prepend the version defined above in the URL
-paths, e.g., for the above, you would get: `/v1.0/addressBook`. ####
-`default_query_params` You can provide a list of default query parameters that
-will be added to all HTTP methods, or optionally you can provide a list of the
-HTTP methods, for which `firestone` will add. ### Generate OpenAPI Client Now,
-to generate your OpenAPI client, you will need the `openapi-generator` command,
-and this can be used to generate client code in many languages. For more
-details on this project, see [here](https://openapi-generator.tech/). This
-client code can then be used as an SDK or used by our CLI generation, see
-below. ``` openapi-generator generate \ -i examples/addressbook/openapi.yaml \
--g python-nextgen \ -o /tmp/addressbook-client \ --skip-validate-spec \ -
-c examples/addressbook/openapi-gen-config.json ``` ### Generate Python CRUD CLI
-Now that you have generated the client code, you can also generate a CRUD,
-Python Click-based CLI around your code. This generator creates a standalone
-script or as a module to be used in your console scripts, as part of your
-project build. Here is an example command we use to generate the example
-Addressbook. ``` firestone generate \ --title 'Addressbook CLI' \ --description
-'This is the CLI for the example Addressbook' \ --resources examples/
-addressbook/addressbook.yaml,examples/addressbook/person.yaml \ --version 1.0 \
-cli \ --pkg addressbook \ --client-pkg addressbook.client > examples/
-addressbook/main.py ``` Let's quickly dissect this command: - we are telling
-firestone to generate an `openapi` spec, given the ``title``, ``description``
-and the two given resource files. - By default, this will output the
-specification file to stdout, alternatively you can provide the `-O` option to
-output to a specific file. ## Contributing
+file. ## Contributing
```

