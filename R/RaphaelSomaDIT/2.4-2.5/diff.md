# Comparing `tmp/RaphaelSomaDIT-2.4-py3-none-any.whl.zip` & `tmp/RaphaelSomaDIT-2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5049 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    10577 b- defN 23-Apr-25 16:37 RaphaelSomaDIT/__init__.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      434 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      591 b- defN 23-Apr-25 16:38 RaphaelSomaDIT-2.4.dist-info/RECORD
-7 files, 13862 bytes uncompressed, 3995 bytes compressed:  71.2%
+Zip file size: 5061 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    10739 b- defN 23-Apr-28 10:09 RaphaelSomaDIT/__init__.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      434 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      591 b- defN 23-Apr-28 10:10 RaphaelSomaDIT-2.5.dist-info/RECORD
+7 files, 14024 bytes uncompressed, 4007 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: RaphaelSomaDIT/__init__.py
 Comment: 
 
-Filename: RaphaelSomaDIT-2.4.dist-info/LICENSE
+Filename: RaphaelSomaDIT-2.5.dist-info/LICENSE
 Comment: 
 
-Filename: RaphaelSomaDIT-2.4.dist-info/LICENSE.txt
+Filename: RaphaelSomaDIT-2.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: RaphaelSomaDIT-2.4.dist-info/METADATA
+Filename: RaphaelSomaDIT-2.5.dist-info/METADATA
 Comment: 
 
-Filename: RaphaelSomaDIT-2.4.dist-info/WHEEL
+Filename: RaphaelSomaDIT-2.5.dist-info/WHEEL
 Comment: 
 
-Filename: RaphaelSomaDIT-2.4.dist-info/top_level.txt
+Filename: RaphaelSomaDIT-2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: RaphaelSomaDIT-2.4.dist-info/RECORD
+Filename: RaphaelSomaDIT-2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RaphaelSomaDIT/__init__.py

```diff
@@ -210,28 +210,34 @@
                 self.mobile = soup.find('input',{'name':'phone_number'}).get('value')
                 self.martial_status = soup.find(id='marital_status_id').find('option',selected=True).text.strip()
 
                 self.nationality = soup.find(id='nationality_id').find('option',selected=True).text.strip()
             
 
                 academic_info = [p for p in links if '/admission/registrationct' in p]
+                
                 academic_info = (f'https://soma.dit.ac.tz/{academic_info[0]}')
+                
                 academic_info = session.get(academic_info).text
                 soup = bs(academic_info,'html.parser')
-
+                
                 self.academic_year = soup.find('h4').text.strip()[-9:]
                 
 
-                module_link = soup.find_all('a')[-3].get("href")
+                module_link = soup.find_all('a')[-4].get("href")
+                
                 module = (f'https://soma.dit.ac.tz{module_link}')
 
                 module = session.get(module).text
+                # print(module)
                 # soup = bs(module,'html.parser')
                 soup = pd.read_html(module)
+                # print(soup)
                 modules = soup[0]['Code'][0][-4]
+                # print(modules)
                 # soup = soup.find('table').find_all('td')[1].text
                 # modules = soup[-4]
                 self.NTA_level = modules
                 
                 sems = list(soup[0]['Semester'])
                 
                 if datetime.datetime.now().month>=4 and datetime.datetime.now().month<=10:
@@ -310,10 +316,8 @@
             elif 'invalid' in p.text:
                self.error = 'Login Failed: invalid credentials'
             else:
                 self.error = 'invalid status code' 
         except:
             self.error = 'no internet connection'
                 
-rex=raphael()
-
-
+rex=raphael()
```

## Comparing `RaphaelSomaDIT-2.4.dist-info/LICENSE` & `RaphaelSomaDIT-2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `RaphaelSomaDIT-2.4.dist-info/LICENSE.txt` & `RaphaelSomaDIT-2.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

