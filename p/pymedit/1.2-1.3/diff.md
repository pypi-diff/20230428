# Comparing `tmp/pymedit-1.2-py3-none-any.whl.zip` & `tmp/pymedit-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 56911 bytes, number of entries: 14
--rw-------  2.0 unx     6645 b- defN 21-Apr-08 07:41 pymedit/P0.py
--rw-------  2.0 unx     4171 b- defN 21-Apr-08 07:41 pymedit/P0_3D.py
--rw-------  2.0 unx    17656 b- defN 22-Mar-17 09:08 pymedit/P1.py
--rw-------  2.0 unx    10987 b- defN 21-Apr-08 07:41 pymedit/P1_3D.py
--rw-------  2.0 unx     1263 b- defN 22-Mar-01 09:34 pymedit/__init__.py
--rw-------  2.0 unx    49777 b- defN 21-Apr-08 07:41 pymedit/abstract.py
--rw-------  2.0 unx    26352 b- defN 22-Apr-05 12:44 pymedit/external.py
--rw-------  2.0 unx    18701 b- defN 22-Feb-28 15:30 pymedit/mesh.py
--rw-------  2.0 unx    26597 b- defN 22-Mar-10 16:04 pymedit/mesh3D.py
--rw-------  2.0 unx    35149 b- defN 22-May-05 13:14 pymedit-1.2.dist-info/LICENSE
--rw-------  2.0 unx     7652 b- defN 22-May-05 13:14 pymedit-1.2.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 22-May-05 13:14 pymedit-1.2.dist-info/WHEEL
--rw-------  2.0 unx        8 b- defN 22-May-05 13:14 pymedit-1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1042 b- defN 22-May-05 13:14 pymedit-1.2.dist-info/RECORD
-14 files, 206092 bytes uncompressed, 55233 bytes compressed:  73.2%
+Zip file size: 57739 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     6809 b- defN 23-Jan-16 10:04 pymedit/P0.py
+-rw-r--r--  2.0 unx     4171 b- defN 23-Jan-16 09:55 pymedit/P0_3D.py
+-rw-r--r--  2.0 unx    22090 b- defN 23-Apr-20 09:46 pymedit/P1.py
+-rw-r--r--  2.0 unx    10987 b- defN 23-Jan-16 09:55 pymedit/P1_3D.py
+-rw-r--r--  2.0 unx     1263 b- defN 23-Jan-16 09:55 pymedit/__init__.py
+-rw-r--r--  2.0 unx    49874 b- defN 23-Jan-16 09:55 pymedit/abstract.py
+-rw-r--r--  2.0 unx    26903 b- defN 23-Mar-21 15:13 pymedit/external.py
+-rw-r--r--  2.0 unx    18973 b- defN 23-Mar-23 13:56 pymedit/mesh.py
+-rw-r--r--  2.0 unx    26597 b- defN 23-Jan-16 09:55 pymedit/mesh3D.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Apr-28 08:34 pymedit-1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7622 b- defN 23-Apr-28 08:34 pymedit-1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 08:34 pymedit-1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-28 08:34 pymedit-1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1042 b- defN 23-Apr-28 08:34 pymedit-1.3.dist-info/RECORD
+14 files, 211580 bytes uncompressed, 56061 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: pymedit/mesh.py
 Comment: 
 
 Filename: pymedit/mesh3D.py
 Comment: 
 
-Filename: pymedit-1.2.dist-info/LICENSE
+Filename: pymedit-1.3.dist-info/LICENSE
 Comment: 
 
-Filename: pymedit-1.2.dist-info/METADATA
+Filename: pymedit-1.3.dist-info/METADATA
 Comment: 
 
-Filename: pymedit-1.2.dist-info/WHEEL
+Filename: pymedit-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pymedit-1.2.dist-info/top_level.txt
+Filename: pymedit-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pymedit-1.2.dist-info/RECORD
+Filename: pymedit-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymedit/P0.py

