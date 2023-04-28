# Comparing `tmp/ringneck-0.0.2.tar.gz` & `tmp/ringneck-0.0.3.tar.gz`

## Comparing `ringneck-0.0.2.tar` & `ringneck-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 ringneck-0.0.2/Makefile
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ringneck-0.0.2/_version.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 ringneck-0.0.2/requirements-dev.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ringneck-0.0.2/setup.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ringneck-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ringneck-0.0.2/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ringneck-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ringneck-0.0.2/examples/generator.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/error_handler.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/grammar.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/interpreter.py
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/parser.py
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/scanner.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tokens.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/ast/__init__.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/ast/base.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/ast/expression.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/ast/printer.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/ast/statement.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/__init__.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/cases.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/test_embedded.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/test_interpreter.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/test_parser.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 ringneck-0.0.2/src/ringneck/tests/test_scanner.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 ringneck-0.0.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 ringneck-0.0.2/LICENSE
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 ringneck-0.0.2/README.md
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 ringneck-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 ringneck-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 ringneck-0.0.3/Makefile
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ringneck-0.0.3/_version.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 ringneck-0.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ringneck-0.0.3/setup.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ringneck-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ringneck-0.0.3/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ringneck-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ringneck-0.0.3/examples/generator.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/error_handler.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/grammar.md
+-rw-r--r--   0        0        0     9764 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/interpreter.py
+-rw-r--r--   0        0        0    10227 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/parser.py
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/scanner.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/tokens.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/ast/__init__.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/ast/base.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/ast/expression.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/ast/printer.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/ast/statement.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/tests/__init__.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/tests/cases.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/tests/test_embedded.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/tests/test_interpreter.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/tests/test_parser.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 ringneck-0.0.3/src/ringneck/tests/test_scanner.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 ringneck-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 ringneck-0.0.3/LICENSE
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 ringneck-0.0.3/README.md
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 ringneck-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 ringneck-0.0.3/PKG-INFO
```

### Comparing `ringneck-0.0.2/Makefile` & `ringneck-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/.github/workflows/publish.yml` & `ringneck-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/examples/generator.py` & `ringneck-0.0.3/examples/generator.py`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/src/ringneck/error_handler.py` & `ringneck-0.0.3/src/ringneck/error_handler.py`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/src/ringneck/grammar.md` & `ringneck-0.0.3/src/ringneck/grammar.md`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/src/ringneck/interpreter.py` & `ringneck-0.0.3/src/ringneck/interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,41 +72,56 @@
 
             if expr.operator.tokentype == TokenType.GREATER_EQUAL:
                 return expr.left.accept(self) >= expr.right.accept(self)
 
             if expr.operator.tokentype == TokenType.AND:
                 return expr.left.accept(self) and expr.right.accept(self)
 
+            if expr.operator.tokentype == TokenType.OR:
+                return expr.left.accept(self) or expr.right.accept(self)
+
             if expr.operator.tokentype == TokenType.EQUAL_EQUAL:
                 return expr.left.accept(self) == expr.right.accept(self)
 
             if expr.operator.tokentype == TokenType.BANG_EQUAL:
                 return expr.left.accept(self) != expr.right.accept(self)
         except TypeError as exp:
             raise RuntimeError(
-                f"Wrong types in expression at {expr.operator.line}, {expr.operator.column}") from exp
+                f"Wrong types in expression at {expr.operator.line}, {expr.operator.column}: {exp}") from exp
 
         raise RuntimeError(f"Unknown operator '{expr.operator.lexeme}'")
 
-    def visit_Expression_Statement(self, stmt: statement.Expression):
-        return self.evaluate(stmt.expr)
+    def visit_AugmentedAssign_Expression(self, expr: expression.AugmentedAssign):
+        if expr.operator.tokentype == TokenType.MINUS_EQUAL:
+            return self.set(expr.left.name.literal, self.get(
+                expr.left.name.literal) - self.evaluate(expr.right))
+
+        if expr.operator.tokentype == TokenType.PLUS_EQUAL:
+            return self.set(expr.left.name.literal, self.get(
+                expr.left.name.literal) + self.evaluate(expr.right))
+
+        raise RuntimeError(f"Unknown operator '{expr.operator.lexeme}'")
 
     def visit_Tuple_Expression(self, expr: expression.Tuple):
         return tuple([v.accept(self) for v in expr.values])
 
     def visit_Assign_Expression(self, expr: expression.Assign):
         if expr.operator.tokentype == TokenType.MAYBE_EQUAL:
             if self.get(expr.name.literal) is not None:
                 return
         self.set(expr.name.literal, self.evaluate(expr.value))
 
     def visit_MultiAssign_Expression(self, expr: expression.MultiAssign):
         identifiers = [v.name.literal for v in expr.identifiers.values]
-        for identifier, value in zip(identifiers, expr.values.values):
-            self.set(f"{identifier}", self.evaluate(value))
+        if isinstance(expr.values, (expression.Variable, expression.Call)):
+            values = self.evaluate(expr.values)
+        else:
+            values = [self.evaluate(v) for v in expr.values.values]
+        for identifier, value in zip(identifiers, values):
+            self.set(f"{identifier}", value)
 
     def visit_AssignIterator_Expression(self, expr: expression.AssignIterator):
         prefix = expr.iterator.prefix.literal
         iterator = expr.iterator.iterator.accept(self)
 
         for it in iterator:
             self.state['%'] = it
@@ -160,26 +175,33 @@
             output.append(value)
 
         return output
 
     def visit_Call_Expression(self, expr: expression.Call):
         callee = self.evaluate(expr.callee)
 
+        if isinstance(expr.arguments, expression.Starred):
+            in_arguments = self.evaluate(expr.arguments)
+        in_arguments = expr.arguments.expressions
+
         arguments: List[Any] = []
-        for argument in expr.arguments.expressions:
+        for argument in in_arguments:
             arguments.append(self.evaluate(argument))
 
         if hasattr(callee, '__globals__'):
             callee.__globals__['state'] = self.state
             callee.__globals__['globals'] = self.globals
 
         try:
             return callee(*arguments)
-        except (AttributeError, TypeError) as exc:
-            raise RuntimeError(f"Error in expression: {expr}") from exc
+        except AttributeError as error:
+            raise RuntimeError(
+                f"Attribute error in expression: {error}") from error
+        except TypeError as error:
+            raise RuntimeError(f"Type error in expression: {error}") from error
 
     def visit_Conditional_Expression(self, expr: expression.Conditional):
         if expr.condition.accept(self):
             return expr.left.accept(self)
 
         if expr.right is not None:
             return expr.right.accept(self)
@@ -226,7 +248,19 @@
             else:
                 result = getattr(result, part)
 
         if isinstance(result, MutableMapping):
             result[parts[0]] = value
         else:
             setattr(result, parts[0], value)
+
+    def visit_Expression_Statement(self, stmt: statement.Expression):
+        return self.evaluate(stmt.expr)
+
+    def visit_If_Statement(self, stmt: statement.If):
+        if self.evaluate(stmt.condition):
+            res = [self.execute(s) for s in stmt.thenbranch]
+            return res
+
+    def visit_Repeat_Statement(self, stmt: statement.Repeat):
+        for _ in range(self.evaluate(stmt.count)):
+            self.execute(stmt.stmt)
```

