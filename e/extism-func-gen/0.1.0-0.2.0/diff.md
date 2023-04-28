# Comparing `tmp/extism_func_gen-0.1.0.tar.gz` & `tmp/extism_func_gen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extism_func_gen-0.1.0.tar", max compression
+gzip compressed data, was "extism_func_gen-0.2.0.tar", max compression
```

## Comparing `extism_func_gen-0.1.0.tar` & `extism_func_gen-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      345 2023-04-27 17:01:38.009735 extism_func_gen-0.1.0/README.md
--rw-r--r--   0        0        0     2745 2023-04-27 16:46:25.629254 extism_func_gen-0.1.0/func_gen/__init__.py
--rw-r--r--   0        0        0   958069 2023-04-27 16:34:39.047735 extism_func_gen-0.1.0/func_gen/eval.wasm
--rw-r--r--   0        0        0      437 2023-04-27 17:23:26.407512 extism_func_gen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 extism_func_gen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      731 2023-04-28 20:12:31.368439 extism_func_gen-0.2.0/README.md
+-rw-r--r--   0        0        0     3086 2023-04-28 20:22:00.982673 extism_func_gen-0.2.0/func_gen/__init__.py
+-rw-r--r--   0        0        0   958069 2023-04-27 16:34:39.047735 extism_func_gen-0.2.0/func_gen/eval.wasm
+-rw-r--r--   0        0        0      437 2023-04-28 20:22:05.718481 extism_func_gen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 extism_func_gen-0.2.0/PKG-INFO
```

### Comparing `extism_func_gen-0.1.0/func_gen/__init__.py` & `extism_func_gen-0.2.0/func_gen/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,28 +42,39 @@
     with Context() as context:
         plugin = context.plugin(config, wasi=True)
         plugin.call("register_function", code)
         return plugin.call("invoke", input)
 
 def init_argparse():
     parser = argparse.ArgumentParser(
-        usage="%(prog)s FUNC_NAME [OPTIONS]",
+        usage="%(prog)s [FUNC_NAME] [OPTIONS]",
         description="Create and execute text processing functions by English descriptions"
     )
-    parser.add_argument('func_name', type=str)
+    parser.add_argument('func_name', type=str, nargs='?')
     parser.add_argument('-d', '--description', type=str, nargs='?')
+    parser.add_argument('-l', '--list', action=argparse.BooleanOptionalAction)
     return parser
 
 def main():
     parser = init_argparse()
     args = parser.parse_args()
 
     if not os.path.exists(HOME_DIR):
         os.makedirs(HOME_DIR)
 
+    if args.list:
+        import glob
+        for f in glob.glob(str(HOME_DIR / "*.js")):
+            print(os.path.basename(f)[:-3])
+        exit(0)
+
+    if not args.func_name:
+        print("Function name is a required argument")
+        exit(1)
+
     if args.description:
         code = generate_code(args.description)
         with open(HOME_DIR / f"{args.func_name}.js", 'w') as file:
             file.write(code)
         print(code)
         exit(0)
```

### Comparing `extism_func_gen-0.1.0/func_gen/eval.wasm` & `extism_func_gen-0.2.0/func_gen/eval.wasm`

 * *Files identical despite different names*