```diff
@@ -80,30 +80,33 @@
                 "Error: "+phi+" should be associated with a 2-D mesh.")
         if self.sol.shape not in [(self.mesh.nt,), (self.mesh.nt, 1)] \
                 or self.n != self.mesh.nt:
             raise Exception("Error: the provided array of values should be"
                             f" of size ({self.mesh.nt},) while it is of size "
                             f"{self.sol.shape}.")
 
-    def plot(self, cmap='jet', doNotPlot=False, tickFormat='2.1f',
+    def plot(self, cmap=None, doNotPlot=False, tickFormat='2.1f',
              bcColor='k', bcLineWidth=0.5, niso=49,
              XLIM=None, YLIM=None, title=None):
         """Plot a P0 function with matplotlib."""
         import matplotlib as mp
         import numpy as np
         import matplotlib.pyplot as plt
         from mpl_toolkits.axes_grid1 import make_axes_locatable
         x, y = self.mesh.vertices[:, 0], self.mesh.vertices[:, 1]
         tri = self.mesh.triangles[:, :-1]-1
         z = self.sol
         fig, ax = plt.subplots()
         vmin = min(z)
         vmax = max(z)
         if len(set(z)) <= 10:
-            cmap = plt.cm.Set3
+            if cmap is None:
+                cmap = plt.cm.Set3
+            else:
+                cmap = plt.cm.get_cmap(cmap)
             values = list(set(z))
             values.sort()
             middles = \
                 [values[0], *[0.5*(x+y) for (x, y)
                               in zip(values[:-1], values[1:])], values[-1]]
             middles[0] = 2*middles[0]-middles[1]
             middles[-1] = 2*middles[-1]-middles[-2]
@@ -115,15 +118,17 @@
                 def __call__(self, value, clip=None):
                     x, y = middles, np.linspace(
                         0, len(values)/cmap.N, len(middles))
                     return np.ma.masked_array(np.interp(value, x, y))
             norm = Normalize()
             bounds = middles
         else:
-            cmap = plt.cm.jet
+            if cmap is None:
+                cmap = 'jet'
+            cmap = plt.cm.get_cmap(cmap)
             cmaplist = [cmap(i) for i in range(cmap.N)]
             bounds = np.linspace(min(z), max(z), min(20, len(set(z))))
             norm = mp.colors.BoundaryNorm(bounds, cmap.N)
         if len(set(z)) <= 10:
             ticks = [0.5*(x+y) for (x, y) in zip(middles[:-1], middles[1:])]
             # print(middles);
             # print(values);
```

## pymedit/P1.py