### Comparing `ringneck-0.0.2/src/ringneck/parser.py` & `ringneck-0.0.3/src/ringneck/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,24 +48,43 @@
             statements.append(self.statement())
             while self.match(TokenType.EOL):
                 pass
 
         return statements
 
     def statement(self):
+        if self.match(TokenType.IF):
+            return self.if_statement()
+        if self.match(TokenType.REPEAT):
+            return self.repeat_statement()
         return self.expression_statement()
 
     def expression_statement(self):
         expr = self.parse_expression()
 
-        if not self.is_at_end():
-            self.consume(
-                TokenType.EOL, f"Expect newline after expression, got {self.peek().tokentype}")
         return statement.Expression(expr)
 
+    def repeat_statement(self):
+        stmt = self.statement()
+        self.consume(TokenType.TIMES, "Except TIMES after REPEAT statement.")
+        times = self.parse_expression()
+        return statement.Repeat(times, stmt)
+
+    def if_statement(self):
+        condition = self.parse_expression()
+        self.consume(TokenType.COLON, "Expected colon after if statement")
+        self.consume(TokenType.EOL, "Expected a newline")
+        then_branch = []
+        while not self.match(TokenType.ENDIF):
+            then_branch.append(self.statement())
+            while self.match(TokenType.EOL):
+                ...
+        stmt = statement.If(condition, then_branch)
+        return stmt
+
     def expression_list(self):
         expr = self.equality()
         if self.peek().tokentype == TokenType.COMMA:
             expr_list = [expr]
             while self.match(TokenType.COMMA):
                 expr_list.append(self.equality())
 
