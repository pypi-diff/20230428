# Comparing `tmp/mysql_type_plugin-0.1.8.tar.gz` & `tmp/mysql_type_plugin-0.1.9.tar.gz`

## Comparing `mysql_type_plugin-0.1.8.tar` & `mysql_type_plugin-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 mysql_type_plugin-0.1.8/Cargo.toml
--rw-rw-r--   0        0        0       22 2022-04-25 13:41:42.000000 mysql_type_plugin-0.1.8/.dockerignore
--rw-rw-r--   0        0        0     1548 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.8/.github/workflows/CI.yml
--rw-rw-r--   0        0        0      685 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.8/.gitignore
--rw-rw-r--   0        0        0      215 2022-04-25 13:41:42.000000 mysql_type_plugin-0.1.8/.pypirc
--rw-rw-r--   0        0        0      361 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.8/Cargo.toml~
--rw-rw-r--   0        0        0      502 2022-04-26 11:20:00.000000 mysql_type_plugin-0.1.8/Dockerfile
--rw-rw-r--   0        0        0       23 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.8/README.md
--rwxrwxr-x   0        0        0      519 2022-04-26 11:20:00.000000 mysql_type_plugin-0.1.8/build.sh
--rw-rw-r--   0        0        0    13431 2022-04-26 11:19:44.000000 mysql_type_plugin-0.1.8/mysql_type_plugin/__init__.py
--rw-rw-r--   0        0        0    13431 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.8/mysql_type_plugin/__init__.py~
--rw-rw-r--   0        0        0      231 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.8/pyproject.toml
--rw-rw-r--   0        0        0     9733 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.8/src/lib.rs
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 mysql_type_plugin-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 mysql_type_plugin-0.1.9/Cargo.toml
+-rw-rw-r--   0        0        0       22 2022-04-25 13:41:42.000000 mysql_type_plugin-0.1.9/.dockerignore
+-rw-rw-r--   0        0        0     1548 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.9/.github/workflows/CI.yml
+-rw-rw-r--   0        0        0      685 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.9/.gitignore
+-rw-rw-r--   0        0        0      215 2022-04-25 13:41:42.000000 mysql_type_plugin-0.1.9/.pypirc
+-rw-rw-r--   0        0        0      361 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.9/Cargo.toml~
+-rw-rw-r--   0        0        0      502 2022-04-26 11:20:00.000000 mysql_type_plugin-0.1.9/Dockerfile
+-rw-rw-r--   0        0        0       23 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.9/README.md
+-rwxrwxr-x   0        0        0      519 2022-04-26 11:20:00.000000 mysql_type_plugin-0.1.9/build.sh
+-rw-rw-r--   0        0        0    11741 2022-05-03 14:32:27.000000 mysql_type_plugin-0.1.9/mysql_type_plugin/__init__.py
+-rw-rw-r--   0        0        0    13431 2022-04-25 13:41:41.000000 mysql_type_plugin-0.1.9/mysql_type_plugin/__init__.py~
+-rw-rw-r--   0        0        0      231 2022-05-03 14:32:27.000000 mysql_type_plugin-0.1.9/pyproject.toml
+-rw-rw-r--   0        0        0    10073 2022-05-03 14:32:27.000000 mysql_type_plugin-0.1.9/src/lib.rs
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 mysql_type_plugin-0.1.9/PKG-INFO
```

### Comparing `mysql_type_plugin-0.1.8/.github/workflows/CI.yml` & `mysql_type_plugin-0.1.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `mysql_type_plugin-0.1.8/.gitignore` & `mysql_type_plugin-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mysql_type_plugin-0.1.8/build.sh` & `mysql_type_plugin-0.1.9/build.sh`

 * *Files identical despite different names*

### Comparing `mysql_type_plugin-0.1.8/mysql_type_plugin/__init__.py` & `mysql_type_plugin-0.1.9/mysql_type_plugin/__init__.py~`

 * *Files identical despite different names*

