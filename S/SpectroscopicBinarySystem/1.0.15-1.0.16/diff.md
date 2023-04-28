# Comparing `tmp/SpectroscopicBinarySystem-1.0.15.tar.gz` & `tmp/SpectroscopicBinarySystem-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.0.15.tar", last modified: Tue Apr 25 15:58:03 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.0.16.tar", last modified: Fri Apr 28 12:14:31 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.0.15.tar` & `SpectroscopicBinarySystem-1.0.16.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 15:58:03.957713 SpectroscopicBinarySystem-1.0.15/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.15/LICENSE
--rw-rw-rw-   0        0        0     1727 2023-04-25 15:58:03.957713 SpectroscopicBinarySystem-1.0.15/PKG-INFO
--rw-rw-rw-   0        0        0     1336 2023-04-25 14:55:51.000000 SpectroscopicBinarySystem-1.0.15/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 15:58:03.949714 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     1727 2023-04-25 15:58:03.000000 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-04-25 15:58:03.000000 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 15:58:03.000000 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-04-25 15:58:03.000000 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-25 15:58:03.000000 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.0.15/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-04-25 15:58:03.957713 SpectroscopicBinarySystem-1.0.15/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 15:58:03.949714 SpectroscopicBinarySystem-1.0.15/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    24777 2023-04-25 15:56:36.000000 SpectroscopicBinarySystem-1.0.15/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:14:31.946306 SpectroscopicBinarySystem-1.0.16/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.16/LICENSE
+-rw-rw-rw-   0        0        0     2127 2023-04-28 12:14:31.946306 SpectroscopicBinarySystem-1.0.16/PKG-INFO
+-rw-rw-rw-   0        0        0     1736 2023-04-28 12:13:45.000000 SpectroscopicBinarySystem-1.0.16/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 12:14:31.942301 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     2127 2023-04-28 12:14:31.000000 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-04-28 12:14:31.000000 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 12:14:31.000000 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-04-28 12:14:31.000000 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-28 12:14:31.000000 SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.0.16/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-04-28 12:14:31.950312 SpectroscopicBinarySystem-1.0.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 12:14:31.946306 SpectroscopicBinarySystem-1.0.16/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    26258 2023-04-28 12:13:45.000000 SpectroscopicBinarySystem-1.0.16/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.0.15/LICENSE` & `SpectroscopicBinarySystem-1.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.15/PKG-INFO` & `SpectroscopicBinarySystem-1.0.16/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.15
+Version: 1.0.16
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -38,19 +38,30 @@
 from spectroscopicbinarysystem import SpectroscopicBinarySystem
 
 sbs = SpectroscopicBinarySystem(
     object_name='hd123299',
     spectra_path='./examples/alphadra/',
     t0=2451441.804,
     period_guess=51,
+    conf={
+        "LAMBDA_REF": 6562.82,
+        "LINE_FIT_MODEL": "voigt",
+        "LINE_FIT_WINDOW_WIDTH": 10,
+        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1.5,
+        "LINE_FIT_FWHM": .5,
+        "RV_CORR_TYPE": "barycentric",
+        "SB_TYPE": 1
+    },
     debug=True)
 
 # plot result with matplotlib and save the results
 sbs.plotRadialVelocityCurve(title="α Dra - HD123299 - Phased radial velocities", savefig=True)
 
 # display result with plotly
 sbs.plotlyRadialVelocityCurve(
     title="α Dra - HD123299 - Phased radial velocities")
 ```
 
-![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/sbs_phased_result.png)
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_phased_result.png)
+
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_debug_result.png)
```

