# Comparing `tmp/ersciyt-1.1.tar.gz` & `tmp/ersciyt-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.1.tar", last modified: Wed Apr 26 21:16:39 2023, max compression
+gzip compressed data, was "ersciyt-1.3.tar", last modified: Fri Apr 28 20:28:45 2023, max compression
```

## Comparing `ersciyt-1.1.tar` & `ersciyt-1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 21:16:39.344195 ersciyt-1.1/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-26 21:16:31.000000 ersciyt-1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-26 21:16:31.000000 ersciyt-1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-26 21:16:39.344195 ersciyt-1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-04-26 21:16:31.000000 ersciyt-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 21:16:39.343195 ersciyt-1.1/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 21:16:31.000000 ersciyt-1.1/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-26 21:16:31.000000 ersciyt-1.1/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-26 21:16:31.000000 ersciyt-1.1/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 21:16:39.344195 ersciyt-1.1/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 21:16:31.000000 ersciyt-1.1/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-26 21:16:31.000000 ersciyt-1.1/ersciyt/models.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-26 21:16:31.000000 ersciyt-1.1/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-04-26 21:16:31.000000 ersciyt-1.1/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     6913 2023-04-26 21:16:31.000000 ersciyt-1.1/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 21:16:39.344195 ersciyt-1.1/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-26 21:16:39.000000 ersciyt-1.1/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-26 21:16:39.000000 ersciyt-1.1/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 21:16:39.000000 ersciyt-1.1/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-26 21:16:39.000000 ersciyt-1.1/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 21:16:39.000000 ersciyt-1.1/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-04-26 21:16:39.345195 ersciyt-1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-26 21:16:31.000000 ersciyt-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:28:45.800511 ersciyt-1.3/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-28 20:28:39.000000 ersciyt-1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-28 20:28:39.000000 ersciyt-1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      795 2023-04-28 20:28:45.800511 ersciyt-1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-04-28 20:28:39.000000 ersciyt-1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:28:45.799511 ersciyt-1.3/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:28:39.000000 ersciyt-1.3/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-28 20:28:39.000000 ersciyt-1.3/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-04-28 20:28:39.000000 ersciyt-1.3/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:28:45.800511 ersciyt-1.3/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:28:39.000000 ersciyt-1.3/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-28 20:28:39.000000 ersciyt-1.3/ersciyt/models.py
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-28 20:28:39.000000 ersciyt-1.3/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-04-28 20:28:39.000000 ersciyt-1.3/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     7317 2023-04-28 20:28:39.000000 ersciyt-1.3/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:28:45.800511 ersciyt-1.3/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      795 2023-04-28 20:28:45.000000 ersciyt-1.3/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-28 20:28:45.000000 ersciyt-1.3/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 20:28:45.000000 ersciyt-1.3/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-28 20:28:45.000000 ersciyt-1.3/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-28 20:28:45.000000 ersciyt-1.3/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      687 2023-04-28 20:28:45.801511 ersciyt-1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-28 20:28:39.000000 ersciyt-1.3/setup.py
```

### Comparing `ersciyt-1.1/LICENSE` & `ersciyt-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.1/PKG-INFO` & `ersciyt-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.1
+Version: 1.3
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.1/README.md` & `ersciyt-1.3/README.md`

 * *Files identical despite different names*

### Comparing `ersciyt-1.1/ersciyt/views.py` & `ersciyt-1.3/ersciyt/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,39 @@
 from youtube_transcript_api.formatters import WebVTTFormatter
 #pip install googletrans==4.0.0-rc1
 #from googletrans import Translator
 import re
 
 
 def ytdwn(request,link):
-    try:
+    try:        
+        os.system('yt-dlp -o a.webm https://www.youtube.com/watch?v={}'.format(link))
+        tmp4=open('a.webm' , 'rb')
+        tmp5=tmp4.read()
+        tmp4.close()
+        response=HttpResponse(tmp5, content_type='video/webm')
+        response['Content-Length'] = os.path.getsize('a.webm')
+        response['Content-Disposition'] = 'filename=a.webm'
+        os.remove('a.webm')
+        '''
         video = YouTube('https://www.youtube.com/watch?v=%s' % link)
         stream = video.streams.get_highest_resolution()
         file = str(link)
-        media_dir=os.path.join(settings.BASE_DIR,'ytdown','media')
+        media_dir=os.path.join(settings.BASE_DIR,'media')
         stream.download(output_path=media_dir,filename=file)
         tmp4=open(media_dir + '/' + file , 'rb')
         tmp5=tmp4.read()
         tmp4.close()
         fn=stream.default_filename
         fn=re.sub(r"\s+", '_', fn)
         response=HttpResponse(tmp5, content_type='video/mp4')
         response['Content-Length'] = os.path.getsize(media_dir + '/' + file)
         response['Content-Disposition'] = 'filename=%s' % fn
         os.remove(media_dir + '/' + file)
+        '''
         return response
     except:
         return HttpResponse ('Youtube Url Is Mistake!')
 
 def sub(request,lang,link):
     try:
         video = YouTube('https://www.youtube.com/watch?v=%s' % link)
```

### Comparing `ersciyt-1.1/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.3/ersciyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.1
+Version: 1.3
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.1/setup.cfg` & `ersciyt-1.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.1
+version = 1.3
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
@@ -18,14 +18,15 @@
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	django
-	pytube
+	yt-dlp
+	pytube3
 	youtube-transcript-api
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