### Comparing `mysql_type_plugin-0.1.8/mysql_type_plugin/__init__.py~` & `mysql_type_plugin-0.1.9/mysql_type_plugin/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,45 +105,51 @@
     if err and not quiet:
         api.fail(message, context)
     elif message and not quiet:
         if note := getattr(api, "note"):
             note(message, context)
     return stmt
 
+def map_type(v: Any, not_null: bool, api: CheckerPluginInterface, context: Context) -> Type:
+    t: Type = AnyType(TypeOfAny.special_form)
+    if isinstance(v, rs.Integer):
+        t = api.named_generic_type("int", [])
+    elif isinstance(v, rs.Float):
+        t = api.named_generic_type("float", [])
+    elif isinstance(v, rs.String):
+        t = api.named_generic_type("str", [])
+    elif isinstance(v, rs.Bool):
+        t = api.named_generic_type("bool", [])
+    elif isinstance(v, rs.Bytes):
+        t = api.named_generic_type("bytes", [])
+    elif isinstance(v, rs.Enum):
+        t = api.named_generic_type("str", [])  # TODO literal with values
+    elif isinstance(v, rs.List):
+        return api.named_generic_type(
+            "typing.Sequence", [map_type(v.type, not_null, api, context)]
+        )
+    elif isinstance(v, rs.Any):
+        t = AnyType(TypeOfAny.special_form)
+    else:
+        api.fail(f"Unknown type {v}", context)
+    if not not_null:
+        t = UnionType((t, NoneType()))
+    return t
 
 def get_argument_types(
     stmt: Any, api: CheckerPluginInterface, context: Context
 ) -> List[Type]:
     ts: List[Type] = []
     if args := getattr(stmt, "arguments", None):
         for k, (v, not_null) in args.items():
             if not isinstance(k, int):
                 continue
             while len(ts) <= k:
                 ts.append(AnyType(TypeOfAny.special_form))
-            t: Type = AnyType(TypeOfAny.special_form)
-            if isinstance(v, rs.Integer):
-                t = api.named_generic_type("int", [])
-            elif isinstance(v, rs.Float):
-                t = api.named_generic_type("float", [])
-            elif isinstance(v, rs.String):
-                t = api.named_generic_type("str", [])
-            elif isinstance(v, rs.Bool):
-                t = api.named_generic_type("bool", [])
-            elif isinstance(v, rs.Bytes):
-                t = api.named_generic_type("bytes", [])
-            elif isinstance(v, rs.Enum):
-                t = api.named_generic_type("str", [])  # TODO literal with values
-            elif isinstance(v, rs.Any):
-                t = AnyType(TypeOfAny.special_form)
-            else:
-                api.fail(f"Unknown type {v}", context)
-            if not not_null:
-                t = UnionType((t, NoneType()))
-            ts[k] = t
+            ts[k] = map_type(v, not_null, api, context)
     return ts
 
 
 class CustomPlugin(Plugin):
     def get_function_signature_hook(
         self, fullname: str
     ) -> Optional[Callable[[FunctionSigContext], CallableType]]:
@@ -156,16 +162,15 @@
 
         def execute_hook(context: FunctionSigContext) -> CallableType:
             try:
                 sql = get_sql(1, context.args, context.api, quiet=True)
                 if sql is None:
                     return context.default_signature
 
-                sql2 = sql.replace("_LIST_", "%s, %s, %s")
-                stmt = type_statement(sql2, context.api, context.context, dict_cursor=False, quiet=True)
+                stmt = type_statement(sql, context.api, context.context, dict_cursor=False, quiet=True)
                 if stmt is None:
                     return context.default_signature
                 ans = CallableType(
                     [
                         context.default_signature.arg_types[0],
                         context.api.named_generic_type("str", []),
                     ],
@@ -173,31 +178,18 @@
                     ["cursor", "sql"],
                     context.default_signature.ret_type,
                     context.default_signature.fallback,
                     variables=context.default_signature.variables,
                 )
 
                 at = get_argument_types(stmt, context.api, context.context)