### Comparing `SpectroscopicBinarySystem-1.0.15/README.md` & `SpectroscopicBinarySystem-1.0.16/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -26,19 +26,30 @@
 from spectroscopicbinarysystem import SpectroscopicBinarySystem
 
 sbs = SpectroscopicBinarySystem(
     object_name='hd123299',
     spectra_path='./examples/alphadra/',
     t0=2451441.804,
     period_guess=51,
+    conf={
+        "LAMBDA_REF": 6562.82,
+        "LINE_FIT_MODEL": "voigt",
+        "LINE_FIT_WINDOW_WIDTH": 10,
+        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1.5,
+        "LINE_FIT_FWHM": .5,
+        "RV_CORR_TYPE": "barycentric",
+        "SB_TYPE": 1
+    },
     debug=True)
 
 # plot result with matplotlib and save the results
 sbs.plotRadialVelocityCurve(title="α Dra - HD123299 - Phased radial velocities", savefig=True)
 
 # display result with plotly
 sbs.plotlyRadialVelocityCurve(
     title="α Dra - HD123299 - Phased radial velocities")
 ```
 
-![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/sbs_phased_result.png)
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_phased_result.png)
+
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_debug_result.png)
```

### Comparing `SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.0.16/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.15
+Version: 1.0.16
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -38,19 +38,30 @@
 from spectroscopicbinarysystem import SpectroscopicBinarySystem
 
 sbs = SpectroscopicBinarySystem(
     object_name='hd123299',
     spectra_path='./examples/alphadra/',
     t0=2451441.804,
     period_guess=51,
+    conf={
+        "LAMBDA_REF": 6562.82,
+        "LINE_FIT_MODEL": "voigt",
+        "LINE_FIT_WINDOW_WIDTH": 10,
+        "LINE_FIT_CONT_NORM_EXCLUDE_WIDTH": 1.5,
+        "LINE_FIT_FWHM": .5,
+        "RV_CORR_TYPE": "barycentric",
+        "SB_TYPE": 1
+    },
     debug=True)
 
 # plot result with matplotlib and save the results
 sbs.plotRadialVelocityCurve(title="α Dra - HD123299 - Phased radial velocities", savefig=True)
 
 # display result with plotly
 sbs.plotlyRadialVelocityCurve(
     title="α Dra - HD123299 - Phased radial velocities")
 ```
 
-![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/sbs_phased_result.png)
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_phased_result.png)
+
+![results](https://github.com/guillbertrand/spectrobinarystarsystem/blob/master/examples/alphadra/sbs_debug_result.png)
```