```diff
@@ -95,14 +95,15 @@
 
             if callable(phi):
                 try:
                     self.sol = np.apply_along_axis(phi, 1, self.mesh.vertices)
                 except TypeError:
                     newsol = lambda x : phi(x[0],x[1])
                     self.sol = np.apply_along_axis(newsol, 1, self.mesh.vertices)
+                self.sol = self.sol.astype(float)
             elif isinstance(phi, P0Function):
                 display("Converting P0 function into P1 function.", 2,
                         self.debug, "green")
                 tic(20)
                 B = integrateP0P1Matrix(self.mesh)
                 A = integrateP1P1Matrix(self.mesh)
                 RHS = B.dot(phi.sol)
@@ -183,47 +184,51 @@
             from matplotlib.tri import Triangulation, LinearTriInterpolator
             triObj = Triangulation(self.mesh.vertices[:,0],self.mesh.vertices[:,1]) 
             #linear interpolation
             self.__triInterp = LinearTriInterpolator(triObj,self.sol)
         return self.__triInterp(x[:,0],x[:,1])
 
     def plot(self, cmap='jet', doNotPlot=False, tickFormat='',
-             niso=49, XLIM=None, YLIM=None,
-             title=None, vmin=None, vmax=None, fill=True, boundary=None,boundary_linewidth=2,
+             niso=49, XLIM=None, YLIM=None, type_plot='tricontourf',
+             title=None, vmin=None, vmax=None, boundary=None,boundary_linewidth=2,
+             fig = None, ax = None,
              **kwargs):
-        """Plot a P1 function with matplotlib."""
         import matplotlib as mp
         import matplotlib.pyplot as plt
         from mpl_toolkits.axes_grid1 import make_axes_locatable
         x, y = self.mesh.vertices[:, 0], self.mesh.vertices[:, 1]
         triang = self.mesh.triangles[:, :-1]-1
-
         z = self.sol
-        if fill:
+        cbar = None
+        if fig is None or ax is None:
             fig, ax = plt.subplots()
-        if not vmin is None:
-            levels = kwargs.get('levels', np.linspace(vmin, vmax, niso))
-            if fill:
-                plot = plt.tricontourf(x, y, triang, z, levels=levels,
-                                       cmap=cmap)
-            else:
-                plot = plt.tricontour(x, y, triang, z,
-                                      levels=levels)
-        else:
+        if vmin is None or vmax is None:
             vmin = min(z)
             vmax = max(z)
-            levels = kwargs.get('levels', np.linspace(vmin, vmax, niso))
-            if fill:
-                plot = plt.tricontourf(x, y, triang, z, niso, cmap=cmap, extend="both")
-            else:
-                fig, ax = self.mesh.plot(doNotPlot=True, colormap='dim',
-                                         boundaryColor='b',
-                                         boundary_linewidth=0.5)
-                plot = ax.tricontour(x, y, triang, z, 1, levels=[
-                                     0], linewidths=0.5, colors='indigo')
+        levels = kwargs.get('levels', np.linspace(vmin, vmax, niso))
+        if 'colors' in kwargs:
+            cmap=None
+        if type_plot == 'tricontourf':
+            plot = ax.tricontourf(x, y, triang, z, niso,
+                                  cmap=cmap, extend="both",
+                                  colors = kwargs.get('colors',None),
+                                  norm = kwargs.get('norm',None),   
+                                  levels=levels,    
+                                  antialiased=kwargs.get('antialiased',False))
+        elif type_plot == 'tricontour':
+            plot = ax.tricontour(x, y, triang, z, cmap=cmap, extend="both",
+                                 levels=levels,
+                                  linewidths=kwargs.get('linewidths',None),
+                                  colors = kwargs.get('colors',None),
+                                  norm = kwargs.get('norm',None))
+        elif type_plot == 'tripcolor':
+            plot = ax.tripcolor(x, y, triang, z, cmap=cmap,
+                                  linewidths=kwargs.get('linewidths',None),
+                                  norm = kwargs.get('norm',None),   
+                                vmin=vmin, vmax=vmax)
         if boundary:
             if boundary == 'all':
                 boundary = self.mesh.Boundaries.keys()
             for i, bc in enumerate(boundary):
                 edges = self.mesh.edges[np.where(self.mesh.edges[:, -1] == bc)[0]]
                 X = self.mesh.vertices[edges[:, 0]-1][:, :-1]
                 Y = self.mesh.vertices[edges[:, 1]-1][:, :-1]
@@ -232,37 +237,117 @@
                 color = mp.cm.Dark2(i)
                 lc = mp.collections.LineCollection(
                     lines, linewidths=boundary_linewidth, colors=color,
                     zorder=100)
                 ax.add_collection(lc)
         if title:
             plt.title(title)
-        if fill:
-            divider = make_axes_locatable(ax)
-            cax = divider.append_axes("right", size="5%", pad=0.05)
-            ax.margins(0)
+        # Colorbar
+        divider = make_axes_locatable(ax)
+        cax = divider.append_axes("right", size="5%", pad=0.05)
+        ax.margins(0)
+        if len(levels)>1:
             cbar = fig.colorbar(plot, cax=cax)
             cbar.set_ticks(np.linspace(vmin, vmax, 5))
             if tickFormat:
                 cbar.set_ticklabels([format(x, tickFormat)
                                      for x in np.linspace(vmin, vmax, 5)])
             cbar.ax.tick_params(labelsize=16)
-            if not kwargs.get('colorbar',True):
-                cbar.remove()
+        if not kwargs.get('colorbar',True) and not cbar is None:
+            cbar.remove()
         ax.set_aspect('equal')
         ax.tick_params(axis='both', which='both', length=0)
         plt.setp(ax.get_xticklabels(), visible=False)
         plt.setp(ax.get_yticklabels(), visible=False)
         if not XLIM is None:
             ax.set_xlim(XLIM)
         if not YLIM is None:
             ax.set_ylim(YLIM)
         if not doNotPlot:
             plt.show()
-        return fig, ax
+        return fig, ax, cbar
+
+
+    #def plot(self, cmap='jet', doNotPlot=False, tickFormat='',
+    #         niso=49, XLIM=None, YLIM=None,
+    #         title=None, vmin=None, vmax=None, fill=True, boundary=None,boundary_linewidth=2,
+    #         fig = None, ax = None,
+    #         **kwargs):
+    #    """Plot a P1 function with matplotlib."""
+    #    import matplotlib as mp
+    #    import matplotlib.pyplot as plt
+    #    from mpl_toolkits.axes_grid1 import make_axes_locatable
+    #    x, y = self.mesh.vertices[:, 0], self.mesh.vertices[:, 1]
+    #    triang = self.mesh.triangles[:, :-1]-1
+
+    #    z = self.sol
+    #    cbar = None
+    #    import ipdb
+    #    ipdb.set_trace()
+    #    if fill and fig is None:
+    #        fig, ax = plt.subplots()
+    #    if not vmin is None:
+    #        levels = kwargs.get('levels', np.linspace(vmin, vmax, niso))
+    #        if fill:
+    #            plot = plt.tricontourf(x, y, triang, z, levels=levels,
+    #                                   cmap=cmap)
+    #        else:
+    #            plot = plt.tricontour(x, y, triang, z,
+    #                                  levels=levels)
+    #    else:
+    #        vmin = min(z)
+    #        vmax = max(z)
+    #        levels = kwargs.get('levels', np.linspace(vmin, vmax, niso))
+    #        if fill:
+    #            plot = ax.tricontourf(x, y, triang, z, niso, cmap=cmap, extend="both")
+    #        else:
+    #            fig, ax = self.mesh.plot(doNotPlot=True, colormap='dim',
+    #                                     boundaryColor='b',
+    #                                     boundary_linewidth=0.5, fig=fig, ax=ax)
+    #            plot = ax.tricontour(x, y, triang, z, 1, levels=[
+    #                                 0], linewidths=0.5, colors='indigo')
+    #    if boundary:
+    #        if boundary == 'all':
+    #            boundary = self.mesh.Boundaries.keys()
+    #        for i, bc in enumerate(boundary):
+    #            edges = self.mesh.edges[np.where(self.mesh.edges[:, -1] == bc)[0]]
+    #            X = self.mesh.vertices[edges[:, 0]-1][:, :-1]
+    #            Y = self.mesh.vertices[edges[:, 1]-1][:, :-1]
+    #            lines = [[tuple(x), tuple(y)]
+    #                     for (x, y) in zip(X.tolist(), Y.tolist())]
+    #            color = mp.cm.Dark2(i)
+    #            lc = mp.collections.LineCollection(
+    #                lines, linewidths=boundary_linewidth, colors=color,
+    #                zorder=100)
+    #            ax.add_collection(lc)
+    #    if title:
+    #        plt.title(title)
+    #    if fill:
+    #        divider = make_axes_locatable(ax)
+    #        cax = divider.append_axes("right", size="5%", pad=0.05)
+    #        ax.margins(0)
+    #        cbar = fig.colorbar(plot, cax=cax)
+    #        cbar.set_ticks(np.linspace(vmin, vmax, 5))
+    #        if tickFormat:
+    #            cbar.set_ticklabels([format(x, tickFormat)
+    #                                 for x in np.linspace(vmin, vmax, 5)])
+    #        cbar.ax.tick_params(labelsize=16)
+    #        if not kwargs.get('colorbar',True):
+    #            cbar.remove()
+    #    ax.set_aspect('equal')
+    #    ax.tick_params(axis='both', which='both', length=0)
+    #    plt.setp(ax.get_xticklabels(), visible=False)
+    #    plt.setp(ax.get_yticklabels(), visible=False)
+    #    if not XLIM is None:
+    #        ax.set_xlim(XLIM)
+    #    if not YLIM is None:
+    #        ax.set_ylim(YLIM)
+    #    if not doNotPlot:
+    #        plt.show()
+    #    return fig, ax, cbar
 
 
 class P1Vector(__AbstractSol):
     """A structure for P1 vectors (components are piecewise linear on 
     each triangle) on a 2D mesh, 
     based on the INRIA .sol and .solb formats."""
 
@@ -330,15 +415,15 @@
 
     @property
     def y(self)->'P1Function':
         """ y component of a P1 vector as a P1 function"""
         return P1Function(self.mesh, self.sol[:, 1], self.debug)
 
     def plot(self, title=None, doNotPlot=False, XLIM=None, YLIM=None,
-             fig=None, ax=None, scaling=1.5,color=False):
+             fig=None, ax=None, scaling=1.5,color=False, **kwargs):
         """ Quiver plot of a 2D vector field with matplotlib"""
         import matplotlib.pyplot as plt
         import matplotlib as mp
         x, y = self.mesh.vertices[:, 0], self.mesh.vertices[:, 1]
         P = list(zip(x, y))
         (vx, vy) = zip(*self.sol)
         if fig is None:
@@ -360,20 +445,28 @@
 
         meshSize = np.mean(localSize)*scaling
         rescale = np.max(norms)/meshSize
         vx = [x/rescale for x in vx]
         vy = [y/rescale for y in vy]
         norm = mp.colors.Normalize()
         norm.autoscale(norms)
+        scale = kwargs.get('scale',1)
+        width = kwargs.get('width',0.002)
+        alpha = kwargs.get('alpha',0.8)
+        headwidth = kwargs.get('headwidth',3.)
         if color:
-            plot = ax.quiver(x, y, vx, vy, norms, units='xy', scale_units='xy',cmap=mp.cm.jet,
-                             angles='xy', scale=1, width=0.002, headwidth=3, alpha=0.8)
+            if isinstance(color,str):
+                plot = ax.quiver(x, y, vx, vy, units='xy', scale_units='xy',color=color,
+                                 angles='xy', scale=scale, width=width, headwidth=headwidth, alpha=alpha)
+            else:
+                plot = ax.quiver(x, y, vx, vy, norms, units='xy', scale_units='xy',cmap=mp.cm.jet,
+                                 angles='xy', scale=scale, width=width, headwidth=headwidth, alpha=alpha)
         else:
             plot = ax.quiver(x, y, vx, vy, color="black", units='xy', scale_units='xy',
-                             angles='xy', scale=1, width=0.002, headwidth=3, alpha=0.8)
+                             angles='xy', scale=scale, width=width, headwidth=headwidth, alpha=alpha)
         if color:
             ax.margins(0)
             cbar = fig.colorbar(plot)
             #cbar.set_ticks(np.linspace(vmin, vmax, 5))
             #if tickFormat:
             #    cbar.set_ticklabels([format(x, tickFormat)
             #                         for x in np.linspace(vmin, vmax, 5)])
@@ -382,14 +475,15 @@
             plt.title(title)
         if not XLIM is None:
             ax.set_xlim(XLIM)
         if not YLIM is None:
             ax.set_ylim(YLIM)
         if not doNotPlot:
             plt.show()
+        return fig, ax
 
 abstractSolClass=__AbstractSol
 class P1Metric(__AbstractSol):
     """A structure for metric files to use with mesh adaptation based on 
     the INRIA .sol and .solb formats."""
 
     def __init__(self, M: Mesh, phi=None, isotropic=False, debug=None):
```

