# Comparing `tmp/cellmap-1.0.1.dev202304271055-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304280314-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1393806 bytes, number of entries: 6
+Zip file size: 1393868 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    85706 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304271055.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304271055.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304271055.dist-info/RECORD
-6 files, 4535102 bytes uncompressed, 1392920 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    85929 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304280314.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304280314.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304280314.dist-info/RECORD
+6 files, 4535325 bytes uncompressed, 1392982 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304271055.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304280314.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304271055.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304280314.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304271055.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304280314.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1536,14 +1536,17 @@
     genes,
     path_key = 'path',
     exp_key = None,
     gene_dynamics_key = 'gene_dynamics',
     fontsize_title = 16,
     fontsize_label = 14,
     fontsize_legend = 12,
+    save = False,
+    save_dir = None,
+    save_filename = 'gene_dynamics_plot',
 ):
     
     # kwargs_arg = check_arguments(adata, verbose=True)
 
     if gene_dynamics_key not in adata.uns.keys():
         gene_dynamics(adata, source_cluster,target_clusters,path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=100)
 
@@ -1589,27 +1592,30 @@
         n_div = 100,
         fontsize_label = 14,
         fontsize_text = 12,
         fontsize_nDEG = 18,
         fontsize_legend = 10,
         DEG_min = 1.0,
         DEG_rate = 0.3,
-        save_dir = None,
         save_type = 'gif',
         adjusttext = True,
         max_num_annotations = 10,
         max_num_legend = 40,
+        save = False,
+        save_dir = None,
+        save_filename = 'gene_dynamics_DEG',
     ):
 
     if gene_dynamics_key not in adata.uns.keys():
         gene_dynamics(adata, source_cluster,target_clusters,path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=100)
 
     n_plot_ = int(len(target_clusters)*(len(target_clusters)-1)/2)
     cmap_ = plt.get_cmap("tab10")
     gene_dynamics_ = adata.uns[gene_dynamics_key]
+    matplotlib.rcParams['animation.embed_limit'] = 2**128
     # def update(t,name_i_,name_j_,max_val_,lim,i,j,k):
     #     print('\rcomputing %s vs %s (%d/%d) %d/%d' % (target_clusters[i],target_clusters[j],k,n_plot_,t+1,n_div),end='')
     #     idx_DEG_i_ = np.arange(adata.shape[1])[(gene_dynamics_[name_j_][t] < gene_dynamics_[name_i_][t] - DEG_rate) & (gene_dynamics_[name_i_][t] > DEG_min)]
     #     idx_DEG_j_ = np.arange(adata.shape[1])[(gene_dynamics_[name_i_][t] < gene_dynamics_[name_j_][t] - DEG_rate) & (gene_dynamics_[name_j_][t] > DEG_min)]
     #     if len(idx_DEG_i_) > max_num_annotations:
     #         idx_DEG_top_i_ = idx_DEG_i_[np.argsort(gene_dynamics_[name_i_][t][idx_DEG_i_]- DEG_rate - gene_dynamics_[name_j_][t][idx_DEG_i_])[::-1][:max_num_annotations]]
     #     else:
@@ -1713,20 +1719,20 @@
             name_i_ = source_cluster+'_'+target_clusters[i]
             name_j_ = source_cluster+'_'+target_clusters[j]
             fig,ax = plt.subplots(1,2,figsize=(14,8),gridspec_kw={'width_ratios': [4,3]},tight_layout=True)
             max_val_ = max(np.max(gene_dynamics_[name_i_]),np.max(gene_dynamics_[name_j_]))
             lim = np.array([-0.01*max_val_,1.01*max_val_])
             k = k+1
             ani = anm.FuncAnimation(fig,update,interval=200,fargs=(name_i_,name_j_,max_val_,lim,i,j,k,),frames=n_div+1)
-            file_name = 'DEG_anoime_%s_%s' % (target_clusters[i],target_clusters[j]) if save_dir == None else '%s/DEG_anoime_%s_%s' % (save_dir,target_clusters[i],target_clusters[j])
             if len(target_genes): file_name += '_TG' + str(len(target_genes))
-            file_name += '.gif'
             IPython.display.display(IPython.display.HTML(ani.to_jshtml()))
             print('\nSaving gif animation as %s' % file_name)
-            ani.save(file_name)
+            if save:
+                file_name = '%s_%s_%s.gif' % (save_filename,target_clusters[i],target_clusters[j]) if save_dir == None else '%s/%s_%s_%s.gif' % (save_dir,save_filename,target_clusters[i],target_clusters[j])
+                ani.save(file_name)
             plt.close()
 
 def bifurcation_diagram(
         adata,
         source_cluster,
         target_clusters,
         path_key = 'path',
```

## Comparing `cellmap-1.0.1.dev202304271055.dist-info/METADATA` & `cellmap-1.0.1.dev202304280314.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304271055
+Version: 1.0.1.dev202304280314
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

