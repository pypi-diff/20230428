# Comparing `tmp/nustarpipeline-0.2.5.tar.gz` & `tmp/nustarpipeline-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nustarpipeline-0.2.5.tar", last modified: Thu Apr  6 06:56:39 2023, max compression
+gzip compressed data, was "nustarpipeline-0.2.6.tar", last modified: Fri Apr 28 09:16:09 2023, max compression
```

## Comparing `nustarpipeline-0.2.5.tar` & `nustarpipeline-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-04-06 06:56:39.955982 nustarpipeline-0.2.5/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1071 2022-08-24 20:22:52.000000 nustarpipeline-0.2.5/LICENSE
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-04-06 06:56:39.955982 nustarpipeline-0.2.5/PKG-INFO
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      688 2022-08-26 16:47:35.000000 nustarpipeline-0.2.5/README.md
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-04-06 06:56:39.955982 nustarpipeline-0.2.5/nustarpipeline/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        0 2022-08-26 16:41:51.000000 nustarpipeline-0.2.5/nustarpipeline/__init__.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    40130 2023-02-15 00:21:50.000000 nustarpipeline-0.2.5/nustarpipeline/process.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    86664 2023-04-06 06:55:43.000000 nustarpipeline-0.2.5/nustarpipeline/utils.py
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-04-06 06:56:39.955982 nustarpipeline-0.2.5/nustarpipeline.egg-info/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-04-06 06:56:39.000000 nustarpipeline-0.2.5/nustarpipeline.egg-info/PKG-INFO
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      343 2023-04-06 06:56:39.000000 nustarpipeline-0.2.5/nustarpipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2023-04-06 06:56:39.000000 nustarpipeline-0.2.5/nustarpipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      188 2023-04-06 06:56:39.000000 nustarpipeline-0.2.5/nustarpipeline.egg-info/entry_points.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      101 2023-04-06 06:56:39.000000 nustarpipeline-0.2.5/nustarpipeline.egg-info/requires.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       15 2023-04-06 06:56:39.000000 nustarpipeline-0.2.5/nustarpipeline.egg-info/top_level.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1541 2023-04-06 06:56:39.955982 nustarpipeline-0.2.5/setup.cfg
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      361 2023-04-06 06:55:38.000000 nustarpipeline-0.2.5/setup.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-04-28 09:16:09.180840 nustarpipeline-0.2.6/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1071 2022-08-24 20:22:52.000000 nustarpipeline-0.2.6/LICENSE
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-04-28 09:16:09.180840 nustarpipeline-0.2.6/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      688 2022-08-26 16:47:35.000000 nustarpipeline-0.2.6/README.md
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-04-28 09:16:09.180840 nustarpipeline-0.2.6/nustarpipeline/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        0 2022-08-26 16:41:51.000000 nustarpipeline-0.2.6/nustarpipeline/__init__.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    40130 2023-02-15 00:21:50.000000 nustarpipeline-0.2.6/nustarpipeline/process.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    87077 2023-04-28 09:04:17.000000 nustarpipeline-0.2.6/nustarpipeline/utils.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-04-28 09:16:09.180840 nustarpipeline-0.2.6/nustarpipeline.egg-info/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      343 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      188 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      101 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/requires.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       15 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/top_level.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1541 2023-04-28 09:16:09.184840 nustarpipeline-0.2.6/setup.cfg
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      361 2023-04-28 09:15:40.000000 nustarpipeline-0.2.6/setup.py
```

### Comparing `nustarpipeline-0.2.5/LICENSE` & `nustarpipeline-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nustarpipeline-0.2.5/PKG-INFO` & `nustarpipeline-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nustarpipeline
-Version: 0.2.5
+Version: 0.2.6
 Summary: nustar-pipeline
 Home-page: https://gitlab.astro.unige.ch/ferrigno/nustar-pipeline
 Author: C.F.
 Author-email: carlo.ferrigno@unige.ch
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `nustarpipeline-0.2.5/README.md` & `nustarpipeline-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nustarpipeline-0.2.5/nustarpipeline/process.py` & `nustarpipeline-0.2.6/nustarpipeline/process.py`

 * *Files identical despite different names*

