# Comparing `tmp/inviz-0.0.5.tar.gz` & `tmp/inviz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.0.5.tar", last modified: Tue Apr 11 23:59:16 2023, max compression
+gzip compressed data, was "inviz-0.0.6.tar", last modified: Thu Apr 27 23:22:14 2023, max compression
```

## Comparing `inviz-0.0.5.tar` & `inviz-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-11 23:59:16.950293 inviz-0.0.5/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-04-11 23:56:04.000000 inviz-0.0.5/LICENSE
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-04-11 23:56:04.000000 inviz-0.0.5/MANIFEST.in
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     4045 2023-04-11 23:59:16.950293 inviz-0.0.5/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     3475 2023-04-11 23:56:04.000000 inviz-0.0.5/README.md
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-11 23:59:16.950293 inviz-0.0.5/inviz/
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-11 23:59:16.950293 inviz-0.0.5/inviz/inviz.egg-info/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     4045 2023-04-11 23:59:16.000000 inviz-0.0.5/inviz/inviz.egg-info/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      227 2023-04-11 23:59:16.000000 inviz-0.0.5/inviz/inviz.egg-info/SOURCES.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-04-11 23:59:16.000000 inviz-0.0.5/inviz/inviz.egg-info/dependency_links.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       98 2023-04-11 23:59:16.000000 inviz-0.0.5/inviz/inviz.egg-info/requires.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-04-11 23:59:16.000000 inviz-0.0.5/inviz/inviz.egg-info/top_level.txt
--rwxrwxr-x   0 maamari   (1000) maamari   (1000)     9933 2023-04-11 23:56:05.000000 inviz-0.0.5/inviz/inviz.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-04-11 23:59:16.950293 inviz-0.0.5/setup.cfg
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1162 2023-04-11 23:58:38.000000 inviz-0.0.5/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-27 23:22:14.106627 inviz-0.0.6/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-04-27 23:20:02.000000 inviz-0.0.6/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-04-27 23:20:02.000000 inviz-0.0.6/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1910 2023-04-27 23:22:14.106627 inviz-0.0.6/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1359 2023-04-27 23:20:02.000000 inviz-0.0.6/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-27 23:22:14.096627 inviz-0.0.6/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-27 23:22:14.106627 inviz-0.0.6/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1910 2023-04-27 23:22:14.000000 inviz-0.0.6/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-04-27 23:22:14.000000 inviz-0.0.6/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-04-27 23:22:14.000000 inviz-0.0.6/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       39 2023-04-27 23:22:14.000000 inviz-0.0.6/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-04-27 23:22:14.000000 inviz-0.0.6/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)     8826 2023-04-27 23:20:03.000000 inviz-0.0.6/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-04-27 23:22:14.106627 inviz-0.0.6/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1127 2023-04-27 23:20:03.000000 inviz-0.0.6/setup.py
```

### Comparing `inviz-0.0.5/LICENSE` & `inviz-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.0.5/inviz/inviz.py` & `inviz-0.0.6/inviz/inviz.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,98 +10,137 @@
 import panel as pn
 import spatialpandas
 import os
 from bokeh.models import HoverTool
 from classy import Class
 import matplotlib.pyplot as plt
 import copy
+from multiprocessing import Pool
 
 hv.extension('bokeh')
-hv.Store.set_current_backend('bokeh')
-pn.extension('tabulator')
-pn.extension(loading_spinner='dots', loading_color='#00aa41', sizing_mode="stretch_width")
+# hv.Store.set_current_backend('bokeh')
+# pn.extension('tabulator')
 pn.extension()
 
 # read in the .paramnames file and put it into list format
 def load_params(filename):
     params_list = []
     with open(filename, 'r') as f:
         for line in f:
             line = line.strip()
             params = re.split(' \t ', line)
             params_list.append(params)
-    return [item[0] for item in params_list]
+    return [item[0] for item in params_list], [item[1] for item in params_list]
 
 
 # create a DataFrame with the chain files as rows and use a list of parameters as the column names
 def load_data(filename, column_names):
     data = np.loadtxt(filename)
-    df = pd.DataFrame(data[:,2:], columns=column_names)
+    df = pd.DataFrame(data[:,1:], columns=column_names)
     return df
 
 
