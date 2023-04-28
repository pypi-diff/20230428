# Comparing `tmp/Turk_game-1.0.3.tar.gz` & `tmp/Turk_game-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Turk_game-1.0.3.tar", last modified: Sat Apr 22 09:26:57 2023, max compression
+gzip compressed data, was "Turk_game-1.0.4.tar", last modified: Fri Apr 28 14:22:03 2023, max compression
```

## Comparing `Turk_game-1.0.3.tar` & `Turk_game-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 09:26:56.000000 Turk_game-1.0.3/
--rw-rw-rw-   0        0        0     1066 2019-06-03 23:39:34.000000 Turk_game-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      298 2023-04-22 09:26:58.000000 Turk_game-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2033 2019-06-03 23:39:34.000000 Turk_game-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 09:26:56.000000 Turk_game-1.0.3/Turk_game.egg-info/
--rw-rw-rw-   0        0        0      298 2023-04-22 09:26:54.000000 Turk_game-1.0.3/Turk_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-04-22 09:26:56.000000 Turk_game-1.0.3/Turk_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 09:26:54.000000 Turk_game-1.0.3/Turk_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 09:26:54.000000 Turk_game-1.0.3/Turk_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2709 2023-04-22 09:25:14.000000 Turk_game-1.0.3/Turk_game.py
--rw-rw-rw-   0        0        0       10 2023-04-11 06:37:16.000000 Turk_game-1.0.3/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-22 09:26:58.000000 Turk_game-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      468 2023-04-22 09:26:38.000000 Turk_game-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:22:02.000000 Turk_game-1.0.4/
+-rw-rw-rw-   0        0        0     1066 2019-06-03 23:39:34.000000 Turk_game-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      277 2023-04-28 14:22:04.000000 Turk_game-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2033 2019-06-03 23:39:34.000000 Turk_game-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 14:22:02.000000 Turk_game-1.0.4/Turk_game.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-04-28 14:22:02.000000 Turk_game-1.0.4/Turk_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-04-28 14:22:02.000000 Turk_game-1.0.4/Turk_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 14:22:02.000000 Turk_game-1.0.4/Turk_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 14:22:02.000000 Turk_game-1.0.4/Turk_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3783 2023-04-28 14:21:02.000000 Turk_game-1.0.4/Turk_game.py
+-rw-rw-rw-   0        0        0       10 2023-04-11 06:37:16.000000 Turk_game-1.0.4/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 14:22:04.000000 Turk_game-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      424 2023-04-28 14:16:26.000000 Turk_game-1.0.4/setup.py
```

### Comparing `Turk_game-1.0.3/LICENSE` & `Turk_game-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Turk_game-1.0.3/README.md` & `Turk_game-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Turk_game-1.0.3/Turk_game.py` & `Turk_game-1.0.4/Turk_game.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,119 @@
+from collections.abc import Callable, Iterable, Mapping
+from typing import Any, Optional
 import pygame as pg
 import threading as th
 import keyboard as ky
 import sys, os , time , random
 
 
+
+
+
+
+pg.init()
+pg.font.init()
+
+
+
+def rastgele(ilk,son,ondalik = False):
+    if ondalik:
+        return random.uniform(ilk,son)
+    else:
+        return random.randint(ilk,son)
+
+
+class is_parcasi(th.Thread):
+    def __init__(self, group: None = None, target: Callable[..., object] | None = None, name: str | None = None, args: Iterable[Any] = ..., kwargs: Mapping[str, Any] | None = None, *, daemon: bool | None = None) -> None:
+        super().__init__(group, target, name, args, kwargs, daemon=daemon)
+
+
+
+class yazi:
+    def __init__(self,text="Made by Turk-game",pixel=1):
+        self.yazi = pg.font.Font.render(text=text,antialias=pixel)
+    def guncelle(self,text,pixel):
+        self.yazi =  pg.font.Font.render(text=text,antialias=pixel)
+
+
+
+def Vektor2_yap(konum):
+    return pg.Vector2(konum)
+
+
+
+def normalize_et(nesne:pg.Vector2):
+    return nesne.normalize()
+
+
+
 def bekle(sure):
     time.sleep(sure)
 
+
+
 def basildi(tus:str):
     return ky.is_pressed(tus)
 
 
 
-
 def carpma_listesi(nesne,diger):
 
     x = nesne.collidelist(diger)
     if x != -1:
         return 1
     else:    
         return 0
 
 
 
-
 def dikdortgen_carp(nesne,diger):
     
     return pg.Rect.colliderect(nesne,diger)
 
 
+
 def ses_yukle(ses):
     pg.mixer.music.load(ses)
 
 
 
 def ses_cal():
     pg.mixer.music.play()
 
 
+
 def s_duraklat():
     pg.mixer.music.pause()
 
 
 
 def s_devam():
     pg.mixer.music.unpause()
 
 
 
 def s_durdur():
     pg.mixer.stop()
 
 
-pg.init()
-
-
 
-class Turk_rect:
-    def __init__(self,ozellik):
-        self.rect = pg.rect.Rect(ozellik[0:2],ozellik[2:])
+class dikdortgen():
+    def __init__(self,konum:list or pg.Vector2,boyut:list):
+        self.rect = pg.rect.Rect(konum,boyut)
     
     def carp(self,diger,carpma_tip):
         return carpma_tip(self.rect,diger)
             
-    def guncelle(self,ozellik):
-        self.rect = pg.rect.Rect(ozellik[0:2],ozellik[2:])
+    def guncelle(self,konum:list or pg.Vector2,boyut:list):
+        self.rect = pg.rect.Rect(konum,boyut)
 
 
 
-class Turk_resim:
+class resim():
     def __init__(self,resim,boyut:list):
         self.resim = pg.transform.scale(pg.image.load(resim),boyut)
     def guncelle(self,resim,boyut:list):
         self.resim = pg.transform.scale(pg.image.load(resim),boyut)
         
 
     
@@ -82,21 +123,23 @@
             self.ikon = pg.transform.scale(pg.image.load(ikon),(320,320))
             pg.display.set_icon(self.ikon)
         pg.display.set_caption(str(baslik))
         self.___ekran___ = pg.display.set_mode((x,y))
         self.running = True  # running özelliğini tanımla
         #self.dongu(normal_islem,event_islem,kapandi_islem,yenileme_cesidi)
 
-    def yerlestir(self,nesne):
-        if type(nesne[0]) == Turk_resim:
-            self.___ekran___.blit(nesne[0].resim,(nesne[1],nesne[2]))
+    def yerlestir(self,nesne,konum):
+        if type(nesne) == resim:
+            self.___ekran___.blit(nesne.resim,konum)
+        elif type(nesne) == yazi:
+            self.___ekran___.blit(nesne.yazi,konum)
         else:
-            self.___ekran___.blit(nesne[0],(nesne[1],nesne[2]))
+            self.___ekran___.blit(nesne,konum)
 
-    def ciz(self,nesne:Turk_rect,renk):
+    def ciz(self,nesne:dikdortgen,renk):
         pg.draw.rect(self.___ekran___,renk,nesne.rect)
 
     def update(self):
         pg.display.update()
 
     def flip(self):
         pg.display.flip()
```

