# Comparing `tmp/yacnew-0.1-py3-none-any.whl.zip` & `tmp/yacnew-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4618 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     3052 b- defN 23-Apr-28 03:35 yacnew/__init__.py
+Zip file size: 7143 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    10250 b- defN 23-Apr-28 04:39 yacnew/__init__.py
 -rw-rw-rw-  2.0 fat     3052 b- defN 23-Apr-28 03:22 yacnew/yacnew.py
--rw-rw-rw-  2.0 fat     1060 b- defN 23-Apr-28 03:48 yacnew-0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      368 b- defN 23-Apr-28 03:48 yacnew-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 03:48 yacnew-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-28 03:48 yacnew-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      521 b- defN 23-Apr-28 03:48 yacnew-0.1.dist-info/RECORD
-7 files, 8152 bytes uncompressed, 3700 bytes compressed:  54.6%
+-rw-rw-rw-  2.0 fat     1060 b- defN 23-Apr-28 04:39 yacnew-0.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      368 b- defN 23-Apr-28 04:39 yacnew-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 04:39 yacnew-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-28 04:39 yacnew-0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      522 b- defN 23-Apr-28 04:39 yacnew-0.2.dist-info/RECORD
+7 files, 15351 bytes uncompressed, 6225 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: yacnew/__init__.py
 Comment: 
 
 Filename: yacnew/yacnew.py
 Comment: 
 
-Filename: yacnew-0.1.dist-info/LICENSE.txt
+Filename: yacnew-0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: yacnew-0.1.dist-info/METADATA
+Filename: yacnew-0.2.dist-info/METADATA
 Comment: 
 
-Filename: yacnew-0.1.dist-info/WHEEL
+Filename: yacnew-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: yacnew-0.1.dist-info/top_level.txt
+Filename: yacnew-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: yacnew-0.1.dist-info/RECORD
+Filename: yacnew-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yacnew/__init__.py