-
-                ati = iter(at)
-                for i, a in enumerate(re.findall("(_LIST_|[%]s|[%]\()", sql)):
-                    try:
-                        if a == "_LIST_":
-                            t = context.api.named_generic_type(
-                                "typing.Sequence", [next(ati)]
-                            )
-                            next(ati)
-                            next(ati)
-                        else:
-                            t = next(ati)
-                        ans.arg_types.append(t)
-                        ans.arg_names.append(f"a{i}")
-                        ans.arg_kinds.append(ARG_POS)
-                    except StopIteration:
-                        context.api.fail(f"Argument match failed {i}", context.context)
+                for i, t in enumerate(at):
+                    ans.arg_types.append(t)
+                    ans.arg_names.append(f"a{i}")
+                    ans.arg_kinds.append(ARG_POS)
                 return ans
             except Exception as e:
                 context.api.fail(f"ICE: {e}", context.context)
                 return context.default_signature
 
         return execute_hook
 
@@ -225,43 +217,22 @@
                         context.api.fail(f"Unknown cursor {ct}", context.context)
                 except AttributeError:
                     context.api.fail(f"Unknown cursor {ct}", context.context)
 
                 sql = get_sql(1, context.args, api, quiet=False)
                 if sql is None:
                     return context.default_return_type
-                sql = sql.replace("_LIST_", "%s")
                 stmt = type_statement(sql, api, context.context, dict_cursor=dc,quiet=False)
                 if stmt is None:
                     return context.default_return_type
 
                 if isinstance(stmt, rs.Select):
                     ntp: List[Tuple[str, Type]] = []
                     for (name, type_, not_null) in stmt.columns:
