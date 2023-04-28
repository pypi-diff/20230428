# Comparing `tmp/cellmap-1.0.1.dev202304280314-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304280337-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1393868 bytes, number of entries: 6
+Zip file size: 1394003 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    85929 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304280314.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304280314.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304280314.dist-info/RECORD
-6 files, 4535325 bytes uncompressed, 1392982 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    86505 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304280337.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304280337.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304280337.dist-info/RECORD
+6 files, 4535901 bytes uncompressed, 1393117 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304280314.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304280337.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304280314.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304280337.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304280314.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304280337.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1557,29 +1557,41 @@
         data_exp = adata.layers[exp_key]
     path = adata.uns[path_key]
     cmap_ = plt.get_cmap("tab10")
 
     for gene in genes:
         if gene in adata.var.index:
             fig = plt.figure(figsize=(10,6))
+            y_data_all = []
             for i in range(len(target_clusters)):
                 name_ = source_cluster+'_'+target_clusters[i]
                 x_data,y_data = np.empty(0,dtype=float),np.empty(0,dtype=float)
                 for pi in path[name_]:
-                    x_data = np.append(x_data,np.linspace(0,1,len(pi)))
-                    y_data = np.append(y_data,data_exp[:,adata.var.index==gene][pi])
-                plt.scatter(x_data, y_data,color=cmap_(i),alpha=0.05,zorder=0)
+                    y_ = data_exp[:,adata.var.index==gene][pi].T[0]
+                    idx_ = y_>0
+                    x_data = np.append(x_data,np.linspace(0,1,len(pi))[idx_])
+                    y_data = np.append(y_data,y_[idx_])
+                if len(y_data):
+                    plt.scatter(x_data, y_data,color=cmap_(i),alpha=0.05,zorder=0)
                 dynamics_ = adata.uns[gene_dynamics_key][name_][:,adata.var.index==gene]
                 plot_x = np.linspace(0,1,len(dynamics_))
+                dynamics_[dynamics_ < 0] = 0
                 plt.plot(plot_x, dynamics_,color='w',lw=8,zorder=1)
                 plt.plot(plot_x, dynamics_,color=cmap_(i),lw=5,label=target_clusters[i],zorder=2)
+                y_data_all = np.append(y_data_all,y_data)
+            y_top_ = np.percentile(y_data_all,99)
+            plt.ylim([-0.05*y_top_,y_top_])
             plt.legend(bbox_to_anchor=(1.05, 0.5), loc='center left', borderaxespad=0,title='Target', fontsize=fontsize_legend, title_fontsize=fontsize_legend)
             plt.xticks([0,0.25,0.5,0.75,1],['Source (0)\n(%s)' % source_cluster,'0.25','0.5','0.75','Target (1)'],fontsize=fontsize_label)
             plt.title(gene,fontsize=fontsize_title)
             plt.show()
+            if save:
+                filename = '%s_%s' % (save_filename,gene) if save_dir == None else '%s/%s_%s' % (save_dir,save_filename,gene)
+                fig.savefig(filename+'.png', bbox_inches='tight')
+            plt.close()
         else:
             print('Gene \"%s\" was not found' % gene)
 
 
 
 def gene_dynamics_DEG(
         adata,
@@ -1721,18 +1733,18 @@
             fig,ax = plt.subplots(1,2,figsize=(14,8),gridspec_kw={'width_ratios': [4,3]},tight_layout=True)
             max_val_ = max(np.max(gene_dynamics_[name_i_]),np.max(gene_dynamics_[name_j_]))
             lim = np.array([-0.01*max_val_,1.01*max_val_])
             k = k+1
             ani = anm.FuncAnimation(fig,update,interval=200,fargs=(name_i_,name_j_,max_val_,lim,i,j,k,),frames=n_div+1)
             if len(target_genes): file_name += '_TG' + str(len(target_genes))
             IPython.display.display(IPython.display.HTML(ani.to_jshtml()))
-            print('\nSaving gif animation as %s' % file_name)
             if save:
-                file_name = '%s_%s_%s.gif' % (save_filename,target_clusters[i],target_clusters[j]) if save_dir == None else '%s/%s_%s_%s.gif' % (save_dir,save_filename,target_clusters[i],target_clusters[j])
-                ani.save(file_name)
+                filename = '%s_%s_%s.gif' % (save_filename,target_clusters[i],target_clusters[j]) if save_dir == None else '%s/%s_%s_%s.gif' % (save_dir,save_filename,target_clusters[i],target_clusters[j])
+                print('\nSaving gif animation as %s' % filename)
+                ani.save(filename)
             plt.close()
 
 def bifurcation_diagram(
         adata,
         source_cluster,
         target_clusters,
         path_key = 'path',
```

## Comparing `cellmap-1.0.1.dev202304280314.dist-info/METADATA` & `cellmap-1.0.1.dev202304280337.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304280314
+Version: 1.0.1.dev202304280337
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