## pymedit/abstract.py

```diff
@@ -883,14 +883,17 @@
 
         writeField(f, "Triangles", self.nt, 'triangles')
         writeField(f, "Edges", self.ne, 'edges')
         writeField(f, "Ridges", self.nri, 'ridges')
         writeField(f, "RequiredEdges", self.nre, 'requiredEdges')
 
         f.write(pack("i", __indicesGmf__['GmfEnd']))
+        nextPos = f.tell()+calcsize("i")
+        # Final size
+        f.write(pack("i",nextPos))
         f.close()
 
         display("Wrote "+meshFile+" in "+toc()+".", 4, self.debug)
 
 
 class __AbstractSol:
     """
```

## pymedit/external.py

```diff
@@ -618,15 +618,33 @@
                         sols[i] = [
                             tmpdir+f"/phi{i}_{j}.solb" for j in [0, 1, 2]]
                 assert len(labels) == nsols
                 assert len(orders) == nsols
             code = """
             load "medit"
             load "iovtk"
+
             mesh3 Th = readmesh3("$MESH");
+
+            func real[int] readSolFile(string fileName){
+                    ifstream f(fileName);
+                    string dummy="";
+                    while(dummy(0:2)!="Sol"){
+                            f>>dummy;
+                    }
+                    int n;
+                    f >> n;
+                real[int]  phi(n);
+                    f >> dummy;
+                    f >> dummy;
+                    for(int i=0;i<n;i++){
+                            f>>phi[i];
+                    }
+                return phi;
+            }
             fespace Fh0(Th,P0);
             fespace Fh1(Th,P1);
             """
             if sols:
                 code += "\nint[int] order = [" \
                     + ",".join([str(int(i)) for i in orders])+"];\n"
                 code += f'string dataname="' + " ".join(labels)+'";'
@@ -636,20 +654,20 @@
                 for i, solFile in enumerate(sols):
                     if isinstance(solFile, list):
                         components = []
                         for j, component in enumerate(solFile):
                             components.append(f'phi{i}{components_labels[j]}')
                             code += f"""
                                 Fh{orders[i]} {components[-1]};
-                                {components[-1]}[] = readsol("{component}");"""
+                                {components[-1]}[] = readSolFile("{component}");"""
                         solutions.append('['+','.join(components)+']')
                     else:
                         code += f"""
                         Fh{orders[i]} phi{i};
-                        phi{i}[] = readsol("{solFile}");"""
+                        phi{i}[] = readSolFile("{solFile}");"""
                         solutions.append(f"phi{i}")
             code += f"""
             savevtk("{output}", Th """
             if sols:
                 code += ","
                 code += ",".join(solutions)
                 code += ',dataname=dataname, order=order'
```