+def run_class(selection):
+    # run class on the user's selection
+    cosmo = Class()
+    cosmo.set(selection)
+    cosmo.set({'output':'mPk, tCl, pCl, lCl','P_k_max_1/Mpc':3.0, 'lensing':'yes'})
+    cosmo.compute()
+
+    # set variables for matter power spectrum and lensed CMB angular power spectra
+    kk = np.logspace(-4,np.log10(3),1000)
+    Pk = []
+    h = cosmo.h()
+    for k in kk:
+        Pk.append(cosmo.pk(k*h,0.)*h**3)
+    Pk = np.array(Pk)
+    l = np.array(range(2,2501))
+    factor = l*(l+1)/(2*np.pi)
+    lensed_cl = cosmo.lensed_cl(2500)
+    
+    results = {'k': kk, 'Pk': Pk, 'l': l, 'Cl_tt': factor*lensed_cl['tt'][2:], 'Cl_ee': factor*lensed_cl['ee'][2:]}
+    return results
+
+
 # generate a scatter plot using the key dimensions from a holoviews.Dataset object, with the CLASS output displayed alongside it
-def viz(data, data_classy_input, data_classy_CDM, class_enabled):
+def viz(data, data_classy_input, data_classy_CDM, class_enabled=True, latex_dict=None):
+    # handle default case of no latex paramname dictionary
+    if latex_dict is None:
+        latex_dict = dict()
+    # setting Panel widgets for user interaction
+    variables = data.columns.values.tolist()
+    var1 = pn.widgets.Select(value=variables[0], name='Horizontal Axis', options=variables)
+    var2 = pn.widgets.Select(value=variables[1], name='Vertical Axis', options=variables)
+    cmap_var = pn.widgets.Select(value=variables[2], name='Colormapped Parameter', options=variables)
+    cmap_option = pn.widgets.Checkbox(value=True, name='Show Colormap', align='end')
+    
+    #  given a param name, find corresponding latex-formatted param name
+    def lookup_latex_label(param):
+        try:
+            latex_param = latex_dict[param]
+            label = r'$${}$$'.format(latex_param)
+            return label
+        except KeyError:
+            label = param
+            return label
+    
     # function for generating the scatter plot, given 2 dimensions as x and y axes, and an additional dimension to colormap
     # to the points on the plot. Also has an option to show or hide the colormap
     def plot_data(kdim1, kdim2, colordim, showcmap):
         if showcmap == True:
             cmapping = opts.Points(color=dim(colordim),
                 colorbar=True,
                 cmap='Viridis')
         else:
             cmapping = opts.Points(color='grey', colorbar=True)
         hover = HoverTool(tooltips=None)
+        xlabel = lookup_latex_label(kdim1)
+        ylabel = lookup_latex_label(kdim2)
         popts = opts.Points(
+            fontscale=1.1,
+            xlabel=xlabel,
+            ylabel=ylabel,
             toolbar='above',
-            #line_color='black',
+            line_color='black',
             #alpha=0.75, selection_alpha=1, nonselection_alpha=0.1,
             tools=[hover, 'box_select','lasso_select','tap'],
             size=7)
         points = hv.Points(data, kdims=[kdim1, kdim2]).opts(popts, cmapping)
         return points
     
-    
-    # setting Panel widgets for user interaction
-    variables = data.columns.values.tolist()
-    var1 = pn.widgets.Select(value=variables[0], name='Horizontal Axis', options=variables)
-    var2 = pn.widgets.Select(value=variables[1], name='Vertical Axis', options=variables)
-    cmap_var = pn.widgets.Select(value=variables[2], name='Colormapped Parameter', options=variables)
-    cmap_option = pn.widgets.Checkbox(value=True, name='Show Colormap', align='end')
-    
     # bind the widget values to the plotting function so it gets called every time the user interacts with the widget
     # call the bound plotting function inside a holoview DynamicMap object for interaction
     interactive_points = pn.bind(plot_data, kdim1=var1, kdim2=var2, colordim=cmap_var, showcmap=cmap_option)
     points_dmap = hv.DynamicMap(interactive_points, kdims=[]).opts(width=500, height=400, framewise=True)
     
     # define a stream to get a list of all the points the user has selected on the plot
     selection = streams.Selection1D(source=points_dmap)
     
+    # formatting the table using plot hooks
+    def hook(plot, element):
+        plot.handles['table'].autosize_mode = "none"
+        for column in plot.handles['table'].columns:
+            column.width = 100
+    
     # function to generate a table of all the selected points
     def make_table(kdim1, kdim2, colordim):
-        table = hv.DynamicMap(lambda index: hv.Table(data.iloc[index], kdims=[kdim1, kdim2, colordim]), streams=[selection])
-        # formatting the table using plot hooks and a holoviews Options object
-        def hook(plot, element):
-            plot.handles['table'].autosize_mode = "none"
-            for column in plot.handles['table'].columns:
-                column.width = 100
-            
         table_options = opts.Table(height=300, width=1000, hooks=[hook])
