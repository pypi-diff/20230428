# Comparing `tmp/AIUT_RoboticsToolbox-0.0.0.2.tar.gz` & `tmp/AIUT_RoboticsToolbox-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\subjects\postgraduate\robotics\AIUTAPP0002\dist\.tmp-szlurci_\AIUT_RoboticsToolbox-0.0.0.2.tar", last modified: Sun Apr 23 07:25:23 2023, max compression
+gzip compressed data, was "D:\subjects\postgraduate\robotics\AIUTAPP0003\dist\.tmp-s_dkgcf0\AIUT_RoboticsToolbox-0.0.0.3.tar", last modified: Fri Apr 28 14:32:22 2023, max compression
```

## Comparing `AIUT_RoboticsToolbox-0.0.0.2.tar` & `AIUT_RoboticsToolbox-0.0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:25:23.829298 AIUT_RoboticsToolbox-0.0.0.2/
--rw-rw-rw-   0        0        0     1091 2022-03-11 09:15:32.000000 AIUT_RoboticsToolbox-0.0.0.2/LICENSE
--rw-rw-rw-   0        0        0      700 2023-04-23 07:25:23.829298 AIUT_RoboticsToolbox-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       86 2022-03-11 09:13:50.000000 AIUT_RoboticsToolbox-0.0.0.2/README.md
--rw-rw-rw-   0        0        0      633 2023-04-23 07:22:09.000000 AIUT_RoboticsToolbox-0.0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      672 2023-04-23 07:25:23.829298 AIUT_RoboticsToolbox-0.0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 07:25:23.813674 AIUT_RoboticsToolbox-0.0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 07:25:23.829298 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox/
--rw-rw-rw-   0        0        0     7258 2023-04-23 07:12:05.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox/Toolbox.py
--rw-rw-rw-   0        0        0        0 2022-03-06 18:20:23.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:25:23.829298 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/
--rw-rw-rw-   0        0        0      700 2023-04-23 07:25:23.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-23 07:25:23.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:25:23.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-23 07:25:23.000000 AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 14:32:22.221294 AIUT_RoboticsToolbox-0.0.0.3/
+-rw-rw-rw-   0        0        0     1091 2022-03-11 09:15:32.000000 AIUT_RoboticsToolbox-0.0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1285 2023-04-28 14:32:22.221294 AIUT_RoboticsToolbox-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-04-28 14:29:41.000000 AIUT_RoboticsToolbox-0.0.0.3/README.md
+-rw-rw-rw-   0        0        0      633 2023-04-28 14:22:24.000000 AIUT_RoboticsToolbox-0.0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      672 2023-04-28 14:32:22.221294 AIUT_RoboticsToolbox-0.0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 14:32:22.190061 AIUT_RoboticsToolbox-0.0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 14:32:22.205690 AIUT_RoboticsToolbox-0.0.0.3/src/AIUT_RoboticsToolbox/
+-rw-rw-rw-   0        0        0     9638 2023-04-28 14:16:04.000000 AIUT_RoboticsToolbox-0.0.0.3/src/AIUT_RoboticsToolbox/Toolbox.py
+-rw-rw-rw-   0        0        0        0 2022-03-06 18:20:23.000000 AIUT_RoboticsToolbox-0.0.0.3/src/AIUT_RoboticsToolbox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:32:22.205690 AIUT_RoboticsToolbox-0.0.0.3/src/AIUT_RoboticsToolbox.egg-info/
+-rw-rw-rw-   0        0        0     1285 2023-04-28 14:32:22.000000 AIUT_RoboticsToolbox-0.0.0.3/src/AIUT_RoboticsToolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-28 14:32:22.000000 AIUT_RoboticsToolbox-0.0.0.3/src/AIUT_RoboticsToolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 14:32:22.000000 AIUT_RoboticsToolbox-0.0.0.3/src/AIUT_RoboticsToolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-28 14:32:22.000000 AIUT_RoboticsToolbox-0.0.0.3/src/AIUT_RoboticsToolbox.egg-info/top_level.txt
```

### Comparing `AIUT_RoboticsToolbox-0.0.0.2/LICENSE` & `AIUT_RoboticsToolbox-0.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AIUT_RoboticsToolbox-0.0.0.2/pyproject.toml` & `AIUT_RoboticsToolbox-0.0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AIUT_RoboticsToolbox"
-version = "0.0.0.2"
+version = "0.0.0.3"
 authors = [
   { name="Maziar Palhang", email="palhang@cc.iut.ac.ir" },
 ]
 description = "A simple Robotics package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `AIUT_RoboticsToolbox-0.0.0.2/setup.cfg` & `AIUT_RoboticsToolbox-0.0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2041 4955 545f 526f 626f 7469 6373   = AIUT_Robotics
 00000020: 546f 6f6c 626f 780d 0a76 6572 7369 6f6e  Toolbox..version
