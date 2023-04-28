# Comparing `tmp/scorpionsql-0.0.5.tar.gz` & `tmp/scorpionsql-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scorpionsql-0.0.5.tar", last modified: Fri Apr 28 16:38:04 2023, max compression
+gzip compressed data, was "dist/scorpionsql-0.0.6.tar", last modified: Fri Apr 28 16:58:06 2023, max compression
```

## Comparing `scorpionsql-0.0.5.tar` & `scorpionsql-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eugenewu   (502) staff       (20)        0 2023-04-28 16:38:04.622840 scorpionsql-0.0.5/
--rw-r--r--   0 eugenewu   (502) staff       (20)     1054 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/LICENSE
--rw-r--r--   0 eugenewu   (502) staff       (20)      264 2023-04-28 16:38:04.622899 scorpionsql-0.0.5/PKG-INFO
--rw-r--r--   0 eugenewu   (502) staff       (20)      132 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/README.md
-drwxr-xr-x   0 eugenewu   (502) staff       (20)        0 2023-04-28 16:38:04.621984 scorpionsql-0.0.5/scorpionsql/
--rw-r--r--   0 eugenewu   (502) staff       (20)       22 2023-04-28 16:34:11.000000 scorpionsql-0.0.5/scorpionsql/__init__.py
--rw-r--r--   0 eugenewu   (502) staff       (20)     1797 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/aggerror.py
--rwxr-xr-x   0 eugenewu   (502) staff       (20)     2428 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/db.py
--rw-r--r--   0 eugenewu   (502) staff       (20)    10590 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/errfunc.py
--rw-r--r--   0 eugenewu   (502) staff       (20)     8681 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/functions.py
--rw-r--r--   0 eugenewu   (502) staff       (20)       36 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/settings.py
--rw-r--r--   0 eugenewu   (502) staff       (20)     8175 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/sql.py
--rw-r--r--   0 eugenewu   (502) staff       (20)     5080 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/sqlparser.py
-drwxr-xr-x   0 eugenewu   (502) staff       (20)        0 2023-04-28 16:38:04.622721 scorpionsql-0.0.5/scorpionsql.egg-info/
--rw-r--r--   0 eugenewu   (502) staff       (20)      264 2023-04-28 16:38:04.000000 scorpionsql-0.0.5/scorpionsql.egg-info/PKG-INFO
--rw-r--r--   0 eugenewu   (502) staff       (20)      392 2023-04-28 16:38:04.000000 scorpionsql-0.0.5/scorpionsql.egg-info/SOURCES.txt
--rw-r--r--   0 eugenewu   (502) staff       (20)        1 2023-04-28 16:38:04.000000 scorpionsql-0.0.5/scorpionsql.egg-info/dependency_links.txt
--rw-r--r--   0 eugenewu   (502) staff       (20)       43 2023-04-28 16:38:04.000000 scorpionsql-0.0.5/scorpionsql.egg-info/requires.txt
--rw-r--r--   0 eugenewu   (502) staff       (20)       12 2023-04-28 16:38:04.000000 scorpionsql-0.0.5/scorpionsql.egg-info/top_level.txt
--rw-r--r--   0 eugenewu   (502) staff       (20)       79 2023-04-28 16:38:04.623205 scorpionsql-0.0.5/setup.cfg
--rwxr-xr-x   0 eugenewu   (502) staff       (20)      857 2023-04-28 16:33:46.000000 scorpionsql-0.0.5/setup.py
+drwxr-xr-x   0 eugenewu   (502) staff       (20)        0 2023-04-28 16:58:06.485858 scorpionsql-0.0.6/
+-rw-r--r--   0 eugenewu   (502) staff       (20)     1054 2023-04-28 16:31:36.000000 scorpionsql-0.0.6/LICENSE
+-rw-r--r--   0 eugenewu   (502) staff       (20)      264 2023-04-28 16:58:06.485922 scorpionsql-0.0.6/PKG-INFO
+-rw-r--r--   0 eugenewu   (502) staff       (20)      132 2023-04-28 16:31:36.000000 scorpionsql-0.0.6/README.md
+drwxr-xr-x   0 eugenewu   (502) staff       (20)        0 2023-04-28 16:58:06.485051 scorpionsql-0.0.6/scorpionsql/
+-rw-r--r--   0 eugenewu   (502) staff       (20)       22 2023-04-28 16:57:55.000000 scorpionsql-0.0.6/scorpionsql/__init__.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)     1797 2023-04-28 16:31:36.000000 scorpionsql-0.0.6/scorpionsql/aggerror.py
+-rwxr-xr-x   0 eugenewu   (502) staff       (20)     2430 2023-04-28 16:56:02.000000 scorpionsql-0.0.6/scorpionsql/db.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)    10597 2023-04-28 16:56:19.000000 scorpionsql-0.0.6/scorpionsql/errfunc.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)     8682 2023-04-28 16:57:43.000000 scorpionsql-0.0.6/scorpionsql/functions.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)       36 2023-04-28 16:31:36.000000 scorpionsql-0.0.6/scorpionsql/settings.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)     8183 2023-04-28 16:57:27.000000 scorpionsql-0.0.6/scorpionsql/sql.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)     5087 2023-04-28 16:56:59.000000 scorpionsql-0.0.6/scorpionsql/sqlparser.py
+drwxr-xr-x   0 eugenewu   (502) staff       (20)        0 2023-04-28 16:58:06.485711 scorpionsql-0.0.6/scorpionsql.egg-info/
+-rw-r--r--   0 eugenewu   (502) staff       (20)      264 2023-04-28 16:58:06.000000 scorpionsql-0.0.6/scorpionsql.egg-info/PKG-INFO
+-rw-r--r--   0 eugenewu   (502) staff       (20)      392 2023-04-28 16:58:06.000000 scorpionsql-0.0.6/scorpionsql.egg-info/SOURCES.txt
+-rw-r--r--   0 eugenewu   (502) staff       (20)        1 2023-04-28 16:58:06.000000 scorpionsql-0.0.6/scorpionsql.egg-info/dependency_links.txt
+-rw-r--r--   0 eugenewu   (502) staff       (20)       43 2023-04-28 16:58:06.000000 scorpionsql-0.0.6/scorpionsql.egg-info/requires.txt
+-rw-r--r--   0 eugenewu   (502) staff       (20)       12 2023-04-28 16:58:06.000000 scorpionsql-0.0.6/scorpionsql.egg-info/top_level.txt
+-rw-r--r--   0 eugenewu   (502) staff       (20)       79 2023-04-28 16:58:06.486187 scorpionsql-0.0.6/setup.cfg
+-rwxr-xr-x   0 eugenewu   (502) staff       (20)      857 2023-04-28 16:33:46.000000 scorpionsql-0.0.6/setup.py
```

### Comparing `scorpionsql-0.0.5/LICENSE` & `scorpionsql-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scorpionsql-0.0.5/scorpionsql/aggerror.py` & `scorpionsql-0.0.6/scorpionsql/aggerror.py`

 * *Files identical despite different names*

### Comparing `scorpionsql-0.0.5/scorpionsql/db.py` & `scorpionsql-0.0.6/scorpionsql/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,28 +36,28 @@
         res = db.execute(queryline, params)
       else:
         res = db.execute(queryline)
     try:
       for row in res.fetchall():
         yield row
     except:
