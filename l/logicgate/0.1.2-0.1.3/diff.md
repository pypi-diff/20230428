# Comparing `tmp/LogicGate-0.1.2.tar.gz` & `tmp/LogicGate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogicGate-0.1.2.tar", max compression
+gzip compressed data, was "LogicGate-0.1.3.tar", max compression
```

## Comparing `LogicGate-0.1.2.tar` & `LogicGate-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-04-15 10:25:03.782472 LogicGate-0.1.2/LICENSE
--rw-r--r--   0        0        0    10796 2023-04-15 16:56:51.145760 LogicGate-0.1.2/LogicGate/LogicGate.py
--rw-r--r--   0        0        0     4544 2023-04-15 10:25:03.782472 LogicGate-0.1.2/README.rst
--rw-r--r--   0        0        0      721 2023-04-15 16:57:11.303809 LogicGate-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5407 2023-04-15 17:03:37.383071 LogicGate-0.1.2/setup.py
--rw-r--r--   0        0        0     5271 2023-04-15 17:03:37.386968 LogicGate-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 10:25:03.782472 LogicGate-0.1.3/LICENSE
+-rw-r--r--   0        0        0    12628 2023-04-28 07:31:10.362775 LogicGate-0.1.3/LogicGate/LogicGate.py
+-rw-r--r--   0        0        0     4209 2023-04-28 07:41:48.636486 LogicGate-0.1.3/LogicGate/lgEncrypt.py
+-rw-r--r--   0        0        0     4498 2023-04-28 05:57:31.398096 LogicGate-0.1.3/README.rst
+-rw-r--r--   0        0        0      773 2023-04-16 15:35:06.995260 LogicGate-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5377 2023-04-28 07:44:03.164981 LogicGate-0.1.3/setup.py
+-rw-r--r--   0        0        0     5225 2023-04-28 07:44:03.165618 LogicGate-0.1.3/PKG-INFO
```

### Comparing `LogicGate-0.1.2/LICENSE` & `LogicGate-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LogicGate-0.1.2/LogicGate/LogicGate.py` & `LogicGate-0.1.3/LogicGate/LogicGate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 from os.path import exists
 from sys import argv
-import sys
+import sys, os
 from random import randint
+from math import sqrt
 
 
 def run(
   filename: str,
   gate: bool = False,  #show gate in result
   ascii: bool = True,  #show ascii in result
   debug: bool = False,  #log during process
-  check: str = ''  #check for error in code, mostly for debug
+  check: str = '',  #check for error in code, mostly for debug
+  out: bool = True
 ) -> int:  #returns exit code for some reason lol
-  """To run this filename is the only thing needed, Error code will be returned. if everything works fine, output will be printed. and 0 will be returned.
+  """To run this filename is the only thing needed, Error will be raised and nothing will return if something went wrong. If ascii is on, it will return the ascii result, otherwise 0.
   
   Arguments, type of input, usecases:
       filename: string, specify which file needed to run
       gate: boolean(True or False), if the result shows gate result or not
       ascii: boolean, if the result converts to ascii and show or not
       debug: boolean, show the unhuman log during the interpute
       check: string, if it is specified then the result will be colored. It compares the difference between the gate result and the binary of check input, only works if both gate and ascii is True 
              (color: green=correct bit
                      red=incorrect bit
                      blue box=missing bit 1
                      purple box=missing bit 0)