```diff
@@ -140,7 +140,271 @@
 - S->+TS - - S-> S->
 T->FR - - T->FR - -
 - R-> R->*FR - R-> R->
 F->i - - F->F(E) - -
     """
     print(s)
 
+def token_separation():
+    s="""
+    import re
+
+#Taking in Input and store as array
+a = open('sample.txt','r')
+text = a.read()
+
+key =['if','else','elif','for','while','break','continue','in','range','int','float','char']
+id = re.findall("[a-zA-Z0-9$_]",text)
+punctuations= [',',"'",'"',".",";",":"]
+operators = ['+','-','*','/','=','>','<','<=','>=','==','(',')']
+
+c1, c2 = 0, 0
+
+for l in text.split("\n"):
+    print(l)
+    for t in l.split():
+        if t in key:
+            print(t+"-> Keyword")
+            c1 +=1
+        elif t in id and t not in re.findall("[0-9]",text):
+            print(t+"-> Identifier")
+            c2+=1
+        elif t in punctuations:
+            print(t+"->Punctuation")
+        elif t in operators:
+            print(t+"-> Operators")
+    print("\n")
+
+print("Count of keywords: ",c1)
+print("Count of identifiers: ",c2)
+-----------input - sample.txt
+int x ;
+list k ;
+for i in k :
+int x = 10 ;
+    """
+    print(s)
+
+def sybbol_table():
+    s="""
+    d_types = ['char','const','double','enum','float','int','long','short','signed',
+           'static','unsigned','void'] #PUT AS MANY AS REQUIRED
+keywords = ['auto','break','case','char','const','continue','default','do','double',
+            'else','enum','extern','float','for','goto','if','int','long','register',
+            'return','short','signed','sizeof','static','struct','switch','typedef',
+            'union','unsigned','void','volatile','while'] #PUT AS MANY AS REQUIRED
+
+id_key, id_var, id_val = [],[],[]
+r_type, num_params, type_params = [],[],[]
+
+a = open('sample.txt','r')
+text = a.read()
+#print(text)
+
+def l_append(var,val,key,return_type='-', no_params='-',params_type ='-' ):
+    id_var.append(var)
+    id_val.append(val)
+    id_key.append(key)
+    r_type.append(return_type)
+    num_params.append(no_params)
+    type_params.append(params_type)
+
+
+for l in text.split("\n")[:-1]:
+    g = l.split()
+    if ';' in g: g.remove(';')
+    while (',' in g): g.remove(',')
+    print("\nl:",g)
+    
+    for j in g: #For each token in g (list of each line)
+        if j == "=":           #(KEYWORD VARIABLES) WITH VALUES Ex: int b = 5
+            print("kvvtemp: ",g)
+            vr = g.index(j) - 1
+            vl = g.index(j) + 1
+            vk = 0
+            l_append(g[vr],g[vl],g[vk]) # Ex: int b = 5
+            del g[vr:vr+3]
+            print("c1",g)
+
+    if ('(' not in g) and len(g)>1: #(KEYWORD VARIABLES) WITHOUT VALUES Ex: int a  
+        for i in range(1,len(g)): #0th index contains keyword
+            #print(temp[i],0,temp[0])
+            l_append(g[i],0,g[0]) # var, val, key
+
+    #FUNCTIONS AND ARGUEMENTS
+    if '(' in g:     
+        d_end, v_end = [], []
+        return_type, var = g[0], g[1]
+        del g[0:2]
+        
+        for i in range(1,len(g)-1): #['(', 'double', 'x', 'double', 'y', ')']
+            if g[i] in d_types:
+                d_end.append(g[i])
+                v_end.append(g[i+1])
+            type_par = [d_end,v_end]
+        
+        l_append(var,'-','-',return_type, (len(g)-2)//2, type_par)  
+        print("c2",g)
+
+#PRINT OUT THE SYMBOL TABLE
+print ("\nThe symbol table for the C code is: \n")
+print ("ID",'\t',"Data Type",'\t',"Return Type",'\t',"InitialValue",
+       '\t','\t',"No. of Parameters",'\t',"Type of Parameters")
+print("-----",'\t',"---------",'\t',"---------",'\t',"---------",
+      "\t\t","---------",'\t\t',"---------",'\n')   
+
+for i in range(0,len(id_key)):
+    print(id_key[i],"\t",id_key[i],"\t\t",r_type[i],"\t\t",id_val[i],"\t\t\t",num_params[i],"\t\t\t",type_params[i],"\n")
+    ---------input - sample.txt
+    int a , b = 5 ;
+char c = 'd' ;
+double Add ( double x , double y ) ;
+    """
+    print(s)
+
+def macro_processor():
+    s="""
+    macros = dict()
+
+f = open("Code.cpp") #Opening the file
+
+for i in f.readlines():
+    l = i.split()
+    if l[0] == '#define': #Define the Macros
+        macros[l[1]] = l[2]
+
+output = []
+f.seek(0) # Bring Input pointer back to 0
+
+for i in f.readlines():
+    l = i.split()
+    if l[0] == '#define': #Ignore the defination lines in code
+        continue
+    for j in range(len(l)): #Replacing macros in each line
+        if l[j] in macros.keys():
+            l[j] = macros[l[j]]
+    output.append(l) #append each line to output list
+
+print("Macros\t\tDeinition") #Display macros and definations
+for m,n in macros.items():
+    print(m + "\t\t" + n)
+
+print("\nExpanded code") #Print the output 2D array of lines
+for x in output:
+    for y in x: 
+        print(y, end = " ")
+    print()
+    -------input - Code.cpp
+    #include <stdio.h>
+#define PI 3.14
+#define AREA(a) (a*a)
+int main() {
+float r, area;
+printf("Enter radius: ");
+scanf("%f", &r);
+printf("Area: %0.2f", PI * AREA(r) );
+return 0;
+}
+    """
+    print(s)
+
+def lex():
+    s="""
+    %{
+int i=0;
+%}
+%%
+[a-zA-Z]*[ ][a-zA-Z]* {i++;}
+%%
+int yywrap(void){}
+int main(){
+yyin=fopen("input.txt","r");
+yylex();
+printf("no of words: %d",i+1);
+}
+----------input
+seg th td yj y
+    """
+    print(s)
+
+def dfa():
+    s="""
+    states = input("Enter the states (space-seperated): ").strip().split(" ")
+alphabets = input("Enter the alphabets (space-seperated): ").strip().split(" ")
+start_state = input("Enter the start state: ").strip()
+Final_States = input("Enter the final states (space-seperated): ").strip().split(" ")
+transition_function = eval(input("Enter the transition table: "))
+
+curr_state = start_state
+walk=""
+inp_string = list(input("Enter the input string: (\'#\' for EOF): ").strip())
+
+for i in inp_string:
+    if i=="#":
+        if curr_state in Final_States:
+            print("\nYes")
+            break
+        else: print("\nNo")
+        break
+    else:
+        curr_state=transition_function[curr_state][i]
+        walk+=curr_state+" -> "
+        
+print("Walk:", start_state+" -> "+walk[:-4])
+-----------input
+A B C D
+a b
+A
+D
+{"A":{"a":"B","b":"A"},"B":{"a":"B","b":"C"},"C":{"a":"B","b":"D"},"D":{"a":"B","b":"A"}}
+    """
+    print(s)
+
+def loader():
+    s="""
+    lines = open("input.txt","r").read().split('\n')
+obcode =[]
+for line in lines:
+    obcode.append(line.split('^'))
+print(obcode)
+
+print("Name of Program: ",obcode[0][1])
+
+for l in obcode[1:]:
+    if l[0]=='E': break
+    addr = int(l[1])
+    for item in l[3:]:
+        print(addr,item[0:2])
+        addr +=1
+        print(addr,item[2:4])
+        addr +=1
+        print(addr,item[4:6])
+        addr +=1
+    print('\n')
+    ----------input.txt
+    H^SAMPLE^001000^0035
+T^001000^0C^001003^071009
+T^002000^03^111111
+E^001000
+    """
+    print(s)
+
+def intermediate():
+    s="""
+    exp=input().split()
+prec=['*','/','+','-']
+flag=1
+t=1
+
+for i in range(len(prec)):
+    for j in range(len(exp)):
+        if(flag==1 and exp[j]==prec[i]):
+            print("t"+str(t)+" = "+exp[j-1]+exp[j]+exp[j+1])
+            flag=0
+            t+=1
+        elif(exp[j]==prec[i]):
+            print("t"+str(t)+"= t"+str(t-1)+exp[j]+exp[j+1])
+            t+=1
+            ---------------input
+            a*b+c/d
+    """
+    print(s)
```