+        table = hv.DynamicMap(lambda index: hv.Table(data.iloc[index], kdims=[kdim1, kdim2, colordim]), streams=[selection])
         return table.opts(table_options).relabel('Selected Points')
     
     
     # generate the table
     selected_table = pn.bind(make_table, kdim1=var1, kdim2=var2, colordim=cmap_var)
     
     #table_stream = streams.Selection1D(source=selected_table)
     
     # function to run CLASS on data from the selection. 
     # first create an empty plot to handle the null selection case
     empty_plot = hv.Curve(np.random.rand(0, 2))
-    def run_class_on_selection(index):
+    def plot_class_results(index):
         if not index:
             empty_pk = empty_plot.relabel('P(k) Residuals - no selection').opts(
                 xlabel=r'$$k~[h/\mathrm{Mpc}]$$', 
                 ylabel=r'$$(P(k)-P_{CDM}(k))/P_{CDM}(k)*100~[\%]$$')
             empty_cl_tt = empty_plot.relabel('Lensed Cl_TT Residuals - no selection').opts(
                 xlabel=r"$$\ell$$", 
                 ylabel=r"$$(C_{\ell}^{TT} - C_{\ell, CDM}^{TT})/C_{\ell, CDM}^{TT}*100~[\%]$$")
@@ -113,90 +152,44 @@
 
         # the Selection1D stream returns an index number. index into the approprate dataframe and turn it into a dictionary for CLASS to read
         selection = data_classy_input.iloc[index]
         selection_CDM = data_classy_CDM.iloc[index]
         sel_dict_list = selection.to_dict('records')
         CDM_dict_list = selection_CDM.to_dict('records')
         
-        # remove nuisance parameters and add some project-specific ones. in the future these will be defined by the user
-#         for i in range(len(sel_dict_list)):
-#             entries_to_remove1 = ('z_reio', 'A_s', 'sigma8', '100theta_s', 'A_cib_217', 'xi_sz_cib', 'A_sz', 'ps_A_100_100', 'ps_A_143_143', 'ps_A_143_217', 'ps_A_217_217', 'ksz_norm', 
-#                                  'gal545_A_100', 'gal545_A_143', 'gal545_A_143_217', 'gal545_A_217', 'galf_TE_A_100', 'galf_TE_A_100_143', 'galf_TE_A_100_217', 'galf_TE_A_143', 'galf_TE_A_143_217', 
-#                                  'galf_TE_A_217', 'calib_100T', 'calib_217T', 'A_planck' )
-#             for j in entries_to_remove1:
-#                 sel_dict_list[i].pop(j, None)
-
-#             sel_dict_list[i]['omega_b'] = sel_dict_list[i]['omega_b']*1e-2
-#             sel_dict_list[i]['sigma_dmeff'] = sel_dict_list[i]['sigma_dmeff']*1e-25
-#             sel_dict_list[i]['h'] = (sel_dict_list[i].pop('H0'))*1e-2
-#             sel_dict_list[i].update({"omega_cdm":1e-15, "npow_dmeff": 0, "Vrel_dmeff": 0, "dmeff_target": "baryons", "m_dmeff": 1e-3})
-
-#         for k in range(len(sel_dict_list)):
-#             params_CDM = copy.deepcopy(sel_dict_list[k])
-#             entries_to_remove2 = ('sigma_dmeff', 'npow_dmeff', 'Vrel_dmeff', 'dmeff_target', 'm_dmeff')
-#             for l in entries_to_remove2:
-#                 params_CDM.pop(l, None)
-#             params_CDM['omega_cdm'] = params_CDM.pop('omega_dmeff')
-#             CDM_dict_list.append(params_CDM)
-
-        # run class on the user's selection
-        cosmo = Class()
-        cosmo.set(sel_dict_list[0])
-        cosmo.set({'output':'mPk, tCl, pCl, lCl','P_k_max_1/Mpc':3.0, 'lensing':'yes'})
-        cosmo.compute()
-
-        # set variables for matter power spectrum and lensed CMB angular power spectra
-        kk = np.logspace(-4,np.log10(3),1000)
-        Pk1 = []
-        h = cosmo.h()
-        for k in kk:
-            Pk1.append(cosmo.pk(k*h,0.)*h**3)
-
-        l = np.array(range(2,2501))
-        factor = l*(l+1)/(2*np.pi)
-        lensed_cl = cosmo.lensed_cl(2500)
-        
-        # run CLASS on the user's selection using the CDM model
-        cosmo_CDM = Class()
-        cosmo_CDM.set(CDM_dict_list[0])
-        cosmo_CDM.set({'output':'mPk, tCl, pCl, lCl','P_k_max_1/Mpc':3.0, 'lensing':'yes'})
-        cosmo_CDM.compute()
-
-        # set variables for CDM observables
-        Pk_CDM = []
-        h = cosmo_CDM.h()
-        for k in kk:
-            Pk_CDM.append(cosmo_CDM.pk(k*h,0.)*h**3)
-
-        lensed_cl_CDM = cosmo_CDM.lensed_cl(2500)
+        # compute stats for user's cosmology and LambdaCDM in parallel
+        if __name__ == '__main__':
+            with Pool() as p:
+                [mycosmo, LambdaCDM] = p.map(run_class, [sel_dict_list[0], CDM_dict_list[0]])
 
         # compute residuals