## pymedit/mesh.py

```diff
@@ -29,14 +29,28 @@
         if self.Dimension is None:
             self.Dimension = 2
         if self.Dimension != 2:
             raise Exception("Error: the mesh "+meshFile+" is not of dimension"
                             " 2.")
 
     @property
+    def x(self):
+        """
+        Returns x coordinate of all vertices.
+        """
+        return self.vertices[:,0]
+
+    @property
+    def y(self):
+        """
+        Returns y coordinate of all vertices.
+        """
+        return self.vertices[:,1]
+
+    @property
     def jacobians(self) -> np.ndarray:
         """
         Returns 2 times the area of each triangle, that is 
         | x_B-x_A  x_C-xA  |
         |                  |
         | y_B-y_A  y_C-y_A |
```

## Comparing `pymedit-1.2.dist-info/LICENSE` & `pymedit-1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymedit-1.2.dist-info/METADATA` & `pymedit-1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: pymedit
-Version: 1.2
+Version: 1.3
 Summary: Package pymedit for operating on 2D and 3D meshes in the INRIA mesh format
 Home-page: https://gitlab.com/florian.feppon/pymedit
 Author: Florian Feppon
 Author-email: florian.feppon@polytechnique.edu
 License: GNU GPL version 3
 Keywords: pymedit,mesh
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy (>=1.12.1)
 Requires-Dist: scipy (>=0.19.1)