@@ -81,23 +100,28 @@
         expr = self.expression_list()
 
         if self.match(TokenType.EQUAL, TokenType.MAYBE_EQUAL):
             equals = self.previous()
             value = self.assignment()
 
             if isinstance(expr, (expression.Tuple, expression.List)):
-                assert isinstance(value, expression.Tuple)
-                assert len(expr.values) == len(value.values)
                 return expression.MultiAssign(expr, equals, value)
             if isinstance(expr, expression.Variable):
                 name = expr.name
                 return expression.Assign(name, equals, value)
             if isinstance(expr, expression.VariableIterator):
                 return expression.AssignIterator(expr, equals, value)
             self.error(equals, "Invalid assignment target.")
+        if self.match(TokenType.MINUS_EQUAL, TokenType.PLUS_EQUAL):
+            operator = self.previous()
+            if isinstance(expr, expression.Tuple):
+                self.error(
+                    operator, "'tuple' is illegal for augmented assignment.")
+            value = self.equality()
+            return expression.AugmentedAssign(expr, operator, value)
         return expr
 
     def equality(self):
         expr = self.logical()
 
         if self.peek().tokentype == TokenType.IF:
             self.consume(TokenType.IF, "Expected conditional")
```

### Comparing `ringneck-0.0.2/src/ringneck/scanner.py` & `ringneck-0.0.3/src/ringneck/scanner.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,16 +30,24 @@
             Token(TokenType.EOF, "\0", None, self._line, self._current))
 
         return self.tokens
 
     def scan_token(self):
         char = self.advance()
         if char == '+':
+            if self.peek() == '=':
+                self.advance()
+                return self.add_token(TokenType.PLUS_EQUAL, '+=')
             return self.add_token(TokenType.PLUS, '+')
+
         if char == '-':
+            if self.peek() == '=':
+                self.advance()
+                return self.add_token(TokenType.MINUS_EQUAL, '-=')
+
             return self.add_token(TokenType.MINUS, '-')
         if char == '*':
             return self.add_token(TokenType.STAR, '*')
         if char == '/':
             return self.add_token(TokenType.SLASH, '/')
 
         if char == '%':
```

### Comparing `ringneck-0.0.2/src/ringneck/tokens.py` & `ringneck-0.0.3/src/ringneck/tokens.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
     MINUS = '-'
     SLASH = '/'
     STAR = '*'
 
     EQUAL = '='
     MAYBE_EQUAL = '?='
 
+    PLUS_EQUAL = '+='
+    MINUS_EQUAL = '-='
+
     DOLLAR = '$'
     DOT = '.'
     COLON = ':'
     COMMA = ','
     HASH = '#'
     PERCENT = '%'
 