### Comparing `SpectroscopicBinarySystem-1.0.15/setup.cfg` & `SpectroscopicBinarySystem-1.0.16/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 302e 3135 0d0a  rsion = 1.0.15..
+00000030: 7273 696f 6e20 3d20 312e 302e 3136 0d0a  rsion = 1.0.16..
 00000040: 6175 7468 6f72 203d 2047 7569 6c6c 6175  author = Guillau
 00000050: 6d65 2042 6572 7472 616e 640d 0a61 7574  me Bertrand..aut
 00000060: 686f 725f 656d 6169 6c20 3d20 6762 652e  hor_email = gbe.
 00000070: 696f 4070 6d2e 6d65 0d0a 6465 7363 7269  io@pm.me..descri
 00000080: 7074 696f 6e20 3d20 5079 7468 6f6e 2061  ption = Python a
 00000090: 7374 726f 6e6f 6d79 2074 6f6f 6c73 2066  stronomy tools f
 000000a0: 6f72 2073 7065 6374 726f 7363 6f70 6963  or spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.0.15/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.0.16/spectroscopicbinarysystem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,29 +151,40 @@
         Compute the radial velocity from a line position and a radial velocity correction
         Reference line rest position in Angstroms can be customize in conf["LAMBDA_REF"]
         :return: None
         """
         c = const.c.to('km/s')
         self._rv = (c * ((self._center_of_line -
                     self._conf["LAMBDA_REF"]) / self._conf["LAMBDA_REF"])) + self._rv_corr
+        
+    def getCenterOfLine(self):
+        """
+        Return the center of the line computed for the spectrum using a fit (non corrected from heliocentric/barycentric velocity)
+        :return: Float
+        """
+        return self._center_of_line
+
+    def getDebugLineFitting(self):
+        return self._debug_line_fitting
 
     def findCenterOfLine(self):
         """
         Find the center of the line in a spectrum using a fit (models available : Gaussian1D, Lorentz1D, Voigt1D)
         :return: None
         """
         w1 = float(self._conf['LINE_FIT_WINDOW_WIDTH']) / 2
         w2 = float(self._conf['LINE_FIT_CONT_NORM_EXCLUDE_WIDTH']) / 2
         fwhm = float(self._conf['LINE_FIT_FWHM'])
 
-        # [2:-2] > Hack to excude first and last value of the spectra.
-        # Sometimes fist value for the intensity is equal to 0.00 and prevents finding the true minima.
+        # > Hack to replace zero values of the spectra.
+        # Sometimes first value for the intensity is equal to 0.00 and prevents finding the true minima.
         # Ex : sample/alphadra/_alphadra_20230406_856.fits
-        ipeak = self.flux[2:-2].argmin()
-        xpeak = self.spectral_axis[ipeak+2].to(u.AA)
+        self.flux[self.flux == 0] = 1 * u.Jy
+        ipeak = self.flux.argmin()
+        xpeak = self.spectral_axis[ipeak].to(u.AA)
 
         invert_s = extract_region(Spectrum1D(flux=self.flux * -1, wcs=self.wcs),
                                   SpectralRegion(xpeak - (w1 * u.AA), xpeak + (w1 * u.AA)))
 
         s_fit = fit_generic_continuum(invert_s,
                                       exclude_regions=[SpectralRegion(xpeak - (w2 * u.AA), xpeak + (w2 * u.AA))])
         invert_s = invert_s / s_fit(invert_s.spectral_axis)
@@ -199,16 +210,15 @@
 
         match self._conf['LINE_FIT_MODEL']:
             case 'gaussian':
                 center = g_fit.mean
             case _:
                 center = g_fit.x_0
 
-        self._debug_line_fitting = {
-            'extracted_profil': invert_s, 'fit_solution': y_fit}
+        self._debug_line_fitting = (invert_s, y_fit)
         self._center_of_line = center.value
 
     def __str__(self):
         return f"Spectrum : {self._basename}\n- obs: {self._observer}\n- jd: {self._jd}\n- center: {self._center_of_line} A\n- {self._conf['RV_CORR_TYPE']}: {self._rv_corr}\n- rv: {self._rv}\n "
 
 #
 
@@ -250,17 +260,19 @@
         self._t0 = t0
         self._period = period
         self._period_guess = period_guess
         self._debug = debug
 
         # load user configuration or defaults
         if conf:
-            self._conf = self._conf.update(conf)
+            self._conf.update(conf)
 
+        print('** SpectroscopicBinarySystem **')
         self.__findObjectCoordinate()
+        print('Load spectra...')
         self.__loadSpectra()
 
     def __findObjectCoordinate(self):
         # try to find the coordinates with the common name of the object
         self._skycoord = None
         if result_table := Simbad.query_object(self._object_name):
             ra = result_table[0]['RA']
@@ -276,14 +288,31 @@
                     sbSpec1D = SBSpectrum1D(
                         spectrum_filename, self._skycoord, self._conf)
                     self._sb_spectra.append(sbSpec1D)
                     if self._debug:
                         print(sbSpec1D)
         if self._debug:
             print(f'{len(self._sb_spectra)} processed spectra')
+            plt.rcParams['font.size'] = '6'
+            plt.rcParams['font.family'] = 'monospace'
+            grid_size = math.ceil(len(self._sb_spectra)/6)
+            fig, axs = plt.subplots(6,grid_size, figsize=(13,7), sharex=True, sharey=True)
+            for i, s in enumerate(self._sb_spectra):
+                ax = axs.flat[i]
+                extracted_profil, line_fitting = s.getDebugLineFitting()
+                ax.set_title(f'{s.getBaseName()}\n{s.getObserver()} JD={s.getJD()}', fontsize="6")
+                ax.grid(True)
+                ax.tick_params(axis='both', which='major', labelsize=6)
+                ax.tick_params(axis='both', which='minor', labelsize=6)
+                ax.plot(extracted_profil.spectral_axis.to(u.AA), extracted_profil.flux, color="k")
+                ax.plot(extracted_profil.spectral_axis.to(u.AA), line_fitting, color="r")
+                ax.axvline(x=s.getCenterOfLine(), color='r', linestyle='-',lw=0.7)
+            plt.tight_layout(pad=0.8, w_pad=2, h_pad=1)
+            plt.savefig(f'{self._spectra_path}/sbs_debug_result.png', dpi=150)
+            plt.show()
 
     def __getPhase(self, jd0, period, jd):
         """
         Compute the phase of a given JD
         :param jd0: JD of the first observation
         :param period: period of the orbit
         :param jd: JD to compute the phase