-                        t: Type
-                        if isinstance(type_, rs.Integer):
-                            t = api.named_generic_type("int", [])
-                        elif isinstance(type_, rs.Float):
-                            t = api.named_generic_type("float", [])
-                        elif isinstance(type_, rs.String):
-                            t = api.named_generic_type("str", [])
-                        elif isinstance(type_, rs.Bool):
-                            t = api.named_generic_type("int", [])  # TODO literal 0,1
-                        elif isinstance(type_, rs.Enum):
-                            t = api.named_generic_type(
-                                "str", []
-                            )  # TODO literal with values
-                        elif isinstance(type_, rs.Bytes):
-                            t = api.named_generic_type("bytes", [])
-                        elif isinstance(type_, rs.Any):
-                            t = AnyType(TypeOfAny.special_form)
-                        else:
-                            api.fail(f"Unknown type {type_}", context.context)
-                        if not not_null:
-                            t = UnionType((t, NoneType()))
+                        t = map_type(type_, not_null, api, context.context)
                         ntp.append((name, t))
                     if sr := self.lookup_fully_qualified("mysql_type.SelectResult"):
                         if dc:
                             return Instance(
                                 sr.node, # type: ignore
                                 [TypedDictType(
                                     OrderedDict(ntp),
```

### Comparing `mysql_type_plugin-0.1.8/src/lib.rs` & `mysql_type_plugin-0.1.9/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -117,35 +117,43 @@
 
 #[pyclass]
 struct Enum {
     #[pyo3(get)]
     values: Vec<std::string::String>,
 }
 
+#[pyclass]
+struct List {
+    #[pyo3(get)]
+    r#type: PyObject,
+}
+
 #[derive(Clone)]
 enum Type {
     Any,
     Integer,
     Float,
     Bool,
     Bytes,
     String,
     Enum(Vec<std::string::String>),
+    List(Box<Type>)
 }
 
 impl IntoPy<PyObject> for Type {
     fn into_py(self, py: Python) -> PyObject {
         match self {
             Type::Any => Py::new(py, Any {}).unwrap().to_object(py),
             Type::Integer => Py::new(py, Integer {}).unwrap().to_object(py),
             Type::Float => Py::new(py, Float {}).unwrap().to_object(py),
             Type::Bool => Py::new(py, Bool {}).unwrap().to_object(py),
             Type::Bytes => Py::new(py, Bytes {}).unwrap().to_object(py),
             Type::String => Py::new(py, String {}).unwrap().to_object(py),
             Type::Enum(values) => Py::new(py, Enum { values }).unwrap().to_object(py),
+            Type::List(r#type) => Py::new(py,List{r#type: r#type.into_py(py)}).unwrap().to_object(py),
         }
     }
 }
 
 #[pyclass]
 struct Select {
     #[pyo3(get)]
@@ -181,16 +189,16 @@
     #[pyo3(get)]
     arguments: HashMap<ArgumentKey, (Type, bool)>,
 }
 
 #[pyclass]
 struct Invalid {}
 
-fn map_type(t: sql_type::Type<'_>) -> Type {
-    match t {
+fn map_type(t: &sql_type::FullType<'_>) -> Type {
+    let b = match &t.t {
         sql_type::Type::Args(_, _) => Type::Any,
         sql_type::Type::Base(v) => {
             match v {
                 sql_type::BaseType::Any => Type::Any,
                 sql_type::BaseType::Bool => Type::Bool,
                 sql_type::BaseType::Bytes => Type::Bytes,
                 sql_type::BaseType::Date => Type::Any, //TODO
@@ -213,28 +221,33 @@
         sql_type::Type::JSON => Type::Any,
         sql_type::Type::Set(_) => Type::String,
         sql_type::Type::U16 => Type::Integer,
         sql_type::Type::U32 => Type::Integer,
         sql_type::Type::U64 => Type::Integer,
         sql_type::Type::U8 => Type::Integer,
         sql_type::Type::Null => Type::Any,
+    };
+    if t.list_hack {
+        Type::List(Box::new(b))
+    } else {
+        b
     }
 }
 
 fn map_arguments(
     arguments: Vec<(sql_type::ArgumentKey<'_>, sql_type::FullType<'_>)>,
 ) -> HashMap<ArgumentKey, (Type, bool)> {
     arguments
         .into_iter()
         .map(|(k, v)| {
             let k = match k {
                 sql_type::ArgumentKey::Index(i) => ArgumentKey::Index(i),
                 sql_type::ArgumentKey::Identifier(i) => ArgumentKey::Identifier(i.to_string()),
             };
-            (k, (map_type(v.t), v.not_null))
+            (k, (map_type(&v), v.not_null))
         })
         .collect()
 }
 
 #[pyfunction]
 fn type_statement(
     py: Python,
@@ -242,15 +255,16 @@
     statement: &str,
     dict_result: bool,
 ) -> PyResult<(PyObject, bool, std::string::String)> {
     let mut issues = Vec::new();
 
     let mut options = TypeOptions::new()
         .dialect(SQLDialect::MariaDB)
-        .arguments(SQLArguments::Percent);
+        .arguments(SQLArguments::Percent)
+        .list_hack(true);
 
     if dict_result {
         options = options
             .warn_duplicate_column_in_select(true)
             .warn_unnamed_column_in_select(true);
     }
 
@@ -259,15 +273,15 @@
     let res = match stmt {
         sql_type::StatementType::Select { columns, arguments } => {
             let columns = columns
                 .into_iter()
                 .map(|v| {
                     (
                         v.name.map(|v| v.to_string()),
-                        map_type(v.type_.t),
+                        map_type(&v.type_),
                         v.type_.not_null,
                     )
                 })
                 .collect();
             Py::new(
                 py,
                 Select {
@@ -336,10 +350,11 @@
     m.add_class::<Integer>()?;
     m.add_class::<Bool>()?;
     m.add_class::<Any>()?;
     m.add_class::<Float>()?;
     m.add_class::<Bytes>()?;
     m.add_class::<String>()?;
     m.add_class::<Enum>()?;
+    m.add_class::<List>()?;
     m.add_class::<Schemas>()?;
     Ok(())
 }
```