## Comparing `yacnew-0.1.dist-info/LICENSE.txt` & `yacnew-0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `yacnew-0.1.dist-info/RECORD` & `yacnew-0.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-yacnew/__init__.py,sha256=nUrYY8RHyuGhSFpKNjc5e3sWQPfJ485UMuTVvXMI_bI,3052
+yacnew/__init__.py,sha256=z8jryNrzIZAcFPqhH0AUiEgiKhBytrpKNN3eGTH33-4,10250
 yacnew/yacnew.py,sha256=nUrYY8RHyuGhSFpKNjc5e3sWQPfJ485UMuTVvXMI_bI,3052
-yacnew-0.1.dist-info/LICENSE.txt,sha256=sq1tNElDatNZSkjNlS75Kzv8LnlUEDJfbmC5zOpl4O0,1060
-yacnew-0.1.dist-info/METADATA,sha256=ZOe1AryFiwLPJSPr0kV_K9Rtvs3Oq-88Iopogvl8Dcg,368
-yacnew-0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-yacnew-0.1.dist-info/top_level.txt,sha256=1COOBsRUCea2iwTw-0VqPvIRkdD2BfgZU-f0qIu3NGI,7
-yacnew-0.1.dist-info/RECORD,,
+yacnew-0.2.dist-info/LICENSE.txt,sha256=sq1tNElDatNZSkjNlS75Kzv8LnlUEDJfbmC5zOpl4O0,1060
+yacnew-0.2.dist-info/METADATA,sha256=ecXCOL3iVpVPWSkJbV7fWEfGtH81ToAgZHYpiFGFJzo,368
+yacnew-0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+yacnew-0.2.dist-info/top_level.txt,sha256=1COOBsRUCea2iwTw-0VqPvIRkdD2BfgZU-f0qIu3NGI,7
+yacnew-0.2.dist-info/RECORD,,
```