-      print queryline, params
+      print(queryline, params)
       raise
     finally:
       res.close()
 
 def db_type(db, table, col):
   q = """SELECT pg_type.typname FROM pg_attribute, pg_class, pg_type where 
     relname = %%s and pg_class.oid = pg_attribute.attrelid and attname = '%s' and
     pg_type.oid = atttypid"""
   try:
     row = db.execute(q % col, table).fetchone()
     return row[0]
   except Exception as e:
-    print e
+    print(e)
     return None
 
 
 def db_schema(db, table):
   """
   only works for postgres
```

### Comparing `scorpionsql-0.0.5/scorpionsql/errfunc.py` & `scorpionsql-0.0.6/scorpionsql/errfunc.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
   bcs[bcs > 0] = 1
   bcs[bcs <= 0] = smooth
   weights = bcs / bcs.sum()
   try:
     return np.average(binfs, axis=0, weights=weights)
   except:
-    print bcs
-    print weights
-    print bds
+    print(bcs)
+    print(weights)
+    print(bds)
     import traceback
     traceback.print_exc()
     import pdb
     pdb.set_trace()
 
 def compute_influence(l, binf, ginf, nclauses=0, *args):
   return l * binf - (1. - l) * ginf - 0.0001 * nclauses # XXX: add - len(rule.clauses)
@@ -386,11 +386,11 @@
 
 
 
 if __name__ == '__main__':
     ef = AvgErrFunc([DummyVar()])
     s1 = ef.state(range(10))
     s2 = ef.state(range(4))
-    print ef.recover(s1), np.mean(range(10))
-    print ef.recover(s2), np.mean(range(4))
-    print ef.recover(ef.update(s1, s2)), np.mean(range(10) + range(4))
-    print ef.recover(ef.remove(s1, s2)), np.mean(range(4,10))
+    print(ef.recover(s1), np.mean(range(10)))
+    print(ef.recover(s2), np.mean(range(4)))
+    print(ef.recover(ef.update(s1, s2)), np.mean(range(10) + range(4)))
+    print(ef.recover(ef.remove(s1, s2)), np.mean(range(4,10)))
```

### Comparing `scorpionsql-0.0.5/scorpionsql/functions.py` & `scorpionsql-0.0.6/scorpionsql/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,8 +339,8 @@
 
 
 if __name__ == '__main__':
     
     stdf = StdFunc()
     data = range(200)
     stdf(np.array(data))
-    print stdf.delta(rm=np.array(data[100:])), np.std(data[:100])
+    print(stdf.delta(rm=np.array(data[100:])), np.std(data[:100]))
```

### Comparing `scorpionsql-0.0.5/scorpionsql/sql.py` & `scorpionsql-0.0.6/scorpionsql/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     select %s
     from 
       ((select distinct %s from %s %s) as foo
         left outer join  
       bar using (%s)) 
     GROUP BY %s
     ORDER BY %s;""" % (filter_q, select_clause, groupby, fr, orig_where, groupby, groupby, orderby)