-        pk_residuals = (np.array(Pk1) - np.array(Pk_CDM))/np.array(Pk_CDM)*100
-        cl_tt_residuals = (lensed_cl['tt'][2:] - lensed_cl_CDM['tt'][2:])/(lensed_cl_CDM['tt'][2:])*100
-        cl_ee_residuals = (lensed_cl['ee'][2:] - lensed_cl_CDM['ee'][2:])/(lensed_cl_CDM['ee'][2:])*100
+        pk_residuals = (mycosmo['Pk'] - LambdaCDM['Pk'])/LambdaCDM['Pk']*100
+        cl_tt_residuals = (mycosmo['Cl_tt'] - LambdaCDM['Cl_tt'])/LambdaCDM['Cl_tt']*100
+        cl_ee_residuals = (mycosmo['Cl_ee'] - LambdaCDM['Cl_ee'])/LambdaCDM['Cl_ee']*100
 
-        plot_pk_residuals = hv.Curve((kk, pk_residuals)).relabel('P(k) Residuals').opts(
+        plot_pk_residuals = hv.Curve((mycosmo['k'], pk_residuals)).relabel('P(k) Residuals').opts(
             xlabel=r'$$k~[h/\mathrm{Mpc}]$$', 
             ylabel=r'$$(P(k)-P_{CDM}(k))/P_{CDM}(k)*100~[\%]$$')
 
-        plot_cl_tt_residuals = hv.Curve((l,cl_tt_residuals)).relabel('Cl_TT Residuals').opts(
+        plot_cl_tt_residuals = hv.Curve((mycosmo['l'],cl_tt_residuals)).relabel('Cl_TT Residuals').opts(
             xlabel=r"$$\ell$$", 
             ylabel=r"$$(C_{\ell}^{TT}-C_{\ell, CDM}^{TT})/C_{\ell, CDM}^{TT}*100~[\%]$$")
 
-        plot_cl_ee_residuals = hv.Curve((l,cl_ee_residuals)).relabel('Cl_EE Residuals').opts(
+        plot_cl_ee_residuals = hv.Curve((mycosmo['l'],cl_ee_residuals)).relabel('Cl_EE Residuals').opts(
             xlabel=r"$$\ell$$", 
             ylabel=r"$$(C_{\ell}^{EE}-C_{\ell, CDM}^{EE})/C_{\ell, CDM}^{EE}*100~[\%]$$")
         
         layout = (plot_pk_residuals + plot_cl_tt_residuals + plot_cl_ee_residuals)
         return layout
     
     # put it all together using Panel
     dashboard = pn.Column(pn.Row(var1, var2, cmap_var, cmap_option), pn.Row(points_dmap, selected_table))
-
+    
     if class_enabled == True:
-        classy_output = hv.DynamicMap(run_class_on_selection, streams=[selection]).opts(
+        classy_output = hv.DynamicMap(plot_class_results, streams=[selection]).opts(
             opts.Curve(color='black', logx=True, width=500, height=400, padding=0.1, framewise=True),
             opts.Layout(shared_axes=False))
         classy_output_pane = pn.panel(classy_output)
-        # pn.param.set_values(classy_output_pane, loading=True)
+        # pn.param.set_values(classy_output_pane, loading_indicator=True)
         dashboard = pn.Column(dashboard, classy_output_pane)
+    
     return dashboard
```

### Comparing `inviz-0.0.5/setup.py` & `inviz-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.0.5",
+    version = "0.0.6",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
@@ -22,14 +22,13 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
     python_requires='>=3.6',
     install_requires=["holoviews==1.15.4",
-                      "spatialpandas==0.4.7",
-                      "hvplot==0.8.3",
-                      "numpy==1.23.5",
-                      "matplotlib==3.7.1",
-                      "bokeh==2.4.0"]
+                    #   "bokeh==2.4.3",
+                      "spatialpandas==0.4.7"]
+                    #   "numpy<=1.24",
+                    #   "matplotlib==3.7.1"]
     )
```