-00000030: 203d 2030 2e30 2e30 2e31 0d0a 6175 7468   = 0.0.0.1..auth
+00000030: 203d 2030 2e30 2e30 2e33 0d0a 6175 7468   = 0.0.0.3..auth
 00000040: 6f72 203d 204d 617a 6961 7220 5061 6c68  or = Maziar Palh
 00000050: 616e 670d 0a61 7574 686f 725f 656d 6169  ang..author_emai
 00000060: 6c20 3d20 7061 6c68 616e 6740 6363 2e69  l = palhang@cc.i
 00000070: 7574 2e61 632e 6972 0d0a 6465 7363 7269  ut.ac.ir..descri
 00000080: 7074 696f 6e20 3d20 6120 726f 626f 7469  ption = a roboti
 00000090: 6373 2074 6f6f 6c62 6f78 0d0a 6c6f 6e67  cs toolbox..long
 000000a0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
```

### Comparing `AIUT_RoboticsToolbox-0.0.0.2/src/AIUT_RoboticsToolbox/Toolbox.py` & `AIUT_RoboticsToolbox-0.0.0.3/src/AIUT_RoboticsToolbox/Toolbox.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #In the Name of Allah
 # programmer : Maziar Palhang
 # First Edit : Wed. 1399/12/6
 # Last  Edit : Thu. 1402/2/3
-
+# Last  Edit : Fri. 1402/2/8 class scara added, DH table is printed in a better way
+#                            now changed to work with matplotlib7
 import math
 from scipy.linalg import logm, expm
 import matplotlib.pyplot as plt
 import numpy as np
 from mpl_toolkits.mplot3d import axes3d
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
@@ -142,15 +143,30 @@
     return
 
 class SerialLink:
 
     def __init__(self, name, links):
         self.name  = name
         self.links = links
+        print(self.name)
+        print('--------------------------------------------')
+        print('i\talpha\ta\td\ttheta\ttype')
+        print('--------------------------------------------')
+        for i in range(np.size(self.links,0)):
+            print(i+1, end='\t')
+            for j in range(np.size(self.links,1)):
+                print(round(self.links[i][j],2), end='\t')
+            print('\n')
+        print('------------------------------------------')
         
+    #Friday 1402/2/8
+    def toDeg(self,radVal):
+        return radVal*180.0/np.pi
+
+    #create T i w.r.t i-1
     def makeT(self,DH):
         T = np.array([[math.cos(DH[3]),                -math.sin(DH[3]),  0,  DH[1]],
                      [math.sin(DH[3])*math.cos(DH[0]), math.cos(DH[3])*math.cos(DH[0]), -math.sin(DH[0]), -DH[2]*math.sin(DH[0])],
                      [math.sin(DH[3])*math.sin(DH[0]), math.cos(DH[3])*math.sin(DH[0]),  math.cos(DH[0]),  DH[2]*math.cos(DH[0])],
                      [0,                                0,                                0,                1]])
         return T
 
@@ -175,15 +191,15 @@
                 self.links[i][2] = joints[i]
         
         T = self.fkinCalc()
         return T
     
     def plot(self):
         fig = plt.figure(1)