### Comparing `nustarpipeline-0.2.5/nustarpipeline/utils.py` & `nustarpipeline-0.2.6/nustarpipeline/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -958,16 +958,17 @@
         k = k + 1
 
     if n_harm <=0:
         m4 = 4*np.arange(1,K+1)
         cumulative_sum = np.zeros(K)
         for k in range(1,K):
             cumulative_sum[k] = np.sum( (a[0:k]/sigma_a[0:k])**2 + (b[0:k]/sigma_b[0:k])**2)
+        #print(cumulative_sum)
         max_harm = np.argmax(cumulative_sum - m4)+1
-        logger.debug("We stop at %d harmonics" % max_harm)
+        #print("We stop at %d harmonics" % max_harm)
     else:
         max_harm = n_harm
     somma = a[0:max_harm] ** 2 + b[0:max_harm] ** 2
     # print(somma)
     differenza = sigma_a[0:max_harm] ** 2 + sigma_b[0:max_harm] ** 2
     bla = somma - differenza
     # print('diff: ',differenza)
@@ -1080,15 +1081,15 @@
         with open(output_file, 'w') as ff:
             ff.write("Energy Energy_error Pulsed_fraction Pulsed_fraction_Error\n")
             for i in range(0, len(e_min)):
                 ff.write("%.2f %.2f %.4f %.4f\n" % (ee_pulsed[i], dee_pulsed[i], 
                             pulsed_frac[i], dpulsed_frac[i]))
     return ee_pulsed, dee_pulsed, pulsed_frac, dpulsed_frac
 