@@ -46,26 +49,33 @@
 
     EOL = 'EOL'
     EOF = 'EOF'
 
     # Keywords
     IF = 'if'
     ELSE = 'else'
+    ENDIF = 'endif'
+
+    REPEAT = 'repeat'
+    TIMES = 'times'
 
     AND = 'and'
     OR = 'or'
     NOT = 'not'
 
     TRUE = 'True'
     FALSE = 'False'
 
 
 keywords = {
     'if': TokenType.IF,
     'else': TokenType.ELSE,
+    'endif': TokenType.ENDIF,
+    'repeat': TokenType.REPEAT,
+    'times': TokenType.TIMES,
     'and': TokenType.AND,
     'or': TokenType.OR,
     'not': TokenType.NOT,
     'True': TokenType.TRUE,
     'False': TokenType.FALSE
 }
```

### Comparing `ringneck-0.0.2/src/ringneck/ast/base.py` & `ringneck-0.0.3/src/ringneck/ast/base.py`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/src/ringneck/ast/expression.py` & `ringneck-0.0.3/src/ringneck/ast/expression.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 @dataclass
 class Binary(Expression):
     left: Expression
     operator: Token
     right: Expression
 
+    def __str__(self):
+        return f"Binary({self.left} {self.operator.literal} {self.right}"
+
 
 @dataclass
 class Grouping(Expression):
     expression: Expression
 
 
 @dataclass
@@ -43,14 +46,17 @@
     right: Expression
 
 
 @dataclass
 class Variable(Expression):
     name: Token
 
+    def __str__(self):
+        return f"Variable({self.name.literal})"
+
 
 @dataclass
 class VariableIterator(Expression):
     prefix: Expression
     iterator: 'List'
 
 
@@ -61,15 +67,15 @@
     value: Any
 
 
 @dataclass
 class MultiAssign(Expression):
     identifiers: Union['Tuple', 'List']
     operator: Token
-    values: Union['Tuple', 'List']
+    values: Expression
 
 
 @dataclass
 class AssignIterator(Expression):
     iterator: VariableIterator
     operator: Token
     value: Any
@@ -102,20 +108,27 @@
     values: TList[Expression] | ExpressionList | Starred
 
 
 @dataclass
 class Call(Expression):
     callee: Expression
     paren: Token
-    arguments: Optional[ExpressionList]
+    arguments: Optional[ExpressionList | Starred]
 
 
 @dataclass
 class Conditional(Expression):
     left: Expression
     condition: Expression
     right: Expression
 
 
 @dataclass
 class IteratorValue(Expression):
     token: Token
+
+
+@dataclass
+class AugmentedAssign(Expression):
+    left: Variable
+    operator: Token
+    right: Expression
```

### Comparing `ringneck-0.0.2/src/ringneck/ast/printer.py` & `ringneck-0.0.3/src/ringneck/ast/printer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, List
 from ringneck.ast.base import VisitorType, Visitor
 
-from ringneck.ast.expression import Binary, Expression, Grouping, Literal
+from ringneck.ast.expression import AugmentedAssign, Binary, Expression, Grouping, Literal
 from ringneck.ast import statement, expression
 
 
 class ASTPrinter(Visitor[VisitorType]):
     def print(self, program: List[Any]):
         output: List[str] = []
         for step in program:
@@ -28,16 +28,16 @@
 
     def visit_Grouping_Expression(self, grouping: Grouping):
         return self.parenthesize("grouping", grouping.expression)
 
     def visit_Binary_Expression(self, expr: Binary):
         return self.parenthesize(expr.operator.lexeme, expr.left, expr.right)
 
-    def visit_Expression_Statement(self, stmt: statement.Expression):
-        return str(stmt.expr.accept(self))
+    def visit_AugmentedAssign_Expression(self, expr: AugmentedAssign):
+        return self.parenthesize(expr.operator.lexeme, expr.left, expr.right)
 
     def visit_Assign_Expression(self, expr: expression.Assign):
         return self.parenthesize(f'assign {expr.name.literal}', expr.value)
 
     def visit_AssignIterator_Expression(self, expr: expression.AssignIterator):
         return self.parenthesize(f'assign {expr.iterator.accept(self)}', expr.value)
 