-        ax = fig.gca(projection='3d')
+        ax = fig.add_subplot(projection='3d')
         TT = np.eye(4)
         for i in range(np.size(self.links,0)):
             To = TT
             TT = TT.dot(self.makeT(self.links[i]))
             ax.plot3D([To[0][3],TT[0][3]],[To[1][3],TT[1][3]],[To[2][3],TT[2][3]])
         ax.plot3D([TT[0][3],TT[0][3]+2*TT[0][0]],
                   [TT[1][3],TT[1][3]+2*TT[1][0]],
@@ -194,25 +210,21 @@
         ax.plot3D([TT[0][3],TT[0][3]+2*TT[0][2]],
                   [TT[1][3],TT[1][3]+2*TT[1][2]],
                   [TT[2][3],TT[2][3]+2*TT[2][2]],'b')
 
         minAll = min(TT[0][3],TT[1][3],TT[2][3])
         maxAll = max(TT[0][3],TT[1][3],TT[2][3])
         ax.plot3D([0, 0],[0,0],[0,minAll-1],'y')
-        #ax.set_xlim(-1, TT[0][3]+5)
-        #ax.set_ylim(-1, TT[1][3]+5)
-        #ax.set_zlim(-50, TT[2][3]+5)
         ax.set_xlim(minAll-1, maxAll+1)
         ax.set_ylim(minAll-1, maxAll+1)
         ax.set_zlim(minAll-1, maxAll+1)
         ax.set_xlabel('x')
         ax.set_ylabel('y')
         ax.set_zlabel('z')
         plt.title(self.name)
-        #ax.view_init(30, 60)
         plt.show()
         return 
 
     
 class Puma560(SerialLink):
     def __init__(self,name):
         self.name = name
@@ -223,7 +235,57 @@
         self.links = [[0.0,     0.0,   0.0,  0.0, 0],
                       [-np.pi/2,0.0,   0.0,  0.0, 0],
                       [0.0,     a2,    d3,   0.0, 0],
                       [-np.pi/2,a3,    d4,   0.0, 0],
                       [np.pi/2, 0.0,   0.0,  0.0, 0],
                       [-np.pi/2,0.0,   0.0,  0.0, 0]]
         SerialLink.__init__(self,self.name,self.links)
+
+#scara robot Friday 1402/2/8
+class SCARA(SerialLink):
+    def __init__(self,name,l1,l2):
+        self.name = name
+        self.l1 = l1
+        self.l2 = l2
+        self.links = [[0.0,     0.0,   0.0,  0.0, 0],
+                      [0.0,     l1,    0.0,  0.0, 0],
+                      [0.0,     l2,    0.0,  0.0, 0],
+                      [np.pi,   0.0,   0.0,  0.0, 1]]
+        SerialLink.__init__(self,self.name,self.links)
+
+
+    def invKin(self,T,type='r'):
+        results = []
+        theta123 = math.atan2(T[1][0],T[0][0])
+        d4 = -T[2][3]
+        x = T[0][3]
+        y = T[1][3]
+        c2 = (x*x+y*y-self.l1*self.l1-self.l2*self.l2)/(2*self.l1*self.l2)
+        if (c2 < -1 or c2 > 1):
+            print('invalid location')
+            return []     
+        s2 = math.sqrt(1-c2*c2)
+        theta2 = math.atan2(s2,c2)
+        k1 = self.l1 + self.l2*c2
+        k2 = self.l2*s2
+        theta1 = math.atan2(y,x) - math.atan2(k2,k1)
+        theta3 = theta123 - theta1 - theta2
+        if type == 'r':   #use radians
+            joints = [theta1,theta2,theta3,d4]
+        elif type == 'd': #use degrees
+            joints = [self.toDeg(theta1),self.toDeg(theta2),self.toDeg(theta3),d4]            
+        results.append(joints)
+        
+        s2 = -s2
+        theta2 = math.atan2(s2,c2)
+        k1 = self.l1 + self.l2*c2
+        k2 = self.l2*s2
+        theta1 = math.atan2(y,x) - math.atan2(k2,k1)
+        theta3 = theta123 - theta1 - theta2
+        if type == 'r':  #use radians
+            joints = [theta1,theta2,theta3,d4]
+        elif type == 'd': #use degrees
+            joints = [self.toDeg(theta1),self.toDeg(theta2),self.toDeg(theta3),d4]
+        results.append(joints)
+        
+        return results
+
```