-def elaborate_pulsed_fraction(ee_pulsed, dee_pulsed, pulsed_frac, dpulsed_frac, debug_plots=True, e1=10, e2=20, 
+def elaborate_pulsed_fraction(ee_pulsed, dee_pulsed, pulsed_frac, dpulsed_frac, debug_plots=True, e1=10, e2=20, ylabel = 'PF',
                               stem='', poly_deg=[3, 3], title='', save_plot=True, e_threshold=0.3, 
                               division_derivative_order=2, max_n_high_lines = 2, forced_gaussian_centroids = [],
                               forced_gaussian_amplitudes = [],
                               forced_gaussian_sigmas = [],
                               y_lim=[0,1], 
                               noFe=False):
     """This function implements the logics to perform a fit of the pulsed fraction.
@@ -1104,14 +1105,15 @@
         ee_pulsed (numpy array): energy
         dee_pulsed (numpy array): energy error
         pulsed_frac (numpy array): pulsed fraction
         dpulsed_frac (numpy array): pulsed fraction uncertainty
         debug_plots (bool, optional): plot the derivative and the fits. Defaults to True.
         e1 (int, optional): lower energy to search the flex in this interval. Defaults to 10.
         e2 (int, optional): lower energy to search the flex in this interval. Defaults to 20.
+        ylabel (str) : label of the y axis. Default 'PF', first, second for amplitude of 1st and 2nd hamonics, respectively
         Note that if you put e1>=e2, we will use only one interval.
         stem (str, optional): a string in fron of output plot names. Defaults to ''.
         poly_deg (int or list of int, optional): degree of the polynomial. Defaults to 3.
         title (str, optional): title of the plots. Defaults to ''.
         save_plot (bool, optional): if plots should be saved Defaults to True.
         e_threshold (float, optional): if energies of PF minima differ in relative terms less than this values, they are reduced.
                                        ex.: if the algorithm finds minima at 32 and 35 keV, it retains only 32.
@@ -1230,15 +1232,15 @@
 
 
 
     pulsed_fit_low = fit_pulsed_frac(ee_pulsed[ind_low],dee_pulsed[ind_low], 
                                         pulsed_frac[ind_low], dpulsed_frac[ind_low], n_gauss=n_gauss, 
                                        center=center,
                                         sigma=sigma,
-                                        amplitude=amplitude,
+                                        amplitude=amplitude, ylabel = ylabel,
                                        degree_pol=poly_deg[0], plot_final=True, stem=stem+'low', y_lim=y_lim)
 
     if make_double_fit:
 
         e_cyc = get_zeros(fake_en, smoothed_pulsed_frac_deriv, smoothed_pulsed_frac_deriv_2, fake_en>e_turn)
         
         if len(e_cyc)>1:
@@ -1297,15 +1299,15 @@
         
         pulsed_fit_high = fit_pulsed_frac(ee_pulsed[ind_high],dee_pulsed[ind_high], 
                                             pulsed_frac[ind_high], dpulsed_frac[ind_high], n_gauss=n_gauss, 
                                         center=center,
                                             sigma=sigma,
                                             amplitude=amplitude,
                                         degree_pol=high_poly_deg, plot_final=True, stem=stem+'high',
-                                        y_lim=y_lim)
+                                        y_lim=y_lim,ylabel = ylabel)
     else:
         pulsed_fit_high = None
 
     
     from matplotlib.pyplot import cm
     comps_low = pulsed_fit_low.eval_components(x=ee_pulsed[ind_low])
     bb_low = (pulsed_frac[ind_low] - pulsed_fit_low.best_fit) / dpulsed_frac[ind_low]
@@ -1325,15 +1327,15 @@
     if make_double_fit:
         ax1.plot(ee_pulsed[ind_high], pulsed_fit_high.best_fit, '-', label='best fit (high)', color=col[2])
         ax1.plot(ee_pulsed[ind_high], comps_high['poly_'], '--', label='Polynomial (high)', color=col[3])
 
     ax1.legend(loc='upper left')
     ax1.set_xscale('log')
     ax2.set_xlabel('E (keV)')
-    ax1.set_ylabel('PF')
+    ax1.set_ylabel(ylabel)
     ax1.set_ylim(y_lim)
     #ax1.set_xlim(x_lim)
     ax1.set_title(title)
     if noFe is False:
         ax1.axvline(6.5, 0,1, linestyle='--', color='cyan')
     for x in forced_gaussian_centroids:
         ax1.axvline(x, 0,1, linestyle='--', color='cyan')
@@ -1350,15 +1352,15 @@
     if save_plot:
         plt.savefig(stem + 'global_pulsed_fitted.pdf')
 
     return pulsed_fit_low, pulsed_fit_high, e_turn
 
 def fit_pulsed_frac(en, den, pf, dpf, stem=None, degree_pol=4, n_gauss=0, center=[],
                     sigma=[], amplitude=[],
-                    plot_final=True, print_results=True, y_lim=[0,1.1], x_lim=[3,70]):
+                    plot_final=True, ylabel = 'PF', print_results=True, y_lim=[0,1.1], x_lim=[3,70]):
     '''
     this function will fit an input energy range of the pulse profile.
     the fitting function will be a simple polynomial + gaussian
     the aim is to retrieve basic gaussian parameters to be compared
     to those obtained in spectral analysis around Ecycl.
      output files: 1. the fit result
                    2. the fit results to be plotted in a file
@@ -1371,14 +1373,15 @@
     :param degree_pol: degree of the polynomial to fit
     :param n_gauss: number of gaussian lines
     :param center: array of centers of gaussians [[initial_value, min, max]]
     :param sigma: array of sigmas of gaussians [[initial_value, min, max]]
     :param amplitude: array of amplitude of gaussians [[initial_value, min, max]],
                         use negative values for absorption-like
     :param plot_final: if make a final plot
+    :param ylabel: ylabel for the plot (defaults to 'PF')
     :param print_results: if results should be printed out in file
     :return:
     '''
     from matplotlib.pyplot import cm
     from lmfit.models import PolynomialModel, GaussianModel
 
     if len(center) != n_gauss or len(sigma) != n_gauss or len (amplitude) != n_gauss:
@@ -1420,27 +1423,27 @@
 
     if not plot_final:
         fig, axes = plt.subplots(1, 2, figsize=(8.8, 4.8))
         axes[0].errorbar(en, pf, xerr=den, yerr=dpf, fmt='.', color=col[0])
         axes[0].plot(en, out.best_fit, '-', label='best fit', color=col[2])
         axes[0].legend(loc='upper left')
         axes[0].set_xlabel('E [keV]')
-        axes[0].set_ylabel('PF')
+        axes[0].set_ylabel(ylabel)
         axes[0].set_ylim(y_lim)
         axes[0].set_xlim(x_lim)
         
 
         axes[1].errorbar(en, pf, xerr=den, yerr=dpf, fmt='.', color=col[0])
         for N in range(1, n_gauss+1):
             axes[1].plot(en, comps['g%d_' % N], '--', label='Gaussian %d' % N, color=col[3])
             axes[1].axvline(center[N - 1][0], 0, 1, linestyle='--', color='cyan')
         axes[1].plot(en, comps['poly_'], '--', label='Polynomial component', color=col[4])
         axes[1].legend(loc='upper left')
         axes[1].set_xlabel('E [keV]')
-        axes[1].set_ylabel('PF')
+        axes[1].set_ylabel(ylabel)
         axes[1].set_ylim(y_lim)
         axes[1].set_xlim(x_lim)
         
         plt.savefig(stem + 'fit_results.pdf')
 
     #Is it of any use maybe to remove?
     if print_results:
@@ -1462,15 +1465,15 @@
                                        )
         ax1.errorbar(en, pf, xerr=den, yerr=dpf, fmt='.', color=col[4], label='data')
         ax1.plot(en, out.best_fit, '-', label='best fit', color=col[0])
         ax1.plot(en, comps['poly_'], '--', label='Polynomial', color=col[1])
         ax1.legend(loc='upper left')
         ax1.set_xscale('log')
         ax2.set_xlabel('E (keV)')
-        ax1.set_ylabel('PF')
+        ax1.set_ylabel(ylabel)
         ax1.set_ylim(y_lim)
         ax1.set_xlim(x_lim)
         for N in range(1, n_gauss+1):
             ax1.axvline(center[N - 1][0], 0, 1, linestyle='--', color='cyan')
         
         ax2.set_ylabel('Residuals')
         #ax1.set_ylim(-0.1, 1)
@@ -1529,16 +1532,16 @@
     if pars ==[]:
         pars = model_fitted.params.copy()
 
     explore = model_fitted.emcee(params=pars, steps=hm_steps, nwalkers=hm_walkers,
                                 is_weighted=True, burn=hm_jump)
     if plot_corner:
         emcee_plot = corner.corner(explore.flatchain, labels=explore.var_names, show_titles=True,
-                                   plot_datapoints=True)
-        emcee_plot.savefig(stem+'_corner.png')
+                                   plot_datapoints=True,figsize = (16,16))
+        emcee_plot.savefig(stem+'_corner.pdf')
 
     highest_prob = np.argmax(explore.lnprob)
     hp_loc = np.unravel_index(highest_prob, explore.lnprob.shape)
     mle_soln = explore.chain[hp_loc]
 
     pars2 = {}
     for el in pars.keys():
@@ -1675,22 +1678,24 @@
         y = np.real(ifft)
         #Necessary to avoid infinite for zero uncertaity
         ind = dx > 0
         #print(ind)
         chi2_val = np.sum(((x[ind] - y[ind]) / dx[ind]) ** 2)
         dof = max(1, n - (1 + 2 * (n_harm - 1)))
         chi2_sf = chi2.sf(chi2_val, dof)
-        # print(chi2_val, dof)
+        logger.debug(chi2_val, chi2_sf, dof, n_harm)
         # print(chi2_sf, old_chi2_sf)
         #Sometimes, we do ot reach the required level, but we cannot describe the pulse significantly better,
         # so we stop in any case (condition chi2_sf < old_chi2_sf)
         if chi2_sf > level or (chi2_sf < old_chi2_sf and chi2_sf > level/100.):
-            logger.debug('chi2_sf = %e (level is %.2f) old_chi2_sf = %e' % (chi2_sf, level, old_chi2_sf))
+            logger.debug('chi2_sf = %e (level is %.5f) old_chi2_sf = %e' % (chi2_sf, level, old_chi2_sf))
             break
         old_chi2_sf = chi2_sf
+        if n_harm == n_harm_max:
+            logger.info('maximum number of harmonics reached')
 
     logger.debug("Used %d harmonics for pulse description" % n_harm)
     
     a = np.absolute(fft) / n
 
     if background is not None and background_error is not None:
         a[0] = subtract_background(a[0], background,background_error)
```

### Comparing `nustarpipeline-0.2.5/nustarpipeline.egg-info/PKG-INFO` & `nustarpipeline-0.2.6/nustarpipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nustarpipeline
-Version: 0.2.5
+Version: 0.2.6
 Summary: nustar-pipeline
 Home-page: https://gitlab.astro.unige.ch/ferrigno/nustar-pipeline
 Author: C.F.
 Author-email: carlo.ferrigno@unige.ch
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `nustarpipeline-0.2.5/setup.cfg` & `nustarpipeline-0.2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.5
+current_version = 0.2.6
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