@@ -329,26 +358,25 @@
             Pguess=self._period_guess,
             covariance=True,
             graphs=False,
         )
 
         self._orbital_solution = (params, err, cov)
 
-        if self._debug:
-            print(
-                f'{self._object_name} orbital solution',
-                f'- γ = {params[0]} ± {err[0]}',
-                f'- K = {params[1]} ± {err[1]}',
-                f'- ω = {params[2]} ± {err[2]}',
-                f'- e = {params[3]} ± {err[3]}',
-                f'- T0 = {params[4]} ± {err[4]}',
-                f'- P = {params[5]} ± {err[5]}',
-                f'- a = {params[6]} ± {err[6]}',
-                f'- f(M) = {params[7]} ± {err[7]}',
-                sep='\n')
+        print(
+            f'{self._object_name} orbital solution with {len(self._sb_spectra)} spectra',
+            f'- γ = {params[0]} ± {err[0]}',
+            f'- K = {params[1]} ± {err[1]}',
+            f'- ω = {params[2]} ± {err[2]}',
+            f'- e = {params[3]} ± {err[3]}',
+            f'- T0 = {params[4]} ± {err[4]}',
+            f'- P = {params[5]} ± {err[5]}',
+            f'- a = {params[6]} ± {err[6]}',
+            f'- f(M) = {params[7]} ± {err[7]}',
+            sep='\n')
 
     def getOrbitalSolution(self):
         self.__solveSystem()
         return self._orbital_solution
 
     def __findNearest(self, array, value):
         """
@@ -405,22 +433,22 @@
             label = f"{obs} - {s.getInstrument()[:30]}…"
             if label not in instruments.keys():
                 if obs not in marker_index:
                     marker_index[obs] = 0
                 instruments[label] = markers_style[marker_index[obs]]
                 marker_index[obs] += 1
                 axs[0].errorbar(s.getPhase(), s.getRV(
-                ), yerr=0, label=label, ecolor='k', capsize=0, fmt=instruments[label], color=color, lw=0.7, markersize=4)
+                ), yerr=0, label=label, ecolor='k', capsize=0, fmt=instruments[label], color=color, lw=0.7, markersize=5)
             else:
                 axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
-                                fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=4)
+                                fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
 
             xindex = self.__findNearest(self._model_x, s.getPhase())
             axs[1].errorbar(s.getPhase(), s.getRV() - self._model_y[xindex],
-                            yerr=0, fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=4)
+                            yerr=0, fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
 
     def plotRadialVelocityCurve(self, title, subtitle="", rv_y_multiple=10, residual_y_multiple=0.5, savefig=False, dpi=150, font_family='monospace', font_size=9):
         if not self._orbital_solution:
             self.__solveSystem()
 
         plt.rcParams['font.size'] = font_size
         plt.rcParams['font.family'] = font_family
@@ -573,15 +601,15 @@
                                    y=[s.getRV()],
                                    mode='markers',
                                    name=label,
                                    marker_symbol=instruments[label],
                                    marker=dict(color=color,
                                                size=8),
                                    showlegend=True))
-            else: # no grouping
+            else:  # no grouping
                 # set label to date
                 label = f"{obs} - {s.getDate()}"
                 fig.add_trace(
                     go.Scatter(x=[phase],
                                y=[s.getRV()],
                                mode='markers',
                                name=label,
```