-Requires-Dist: cvxopt (>=1.2.1)
 Requires-Dist: colored (>=1.3.93)
 Requires-Dist: matplotlib (>=2.0.2)
 
 # PyMedit
 `PyMedit` is a python package which allows to process triangle and tetrahedral meshes
 in the INRIA `.mesh` file format (see e.g. the reference documentations of Cecile
 Dobrzynski [here](https://hal.inria.fr/hal-00681813/file/RT-422.pdf)).
@@ -221,9 +220,7 @@
 Plotting Truncated mesh
 medit /tmp/tmpc35iy48n/Th.meshb
 Wrote Thf.meshb in 0.18s.
 Saved Thf.meshb
 ```
 
 
-
-
```

## Comparing `pymedit-1.2.dist-info/RECORD` & `pymedit-1.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-pymedit/P0.py,sha256=ycmYa0jQuCZeSjtUmSFgu12phB2hGQ0jb5i6igz8yLg,6645
+pymedit/P0.py,sha256=zOtJyLyoFiQd9NdM_2a9QfBKDzkdpwBdA8Yc7stAxog,6809
 pymedit/P0_3D.py,sha256=ht-6EAGQJ-d1IBVgjkhSua5Yt1zi2JgU6n-a1RnXA0o,4171
-pymedit/P1.py,sha256=meb_oLd6fYOtmIDWWlN1j32xz2Di-E3VsfHPbRRV5dE,17656
+pymedit/P1.py,sha256=NkhwjArUwJJ2nmqLRf6JcWvNuNNXHC7GrwyhzaHxPY8,22090
 pymedit/P1_3D.py,sha256=zLc0kxTjXKwv0IAAGSmfthOjUky1ZkbPd4cXZCQGqZY,10987
 pymedit/__init__.py,sha256=KGLZtBZbTEWavTvhVRlI2sK8a3tS-IeIcF6hInsv7Rc,1263
-pymedit/abstract.py,sha256=YJ0Fs_OF-0P_y2ScxMFOdFcgb9LlAQ5ij7hD_seHcG8,49777
-pymedit/external.py,sha256=oq_uKAj4bWeCEBP4qViZMr4kA7jK3yOA4n4LegmkrLM,26352
-pymedit/mesh.py,sha256=nYpUW8djp_xgseN79mZ8QYhCqWLI9b-2AfPkFLHik88,18701
+pymedit/abstract.py,sha256=6TYSfpCA1mPBoXnc3R_uySaAPEstqkdGz9VU_l5GXaE,49874
+pymedit/external.py,sha256=OHtEOq2PeFecI0ZdK-r-8go-L3s0STGEJ43PFZJ1G98,26903
+pymedit/mesh.py,sha256=XiOGE8pUt0DP3B0-sGkCUlt2C0Vu0GBjZLDSTdZR3j4,18973
 pymedit/mesh3D.py,sha256=mBgn25Ht_tEgFUKJiK_ZfyErzC9W7UlpiW4K0lnypGQ,26597
-pymedit-1.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-pymedit-1.2.dist-info/METADATA,sha256=h8H0paf-dOkf5fDaVpg56roqsm_EWTiy-KpbKWme-VI,7652
-pymedit-1.2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-pymedit-1.2.dist-info/top_level.txt,sha256=-WbXbpTwHjv6GSV8xO9Cn8fz2rQ_TjYS3_0dP9CcP3Q,8
-pymedit-1.2.dist-info/RECORD,,
+pymedit-1.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+pymedit-1.3.dist-info/METADATA,sha256=GeosSfyd4nhFzxAa9XuymznQDp6s07mnqWDNU6T-uW8,7622
+pymedit-1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pymedit-1.3.dist-info/top_level.txt,sha256=-WbXbpTwHjv6GSV8xO9Cn8fz2rQ_TjYS3_0dP9CcP3Q,8
+pymedit-1.3.dist-info/RECORD,,
```