+      out: boolean, enable for outputs
                      """
 
   def process(
     obj,  #first command
     line: tuple = (
       0, 0
     ),  #for error reporting, first is line and second is index, sometimes third for the latest gate called
     aft=None,  #command afterward
     an=None,  #None/True/False -> (1/0/Not)/And/Or
   ) -> tuple:  #(0 or 1, unprocessed commands that may be used by and/or gates in previous commands in list)
     'One line code processor, return one output from a line of input, internal use only'
     if debug: print('called, args:', obj, line, aft, an)
     if len(str(obj)) == 1:  #if the first process string is a single command
       obj = str(obj)
+      if obj == "#":
+        if aft[:2] == '##':
+          return
       AnList = None
       if an != None:
         #if AnList exists, it is an and/or gate, depends on the first index is True(and) or False(or)
         AnList = [an]
         if debug: print('AnList init:', AnList)
       if obj == '1':
         if debug: print('1:', aft)
@@ -91,160 +97,190 @@
           AnList.append(
             process(
               AnList[1][1][0],
               line=(line[0], line[1] + 1, 'A' if AnList[0] else 'O'),
               aft=None if len(str(AnList[1][1])) == 1 else AnList[1][1][1:]))
         except IndexError:
           sys.tracebacklimit = 0
+          sys.stdout = sys.__stdout__
           raise SyntaxError(
             f'gate {line[2] if obj=="0" or obj=="1" else obj} in line {line[0]} index {line[1]-1} requires {"1" if (line[2] if obj=="0" or obj=="1" else obj)=="N" else "2"} inputs, 1 received'
           )
         if len(AnList) == 3:
           if AnList[0]:
             return (AnList[1][0] and AnList[2][0], AnList[2][1])
           else:
             return (AnList[1][0] or AnList[2][0], AnList[2][1])
       else:
         #and/or gate syntax error
         sys.tracebacklimit = 0
+        sys.stdout = sys.__stdout__
         raise SyntaxError(
           f'gate {line[2] if obj=="0" or obj=="1" else obj} in line {line[0]} index {line[1]} requires {"1" if (line[2] if obj=="0" or obj=="1" else obj).upper()=="N" else "2"} inputs, 0 received'
         )
     else:
       #if the first command given is not one command
+      sys.stdout = sys.__stdout__
       raise SystemError(
         'Internal error, unexpected arguments received in internal helper function, please do not change the code'
       )
 
+  
+  if out:
+    sys.stdout = sys.__stdout__
+  else:
+    sys.stdout = open(os.devnull, 'w')
   if exists(filename):
     with open(filename, 'r') as f:
+      f.seek(0,0)
       Out = [[]]
       dt = f.readlines()
       if filename[-6:] != '.lgeso':
-        print(
-          f'{filename} is not an lgeso file, maybe renaming the file extension to lgeso and try again'
-        )
-        return 1
+        sys.tracebacklimit = 0
+        sys.stdout = sys.__stdout__
+        raise NameError(
+          f'{filename} is not an lgeso file, maybe renaming the file extension to lgeso and try again')
       for dtidx, line in enumerate(dt):
         line = line.replace('\n', '')
         if '---' in line:
           Out.append([])
-        elif '###' in line:
-          continue
         else:
-          Out[-1].append(
+          try:
+            Out[-1].append(
             str(
               process(line[0],
                       line=(dtidx + 1, 1),
                       aft=(None if len(line) == 1 else line[1:]))[0]))
+          except OverflowError:
+            sys.tracebacklimit = 0
+            sys.stdout = sys.__stdout__
+            raise OverflowError(f'too many commands in line {dtidx+1}, more than max command on this os ({sys.getrecursionlimit()} commands per line), process overflowed, exited')
       hold = ""
+      checkOut = ""
       checkhold = []
       if check:
         for char in check:
           checkhold.append(str(bin(ord(char))[2:]))
       if gate:
         print('gates result:')
       for nidx, n in enumerate(Out):
+        checkOut+='-'
         Nhold = n.copy()
         if n == []:
           continue
         if gate:
           for chekidx, chek in enumerate(n):
             if '\033[0;37;41m' in chek and '\033[0;37;40m' in chek:
               continue
             if chek != '1' and chek != '0' and chek != ' ':
               print(
                 f'error char {repr(chek)} found in index {chekidx}, line {nidx+1}, please report that line of code shown in lgeso file to the dev. '
               )
             if ascii and check:
               if nidx >= len(checkhold):
                 n[chekidx] = f'\033[0;37;41m{chek}\033[0;37;40m'
+                checkOut+=chek
               else:
                 if len(n) > len(checkhold[nidx]):
                   for _ in range(len(n)-len(checkhold[nidx])):
                     checkhold[nidx] = '0' + checkhold[nidx]
                 if chek != checkhold[nidx][chekidx]:
                   n[chekidx] = f'\033[0;37;41m{chek}\033[0;37;40m'
+                  checkOut+=chek
                 else:
                   n[chekidx] = f'\033[0;37;42m{chek}\033[0;37;40m'
           if nidx < len(checkhold):
             if len(n) < len(checkhold[nidx]):
               for x in checkhold[nidx][len(n):]:
                 n.append(f'\033[0;37;{"46" if int(x) else "45"}m▯\033[0;37;40m')
+                checkOut+='0' if int(x) else '1'
           n.append(' ')
           print(''.join(n))
         if ascii:
           try:
             hold += chr(int(''.join(Nhold), 2))
           except ValueError:
             print(
               f'unacceptable ascii result received, ascii code: {"".join(Nhold), 2}'
             )
       if ascii:
         print("\nAscii converted result:\n" + hold)
         if gate and check:
           print('\nExpected result:\n' + check)
-      return 0
+      sys.stdout = sys.__stdout__
+      return checkOut if (check and gate and ascii) else hold if ascii else 0
   else:
-    print(
+    sys.tracebacklimit = 0
+    sys.stdout = sys.__stdout__
+    raise FileNotFoundError(
       f'{filename} is not an existing file from given path, prehaps try moving the file to the same directory as this program?'
     )
-    return 1
 
 
 def compile(
   filename: str = 'main.lgeso',
   output: str = 'Hello World!',
   randomize: bool = True,
   random_range: list = [1, 5],
-  pure_random: list = []
+  write:bool = True,
+  override:bool = False,
+  BitLock:int = -1
 ) -> None:  #I swear if this thing returns anything somehow somewhere and somewhat, python is dying or my brain is dying
   """compile string to lgeso file, random_range is needed only when randomize is true.
   filename: string, specify which file to write the data into, new file named as filename will be created if it doesn't exist
   output: string, specify what result will be produced
   randomize: boolean, if the data written is pure binary or further encrypted with gates
   random_range: list, the maximum set of gates in the written data will be the square of the second item while the minimum will be the square of the first item.