@@ -75,7 +75,16 @@
         return f"(tuple {', '.join(str(v.accept(self)) for v in expr.values)})"
 
     def visit_ExpressionList_Expression(self, expr: expression.ExpressionList):
         return f"(expressionlist {', '.join(str(v.accept(self)) for v in expr.expressions)})"
 
     def visit_Starred_Expression(self, expr: expression.Starred):
         return self.parenthesize("starred", expr.value)
+
+    def visit_Expression_Statement(self, stmt: statement.Expression):
+        return str(stmt.expr.accept(self))
+
+    def visit_If_Statement(self, stmt: statement.If):
+        return f"(if {stmt.condition.accept(self)} {' '.join([s.accept(self) for s in stmt.thenbranch])})"
+
+    def visit_Repeat_Statement(self, stmt: statement.Repeat):
+        return f"(repeat {stmt.count.accept(self)} {stmt.stmt.accept(self)})"
```

### Comparing `ringneck-0.0.2/src/ringneck/tests/cases.py` & `ringneck-0.0.3/src/ringneck/tests/cases.py`

 * *Files 21% similar despite different names*

```diff
@@ -69,9 +69,31 @@
 b = 2
 """, 8, ["(assign a 1)", "(assign b 2)"]),
     TestCase("a, b = 1, 2", 7, [
              "(assign (tuple a, b) (tuple 1, 2))"], state={'a': 1, 'b': 2}),
     TestCase("a=[*(1, 2, 3)]", 12,
              ["(assign a (starred (tuple 1, 2, 3)))"], state={'a': [1, 2, 3]}),
     TestCase("$.['a', 'b', 'c'] = %", 10, globals={
-             'a': 'a', 'b': 'b', 'c': 'c'})
+             'a': 'a', 'b': 'b', 'c': 'c'}),
+    TestCase("a=(1, 2)\nb, c = a", 13, [
+             "(assign a (tuple 1, 2))", "(assign (tuple b, c) a)"], state={'a': (1, 2), 'b': 1, 'c': 2}),
+    TestCase("a=1\na-=1", 7, ["(assign a 1)",
+             "(-= a 1)"], state={'a': 0}),
+    TestCase("""a=1
+if a > 0:
+b = 2
+endif
+if a > 4:
+a=6
+endif
+if b < 3 and a < 5:
+a=0
+c=3
+endif""", 47,
+             ["(assign a 1)", "(if (> a 0) (assign b 2))", "(if (> a 4) (assign a 6))",
+              "(if (and (< b 3) (< a 5)) (assign a 0) (assign c 3))"],
+             state={'a': 0, 'b': 2, 'c': 3}),
+    TestCase("a=0\nrepeat a += 1 times 5", 10,
+             ["(assign a 0)", "(repeat 5 (+= a 1))"], state={'a': 5}),
+    TestCase("a=foo(*bar.baz)", 7, ["(assign a (call foo (starred bar.baz)))"])
+
 ]
```

### Comparing `ringneck-0.0.2/src/ringneck/tests/test_embedded.py` & `ringneck-0.0.3/src/ringneck/tests/test_embedded.py`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/src/ringneck/tests/test_interpreter.py` & `ringneck-0.0.3/src/ringneck/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/src/ringneck/tests/test_parser.py` & `ringneck-0.0.3/src/ringneck/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/LICENSE` & `ringneck-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/pyproject.toml` & `ringneck-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ringneck-0.0.2/PKG-INFO` & `ringneck-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ringneck
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python-ish script interpreter.
 Project-URL: Homepage, https://github.com/gregersn/ringneck
 Author-email: Greger Stolt Nilsen <gregersn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Greger Stolt Nilsen
```