-    print sql
+    print(sql)
     return sql
 
     """
     with right as (select * from lqm where WHERECLAUSE)
     select coalesce(sum(total_cost), 0), ccm_payor 
     from 
       ((select distinct ccm_payor from lqm) as payors 
@@ -151,16 +151,16 @@
     
 
 class Select(list):
   def __init__(self, *args):
     try:
       super(Select, self).__init__(*args)
     except Exception as e:
-      print e
-      print args
+      print(e)
+      print(args)
       super(Select, self).__init__(*[args])
 
   def __str__(self):
     return ', '.join(map(str, self))
 
   def coalesced_str(self):
     return ', '.join([s.coalesced_str() for s in self])
@@ -249,23 +249,23 @@
     from pyparsing import *
 
         
 
     exprStack = []
 
     def pushNum(s, loc, toks):
-        print 'num ', toks
+        print('num ', toks)
     def pushVar(s, loc, toks):
-        print 'var ', toks
+        print('var ', toks)
     def pushNest(s, loc, toks):
-        print 'nest ', toks
+        print('nest ', toks)
     def pushFunc(s, loc, toks):
-        print 'func ', toks
+        print('func ', toks)
     def pushArith(s, loc, toks):
-        print 'arith ', toks
+        print('arith ', toks)
 
     def pushFirst( strg, loc, toks ):
         exprStack.append( toks[0] )
     def pushUMinus( strg, loc, toks ):
         if toks and toks[0]=='-': 
             exprStack.append( 'unary -' )
             #~ exprStack.append( '-1' )
```

### Comparing `scorpionsql-0.0.5/scorpionsql/sqlparser.py` & `scorpionsql-0.0.6/scorpionsql/sqlparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,18 +36,18 @@
         queryobj = self.json_to_obj(jsonobj)
         return queryobj
 
     def fetch_json(self, q):
         try:
             cmd = ["java", "-cp", classes, "main", q]
             ret = subprocess.check_output(cmd)
-            print ret
+            print(ret)
             return json.loads(ret)
         except subprocess.CalledProcessError as e:
-            print >>sys.stderr, str(e)
+            print(str(e), file=sys.stderr)
             import traceback
             traceback.print_exc()
             return None
 
 
     def json_to_obj(self, j):
         select = j['select']
@@ -162,23 +162,23 @@
 if __name__ == '__main__':
     from tests.gentestdata import *
     for name in datasetnames:
         test_data = get_test_data(name)
         q = test_data[1]
         parser = SqlParser()
         qobj = parser(q)
-        print qobj
+        print(qobj)
     exit()
     import Orange
     t = Orange.data.Table('iris')
     names = ['slen', 'swid', 'plen', 'pwid', 'iris']
     for d, n in zip(t.domain, names):
         d.name = n
 
     func = qobj.select.aggregates[0].func
     func.setup(t, ErrTypes(ErrTypes.TOOHIGH))
 
     tn = t.to_numpy('a')[0]
     for i in xrange(len(t)):
-        print func(tn[(i,),:], "rm"), tn[i,:]
+        print(func(tn[(i,),:], "rm"), tn[i,:])
```

### Comparing `scorpionsql-0.0.5/setup.py` & `scorpionsql-0.0.6/setup.py`

 * *Files identical despite different names*