-  pure_random: boolean, if the """
+  write: boolean, if the result is returned or is written to file
+  override: boolean, safety checks are off, proceed with caution
+  BitLock: integer, if the binary of a character is shorter than this value, 0 will be appended. Defalt is -1, which is off, all negative number will be counted as ignore as well"""
 
-  if not output:
+  out = ""
+  override = not override
+  if not output and override:
     output = 'Hello World!'
-  if filename:
+  if filename and write and override:
     if len(filename) > 6:
       if filename[-6:] != '.lgeso':
         print(f'filename is not an lgeso file, filename changed to {filename}')
         filename += '.lgeso'
     elif '.' in filename:
       print(f'filename is not an lgeso file, filename changed to {filename}')
       filename += '.lgeso'
     else:
       print(f'filename is not an lgeso file, filename changed to {filename}')
       filename = 'main.lgeso'
   else:
-    print(f'filename is not an lgeso file, filename changed to {filename}')
-    filename = 'main.lgeso'
+    if override:
+      print(f'filename is not an lgeso file, filename changed to {filename}')
+      filename = 'main.lgeso'
   with open(filename, 'w') as f:
-    if len(random_range) != 2 or random_range[0] > random_range[1]:
+    if (len(random_range) != 2 or random_range[0] > random_range[1]) and override:
       print('invalid random range received, changed to 1-5')
       random_range = [1, 5]  #when the random_range is not correctly formatted
     for checkidx, check in enumerate(random_range):
       try:
         random_range[checkidx] == int(check)  #if the input is a number or not
       except ValueError:
-        print('invalid random range received, changed to 1-5')
-        random_range = [1, 5]
-        break
+        if override:
+          print('invalid random range received, changed to 1-5')
+          random_range = [1, 5]
+          break
       else:
-        if check < 1 or check > 1000:  #avoid too many looping
+        if (check < 1 or check > (sqrt(sys.getrecursionlimit())//3)) and override:  #avoid overflow error when running
           print(
             'an item in random range is too large or too small, changed to 1-5'
           )
           random_range = [1, 5]
           break
     for char in output:
       line = str(bin(ord(char))[2:])
+      if len(line) < BitLock and BitLock >= 0:
+        for _ in range(BitLock-len(line)):
+          line = '0'+line
       for char in line:
         if randomize:
           charGoal = int(char)  #the ideal final output after the randomizing
           for _ in range(
               randint(random_range[0], random_range[1]) *
               randint(random_range[0], random_range[1])):
             gates = randint(0, 3)
@@ -253,16 +289,23 @@
                       ('NN' + char))
             elif gates == 2:
               buff = ('1' if randint(0, 1) else '0') if charGoal else '0'
               char = 'O' + (char + buff if randint(0, 1) else buff + char)
             elif gates == 3:
               buff = '1' if charGoal else ('1' if randint(0, 1) else '0')
               char = 'A' + (char + buff if randint(0, 1) else buff + char)
-        f.write(char + '\n')
-      f.write('---\n')
+        if write:
+          f.write(char + '\n')
+        else:
+          out += char
+      if write:
+        f.write('---\n')
+      else:
+        out += "-"
     print(
-      f'compilation completed and result written in {filename} with output as {output}.\nrandomizaion is {"on" if randomize else "off"}\n\n\n'
+      f'compilation completed and result {"written in" if write else "returned"} {filename if write else ""} with output as {output}\nrandomizaion is {"on" if randomize else "off"}\n\n\n'
     )
+    return None if write else out
 
 
 if __name__ == '__main__':
   exit(run((str(argv[1]) if len(argv) != 1 else 'main.lgeso')))
```

### Comparing `LogicGate-0.1.2/README.rst` & `LogicGate-0.1.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 All you can do in this language is to make a program with logic gates,
 sounds difficult and indeed it is.
 
 Startup
 -------
 
 First, make a logic gate file. The file extension should be lgeso also
-you will need the runner
 
 Runner
 ------
 
 To use it, import the python file **LogicGate.py** in your python
 script, or just run the LogicGate.py Remember for the run function, only
 the filename argument is needed. The run function will return an exit
@@ -54,15 +53,15 @@
 ~~~~~~~~~~~~~~
 
 There are 2 special syntax
 
 —-- (three hyphens): new word, used for the ascii output separating the
 binary for ascii translation
 
-### (three hashes): comment the entire line
+### (three hashes): comment everything after the syntax
 
 For any of the special syntax, they are not being interpreted as special
 syntax unless the entire syntax appears. They can be anywhere in a line,
 and that line will act like what the syntax shows (if the special syntax
 appears in the same line, they will be scanned and processed according
 to here)
 
@@ -74,12 +73,16 @@
 ``1\n 0\n 0\n 1\n 0\n 0\n 0\n ---\n 1\n 1\n 0\n 0\n 1\n 0\n 1\n ---\n 1\n 1\n 0\n 1\n 1\n 0\n 0\n ---\n 1\n 1\n 0\n 1\n 1\n 0\n 0\n ---\n 1\n 1\n 0\n 1\n 1\n 1\n 1\n ---\n 1\n 0\n 0\n 0\n 0\n 0\n ---\n 1\n 0\n 1\n 0\n 1\n 1\n 1\n ---\n 1\n 1\n 0\n 1\n 1\n 1\n 1\n ---\n 1\n 1\n 1\n 0\n 0\n 1\n 0\n ---\n 1\n 1\n 0\n 1\n 1\n 0\n 0\n ---\n 1\n 1\n 0\n 0\n 1\n 0\n 0\n ---\n 1\n 0\n 0\n 0\n 0\n 1\n``
 
 another version generated by LogicGate.compile():
 ``O1NNAANNNNA1AA1AO0AA1AO1NNANNAA1A1111111111\n NNANNAAAO0O000001\n OO0NNN10\n O1O1NNA1O01\n NNOONNA0O0000\n 0\n AA0NNANNOONNNNAO0A1O0000001\n ---\n OO1O1OAO1NNAO111111\n NNNNO0NNAA1O0N01\n OANNOA0O00000\n ANNNNA001\n NNA11\n NNANNA1ANNO0001\n NNAANNAOOA1NNAO10110111\n ---\n OA111\n A1OA1OO0A1O1NNA1O0ONNNNNNN0000\n A1O0A00\n A1O0NNAO0O0A111\n NNAO1NNONNNNA1O1111\n O0A1OANNA0NNOO0ON10000\n 0\n ---\n O0NNN0\n A1ANNNNNNNNNNO101\n O00\n NNA1OO1ONNAO10110\n OAA1110\n OO0AAO0AAONNO0O0NNO00001100\n NNO0A0ONNN10\n ---\n O0O1O0A1NNO1ANNO0AA1O1AA1A1A11111\n NNANNO1ONNNNNNNNNNO0AO11101\n O0OONNNNAAO0N11000\n A1O0N0\n OONNNNOA1ONNOO0AA11100100\n NNO0ON00\n O0OA1NNA1O100\n ---\n O0OO1OO1A1O1000\n NNOO0AONNONNO0A0NNA0NNA010010\n NNAA0OOOA0O000001\n A0NNNNN1\n AO0NNNNA1OO0001\n O0OA1O0O0OO0OA1O00000\n ---\n 1\n A0NNAO0A0OA0NNA1A0000\n NNO0NNA1NNOO011\n NNO0NNA0A0A0NNOO000\n ANNA1AA1NNNNNNNNAA1NNAA1A111111\n NNA1ANNA1OAO1O11111\n A1A1NNA1O1NNANNA1AA1111\n ---\n ONNNNAOO11110\n OANNOONNA1AA1110111\n AA0NNNNNNO0O0A0O0N10\n NNNNNNOA110\n O1OONNA1101\n A1NNNNA11\n ANNOONNAAO1A1ANNA11111011\n ---\n O0NNO0AO0A111\n NNNNNNA1O0ONNA1NNNNO0NNANNOOA1ANNNNAA11110111\n NNO11\n AO0AN101\n OAA1000\n 1\n O0A0NNO0O0NNA0A0NNA1ON10\n ---\n O0N0\n NNNNNNO0ONNA1N00\n O00\n O0AN01\n NNONNNNNNNNA111\n NNNNONNOO0000\n AONNO0ANNO00101\n ---\n O1ONNANNNNA1111\n NNNNOOOO0NNAA1NNONNO1011111\n NNA0A0A01\n AA1N10\n O1OANNNNNNA1ONNNNOO1AOOO1AAN0110111110\n 0\n OOAO0NNO0A0OAANNA0AONNO0001100000\n ---\n A1A1NNO0NNA11\n OA100\n NNANNOA1001\n 0\n NNO0OA0O000\n ANNO0OONNA1O11001\n ---``
 
 Sources
 -------
-
-Current source code(working in progress): `gitbub
-link <https://github.com/TaokyleYT/LogicGate/>`__\  Esolang wiki:
-`LogicGate <https://esolangs.org/wiki/LogicGate>`__\Replit up-to-date version:
+<br>
+`gitbub
+<https://github.com/TaokyleYT/LogicGate/>`__\
+<br>
+Esolang wiki:
+`LogicGate <https://esolangs.org/wiki/LogicGate>`__\
+<br>
+Replit up-to-date version:
 `replit <https://replit.com/@s3D27ZHOU/LogicGate>`__
```

### Comparing `LogicGate-0.1.2/pyproject.toml` & `LogicGate-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "LogicGate"
-version = "0.1.2"
+version = "0.1.3"
 description = "an esolang designed for manual encryption with logic gates"
 license = "MIT"
 authors = ["Taokyle <taokyle415@gmail.com>"]
 readme = "README.rst"
 repository = "https://replit.com/@s3D27ZHOU/LogicGate"
 packages = [
     { include = "LogicGate.py", from = "LogicGate" },
+    { include = "lgEncrypt.py", from = "LogicGate"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
```

### Comparing `LogicGate-0.1.2/setup.py` & `LogicGate-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'LogicGate'}
 
 modules = \
-['LogicGate']
+['LogicGate', 'lgEncrypt']
 setup_kwargs = {
     'name': 'logicgate',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'an esolang designed for manual encryption with logic gates',
-    'long_description': 'LogicGate\n=========\n\nThis language is inspired by logic gates, by using simple alphabet you\ncould make a program.\n\nIt is designed as a way for manual encryption, which kinda failed\n\nAll you can do in this language is to make a program with logic gates,\nsounds difficult and indeed it is.\n\nStartup\n-------\n\nFirst, make a logic gate file. The file extension should be lgeso also\nyou will need the runner\n\nRunner\n------\n\nTo use it, import the python file **LogicGate.py** in your python\nscript, or just run the LogicGate.py Remember for the run function, only\nthe filename argument is needed. The run function will return an exit\ncode if you use the run function, and outputs of the file will be\nprinted(binary to ascii, and logical binary if enabled) The compile\nfunction does the otherwise, it doesn’t return anything but it can write\ncode into lgeso file.\n\nsyntax\n------\n\nFor syntax it is very straight forward. It process each character in\neach line as each command For gates with multiple inputs (such as or,\nand) type like other syntax, the quota for the gate will automatically\nbe processed. No linking between words, unless the syntax at the middle\nis invalid\n\nBasic gates(gates that doesn’t require includes):\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nA (and gate): the next **2** results will be accepted as inputs. If both\ninputs are 1, output is 1, else 0\n\nO (or gate): the next **2** results will be accepted as inputs. If one\nof the inputs are 1, output is 1, else 0\n\nN (not gate): the next **1** result will be accepted as inputs. If the\ninput is 1, output is 0, else 0\n\n1 and 0 (True and False): **NO** result will be accepted as inputs. They\nare the results, self explanatory\n\nspecial syntax\n~~~~~~~~~~~~~~\n\nThere are 2 special syntax\n\n—-- (three hyphens): new word, used for the ascii output separating the\nbinary for ascii translation\n\n### (three hashes): comment the entire line\n\nFor any of the special syntax, they are not being interpreted as special\nsyntax unless the entire syntax appears. They can be anywhere in a line,\nand that line will act like what the syntax shows (if the special syntax\nappears in the same line, they will be scanned and processed according\nto here)\n\nexamples\n========\n\nThis is a hello world in LogicGate\n\n``1\\n 0\\n 0\\n 1\\n 0\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 0\\n ---\\n 1\\n 0\\n 1\\n 0\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 0\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 1\\n``\n\nanother version generated by LogicGate.compile():\n``O1NNAANNNNA1AA1AO0AA1AO1NNANNAA1A1111111111\\n NNANNAAAO0O000001\\n OO0NNN10\\n O1O1NNA1O01\\n NNOONNA0O0000\\n 0\\n AA0NNANNOONNNNAO0A1O0000001\\n ---\\n OO1O1OAO1NNAO111111\\n NNNNO0NNAA1O0N01\\n OANNOA0O00000\\n ANNNNA001\\n NNA11\\n NNANNA1ANNO0001\\n NNAANNAOOA1NNAO10110111\\n ---\\n OA111\\n A1OA1OO0A1O1NNA1O0ONNNNNNN0000\\n A1O0A00\\n A1O0NNAO0O0A111\\n NNAO1NNONNNNA1O1111\\n O0A1OANNA0NNOO0ON10000\\n 0\\n ---\\n O0NNN0\\n A1ANNNNNNNNNNO101\\n O00\\n NNA1OO1ONNAO10110\\n OAA1110\\n OO0AAO0AAONNO0O0NNO00001100\\n NNO0A0ONNN10\\n ---\\n O0O1O0A1NNO1ANNO0AA1O1AA1A1A11111\\n NNANNO1ONNNNNNNNNNO0AO11101\\n O0OONNNNAAO0N11000\\n A1O0N0\\n OONNNNOA1ONNOO0AA11100100\\n NNO0ON00\\n O0OA1NNA1O100\\n ---\\n O0OO1OO1A1O1000\\n NNOO0AONNONNO0A0NNA0NNA010010\\n NNAA0OOOA0O000001\\n A0NNNNN1\\n AO0NNNNA1OO0001\\n O0OA1O0O0OO0OA1O00000\\n ---\\n 1\\n A0NNAO0A0OA0NNA1A0000\\n NNO0NNA1NNOO011\\n NNO0NNA0A0A0NNOO000\\n ANNA1AA1NNNNNNNNAA1NNAA1A111111\\n NNA1ANNA1OAO1O11111\\n A1A1NNA1O1NNANNA1AA1111\\n ---\\n ONNNNAOO11110\\n OANNOONNA1AA1110111\\n AA0NNNNNNO0O0A0O0N10\\n NNNNNNOA110\\n O1OONNA1101\\n A1NNNNA11\\n ANNOONNAAO1A1ANNA11111011\\n ---\\n O0NNO0AO0A111\\n NNNNNNA1O0ONNA1NNNNO0NNANNOOA1ANNNNAA11110111\\n NNO11\\n AO0AN101\\n OAA1000\\n 1\\n O0A0NNO0O0NNA0A0NNA1ON10\\n ---\\n O0N0\\n NNNNNNO0ONNA1N00\\n O00\\n O0AN01\\n NNONNNNNNNNA111\\n NNNNONNOO0000\\n AONNO0ANNO00101\\n ---\\n O1ONNANNNNA1111\\n NNNNOOOO0NNAA1NNONNO1011111\\n NNA0A0A01\\n AA1N10\\n O1OANNNNNNA1ONNNNOO1AOOO1AAN0110111110\\n 0\\n OOAO0NNO0A0OAANNA0AONNO0001100000\\n ---\\n A1A1NNO0NNA11\\n OA100\\n NNANNOA1001\\n 0\\n NNO0OA0O000\\n ANNO0OONNA1O11001\\n ---``\n\nSources\n-------\n\nCurrent source code(working in progress): `gitbub\nlink <https://github.com/TaokyleYT/LogicGate/>`__\\  Esolang wiki:\n`LogicGate <https://esolangs.org/wiki/LogicGate>`__\\Replit up-to-date version:\n`replit <https://replit.com/@s3D27ZHOU/LogicGate>`__\n',
+    'long_description': 'LogicGate\n=========\n\nThis language is inspired by logic gates, by using simple alphabet you\ncould make a program.\n\nIt is designed as a way for manual encryption, which kinda failed\n\nAll you can do in this language is to make a program with logic gates,\nsounds difficult and indeed it is.\n\nStartup\n-------\n\nFirst, make a logic gate file. The file extension should be lgeso also\n\nRunner\n------\n\nTo use it, import the python file **LogicGate.py** in your python\nscript, or just run the LogicGate.py Remember for the run function, only\nthe filename argument is needed. The run function will return an exit\ncode if you use the run function, and outputs of the file will be\nprinted(binary to ascii, and logical binary if enabled) The compile\nfunction does the otherwise, it doesn’t return anything but it can write\ncode into lgeso file.\n\nsyntax\n------\n\nFor syntax it is very straight forward. It process each character in\neach line as each command For gates with multiple inputs (such as or,\nand) type like other syntax, the quota for the gate will automatically\nbe processed. No linking between words, unless the syntax at the middle\nis invalid\n\nBasic gates(gates that doesn’t require includes):\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nA (and gate): the next **2** results will be accepted as inputs. If both\ninputs are 1, output is 1, else 0\n\nO (or gate): the next **2** results will be accepted as inputs. If one\nof the inputs are 1, output is 1, else 0\n\nN (not gate): the next **1** result will be accepted as inputs. If the\ninput is 1, output is 0, else 0\n\n1 and 0 (True and False): **NO** result will be accepted as inputs. They\nare the results, self explanatory\n\nspecial syntax\n~~~~~~~~~~~~~~\n\nThere are 2 special syntax\n\n—-- (three hyphens): new word, used for the ascii output separating the\nbinary for ascii translation\n\n### (three hashes): comment everything after the syntax\n\nFor any of the special syntax, they are not being interpreted as special\nsyntax unless the entire syntax appears. They can be anywhere in a line,\nand that line will act like what the syntax shows (if the special syntax\nappears in the same line, they will be scanned and processed according\nto here)\n\nexamples\n========\n\nThis is a hello world in LogicGate\n\n``1\\n 0\\n 0\\n 1\\n 0\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 0\\n ---\\n 1\\n 0\\n 1\\n 0\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 0\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 1\\n``\n\nanother version generated by LogicGate.compile():\n``O1NNAANNNNA1AA1AO0AA1AO1NNANNAA1A1111111111\\n NNANNAAAO0O000001\\n OO0NNN10\\n O1O1NNA1O01\\n NNOONNA0O0000\\n 0\\n AA0NNANNOONNNNAO0A1O0000001\\n ---\\n OO1O1OAO1NNAO111111\\n NNNNO0NNAA1O0N01\\n OANNOA0O00000\\n ANNNNA001\\n NNA11\\n NNANNA1ANNO0001\\n NNAANNAOOA1NNAO10110111\\n ---\\n OA111\\n A1OA1OO0A1O1NNA1O0ONNNNNNN0000\\n A1O0A00\\n A1O0NNAO0O0A111\\n NNAO1NNONNNNA1O1111\\n O0A1OANNA0NNOO0ON10000\\n 0\\n ---\\n O0NNN0\\n A1ANNNNNNNNNNO101\\n O00\\n NNA1OO1ONNAO10110\\n OAA1110\\n OO0AAO0AAONNO0O0NNO00001100\\n NNO0A0ONNN10\\n ---\\n O0O1O0A1NNO1ANNO0AA1O1AA1A1A11111\\n NNANNO1ONNNNNNNNNNO0AO11101\\n O0OONNNNAAO0N11000\\n A1O0N0\\n OONNNNOA1ONNOO0AA11100100\\n NNO0ON00\\n O0OA1NNA1O100\\n ---\\n O0OO1OO1A1O1000\\n NNOO0AONNONNO0A0NNA0NNA010010\\n NNAA0OOOA0O000001\\n A0NNNNN1\\n AO0NNNNA1OO0001\\n O0OA1O0O0OO0OA1O00000\\n ---\\n 1\\n A0NNAO0A0OA0NNA1A0000\\n NNO0NNA1NNOO011\\n NNO0NNA0A0A0NNOO000\\n ANNA1AA1NNNNNNNNAA1NNAA1A111111\\n NNA1ANNA1OAO1O11111\\n A1A1NNA1O1NNANNA1AA1111\\n ---\\n ONNNNAOO11110\\n OANNOONNA1AA1110111\\n AA0NNNNNNO0O0A0O0N10\\n NNNNNNOA110\\n O1OONNA1101\\n A1NNNNA11\\n ANNOONNAAO1A1ANNA11111011\\n ---\\n O0NNO0AO0A111\\n NNNNNNA1O0ONNA1NNNNO0NNANNOOA1ANNNNAA11110111\\n NNO11\\n AO0AN101\\n OAA1000\\n 1\\n O0A0NNO0O0NNA0A0NNA1ON10\\n ---\\n O0N0\\n NNNNNNO0ONNA1N00\\n O00\\n O0AN01\\n NNONNNNNNNNA111\\n NNNNONNOO0000\\n AONNO0ANNO00101\\n ---\\n O1ONNANNNNA1111\\n NNNNOOOO0NNAA1NNONNO1011111\\n NNA0A0A01\\n AA1N10\\n O1OANNNNNNA1ONNNNOO1AOOO1AAN0110111110\\n 0\\n OOAO0NNO0A0OAANNA0AONNO0001100000\\n ---\\n A1A1NNO0NNA11\\n OA100\\n NNANNOA1001\\n 0\\n NNO0OA0O000\\n ANNO0OONNA1O11001\\n ---``\n\nSources\n-------\n<br>\n`gitbub\n<https://github.com/TaokyleYT/LogicGate/>`__\\\n<br>\nEsolang wiki:\n`LogicGate <https://esolangs.org/wiki/LogicGate>`__\\\n<br>\nReplit up-to-date version:\n`replit <https://replit.com/@s3D27ZHOU/LogicGate>`__\n',
     'author': 'Taokyle',
     'author_email': 'taokyle415@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://replit.com/@s3D27ZHOU/LogicGate',
     'package_dir': package_dir,
     'py_modules': modules,
```

### Comparing `LogicGate-0.1.2/PKG-INFO` & `LogicGate-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logicgate
-Version: 0.1.2
+Version: 0.1.3
 Summary: an esolang designed for manual encryption with logic gates
 Home-page: https://replit.com/@s3D27ZHOU/LogicGate
 License: MIT
 Author: Taokyle
 Author-email: taokyle415@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,14 @@
 All you can do in this language is to make a program with logic gates,
 sounds difficult and indeed it is.
 
 Startup
 -------
 
 First, make a logic gate file. The file extension should be lgeso also
-you will need the runner
 
 Runner
 ------
 
 To use it, import the python file **LogicGate.py** in your python
 script, or just run the LogicGate.py Remember for the run function, only
 the filename argument is needed. The run function will return an exit
@@ -72,15 +71,15 @@
 ~~~~~~~~~~~~~~
 
 There are 2 special syntax
 
 —-- (three hyphens): new word, used for the ascii output separating the
 binary for ascii translation
 
-### (three hashes): comment the entire line
+### (three hashes): comment everything after the syntax
 
 For any of the special syntax, they are not being interpreted as special
 syntax unless the entire syntax appears. They can be anywhere in a line,
 and that line will act like what the syntax shows (if the special syntax
 appears in the same line, they will be scanned and processed according
 to here)
 
@@ -92,13 +91,17 @@
 ``1\n 0\n 0\n 1\n 0\n 0\n 0\n ---\n 1\n 1\n 0\n 0\n 1\n 0\n 1\n ---\n 1\n 1\n 0\n 1\n 1\n 0\n 0\n ---\n 1\n 1\n 0\n 1\n 1\n 0\n 0\n ---\n 1\n 1\n 0\n 1\n 1\n 1\n 1\n ---\n 1\n 0\n 0\n 0\n 0\n 0\n ---\n 1\n 0\n 1\n 0\n 1\n 1\n 1\n ---\n 1\n 1\n 0\n 1\n 1\n 1\n 1\n ---\n 1\n 1\n 1\n 0\n 0\n 1\n 0\n ---\n 1\n 1\n 0\n 1\n 1\n 0\n 0\n ---\n 1\n 1\n 0\n 0\n 1\n 0\n 0\n ---\n 1\n 0\n 0\n 0\n 0\n 1\n``
 
 another version generated by LogicGate.compile():
 ``O1NNAANNNNA1AA1AO0AA1AO1NNANNAA1A1111111111\n NNANNAAAO0O000001\n OO0NNN10\n O1O1NNA1O01\n NNOONNA0O0000\n 0\n AA0NNANNOONNNNAO0A1O0000001\n ---\n OO1O1OAO1NNAO111111\n NNNNO0NNAA1O0N01\n OANNOA0O00000\n ANNNNA001\n NNA11\n NNANNA1ANNO0001\n NNAANNAOOA1NNAO10110111\n ---\n OA111\n A1OA1OO0A1O1NNA1O0ONNNNNNN0000\n A1O0A00\n A1O0NNAO0O0A111\n NNAO1NNONNNNA1O1111\n O0A1OANNA0NNOO0ON10000\n 0\n ---\n O0NNN0\n A1ANNNNNNNNNNO101\n O00\n NNA1OO1ONNAO10110\n OAA1110\n OO0AAO0AAONNO0O0NNO00001100\n NNO0A0ONNN10\n ---\n O0O1O0A1NNO1ANNO0AA1O1AA1A1A11111\n NNANNO1ONNNNNNNNNNO0AO11101\n O0OONNNNAAO0N11000\n A1O0N0\n OONNNNOA1ONNOO0AA11100100\n NNO0ON00\n O0OA1NNA1O100\n ---\n O0OO1OO1A1O1000\n NNOO0AONNONNO0A0NNA0NNA010010\n NNAA0OOOA0O000001\n A0NNNNN1\n AO0NNNNA1OO0001\n O0OA1O0O0OO0OA1O00000\n ---\n 1\n A0NNAO0A0OA0NNA1A0000\n NNO0NNA1NNOO011\n NNO0NNA0A0A0NNOO000\n ANNA1AA1NNNNNNNNAA1NNAA1A111111\n NNA1ANNA1OAO1O11111\n A1A1NNA1O1NNANNA1AA1111\n ---\n ONNNNAOO11110\n OANNOONNA1AA1110111\n AA0NNNNNNO0O0A0O0N10\n NNNNNNOA110\n O1OONNA1101\n A1NNNNA11\n ANNOONNAAO1A1ANNA11111011\n ---\n O0NNO0AO0A111\n NNNNNNA1O0ONNA1NNNNO0NNANNOOA1ANNNNAA11110111\n NNO11\n AO0AN101\n OAA1000\n 1\n O0A0NNO0O0NNA0A0NNA1ON10\n ---\n O0N0\n NNNNNNO0ONNA1N00\n O00\n O0AN01\n NNONNNNNNNNA111\n NNNNONNOO0000\n AONNO0ANNO00101\n ---\n O1ONNANNNNA1111\n NNNNOOOO0NNAA1NNONNO1011111\n NNA0A0A01\n AA1N10\n O1OANNNNNNA1ONNNNOO1AOOO1AAN0110111110\n 0\n OOAO0NNO0A0OAANNA0AONNO0001100000\n ---\n A1A1NNO0NNA11\n OA100\n NNANNOA1001\n 0\n NNO0OA0O000\n ANNO0OONNA1O11001\n ---``
 
 Sources
 -------
-
-Current source code(working in progress): `gitbub
-link <https://github.com/TaokyleYT/LogicGate/>`__\  Esolang wiki:
-`LogicGate <https://esolangs.org/wiki/LogicGate>`__\Replit up-to-date version:
+<br>
+`gitbub
+<https://github.com/TaokyleYT/LogicGate/>`__\
+<br>
+Esolang wiki:
+`LogicGate <https://esolangs.org/wiki/LogicGate>`__\
+<br>
+Replit up-to-date version:
 `replit <https://replit.com/@s3D27ZHOU/LogicGate>`__
```

