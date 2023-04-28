# Comparing `tmp/cellmap-1.0.1.dev202304280337-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304281103-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1394003 bytes, number of entries: 6
+Zip file size: 1395164 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    86505 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304280337.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304280337.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304280337.dist-info/RECORD
-6 files, 4535901 bytes uncompressed, 1393117 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    91233 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304281103.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304281103.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304281103.dist-info/RECORD
+6 files, 4540629 bytes uncompressed, 1394278 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304280337.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304281103.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304280337.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304281103.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304280337.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304281103.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -10,57 +10,34 @@
 import matplotlib.animation as anm
 from matplotlib import patheffects as PathEffects
 import networkx as nx
 import scanpy
 import scipy
 import scvelo as scv
 import sklearn.preprocessing
+import sklearn.mixture
 import sklearn.neighbors
 from sklearn.linear_model import LinearRegression
 from sklearn.preprocessing import PolynomialFeatures
 import pandas as pd
 import plotly.graph_objects as go
-from plotly.offline import plot
+import plotly.io as pio
+import plotly.offline
+import umap
 
 
 
 
 def create_graph(
     X,
     cutedge_vol = None,
     cutedge_length = None,
     cut_std = None,
     return_type = 'edges',
 ):
-    # tri_ = matplotlib.tri.Triangulation(X[:,0],X[:,1])
-    # X_src_,X_trg_ = X[tri_.edges[:,0]],X[tri_.edges[:,1]]
-    # length_edge_ = np.linalg.norm(X_src_-X_trg_,axis=1)
-    # x1,y1 = X[tri_.triangles[:,0],0],X[tri_.triangles[:,0],1]
-    # x2,y2 = X[tri_.triangles[:,1],0],X[tri_.triangles[:,1],1]
-    # x3,y3 = X[tri_.triangles[:,2],0],X[tri_.triangles[:,2],1]
-    # vol_ = np.abs((x1-x3)*(y2-y3)-(x2-x3)*(y1-y3))
-    # length_ = np.max([(x1-x2)**2+(y1-y2)**2,(x2-x3)**2+(y2-y3)**2,(x3-x1)**2+(y3-y1)**2],axis=0)
-    # if cut_std == None:
-    #     std_delta_ = 0.1
-    #     std_min_ = 1
-    #     cut_std = std_min_
-    #     while 1:
-    #         if len(np.unique(tri_.edges[length_edge_ < cut_std*np.std(length_edge_)].reshape(-1,1).T[0])) == X.shape[0]:
-    #             break
-    #         cut_std = cut_std + std_delta_
-    # if cutedge_vol == None:
-    #     judge_vol_tri_ = vol_ < cut_std*np.std(vol_)
-    # else:
-    #     judge_vol_tri_ = vol_ < np.percentile(vol_,100-cutedge_vol)
-    # if cutedge_length == None:
-    #     judge_length_edge_ = length_edge_ < cut_std*np.std(length_edge_)
-    #     judge_length_tri_= length_ < cut_std*np.std(length_)
-    # else:
-    #     judge_length_edge_ = length_edge_ < np.percentile(length_edge_,100-cutedge_length)
-    #     judge_length_tri_ = length_ < np.percentile(length_edge_,100-cutedge_length)#np.percentile(length_,100-cutedge_length)
     tri_ = matplotlib.tri.Triangulation(X[:,0],X[:,1])
     X_src_,X_trg_ = X[tri_.edges[:,0]],X[tri_.edges[:,1]]
     length_edge_ = np.linalg.norm(X_src_-X_trg_,axis=1)
     x1,y1 = X[tri_.triangles[:,0],0],X[tri_.triangles[:,0],1]
     x2,y2 = X[tri_.triangles[:,1],0],X[tri_.triangles[:,1],1]
     x3,y3 = X[tri_.triangles[:,2],0],X[tri_.triangles[:,2],1]
     vol_ = np.abs((x1-x3)*(y2-y3)-(x2-x3)*(y1-y3))
@@ -1035,15 +1012,15 @@
         )
         data = [surf]
         if show_cells: data.append(cells)
         if show_shadow: data.append(shadow)
         fig = go.Figure(data=data, layout=layout)
     fig.show()
     
-    if save: plot(fig, filename=filename+'.html')
+    if save: plotly.offline.plot(fig, filename=filename+'.html')
 
 def view_surface_3D(
     adata,
     basis = 'umap',
     potential_key = 'potential',
     graph_key = 'CellMap_graph',
     cluster_key = None,
@@ -1518,15 +1495,17 @@
 
         X = x_data[:, np.newaxis]
         poly = PolynomialFeatures(degree=10)
         X_poly = poly.fit_transform(X)
         model = LinearRegression()
         model.fit(X_poly, y_data)
         plot_x = np.linspace(0,1,n_div+1)
-        gene_dynamics_[source_cluster+'_'+target_clusters[i]] = model.predict(poly.fit_transform(plot_x[:, np.newaxis]))
+        gd_i_ = model.predict(poly.fit_transform(plot_x[:, np.newaxis]))
+        gd_i_[gd_i_ <0] = 0
+        gene_dynamics_[source_cluster+'_'+target_clusters[i]] = gd_i_
     adata.uns[gene_dynamics_key] = gene_dynamics_
     print('Done the computation of gene dynamics')
     
 
 
 
 def gene_dynamics_plot(
@@ -1731,18 +1710,19 @@
             name_i_ = source_cluster+'_'+target_clusters[i]
             name_j_ = source_cluster+'_'+target_clusters[j]
             fig,ax = plt.subplots(1,2,figsize=(14,8),gridspec_kw={'width_ratios': [4,3]},tight_layout=True)
             max_val_ = max(np.max(gene_dynamics_[name_i_]),np.max(gene_dynamics_[name_j_]))
             lim = np.array([-0.01*max_val_,1.01*max_val_])
             k = k+1
             ani = anm.FuncAnimation(fig,update,interval=200,fargs=(name_i_,name_j_,max_val_,lim,i,j,k,),frames=n_div+1)
-            if len(target_genes): file_name += '_TG' + str(len(target_genes))
             IPython.display.display(IPython.display.HTML(ani.to_jshtml()))
             if save:
-                filename = '%s_%s_%s.gif' % (save_filename,target_clusters[i],target_clusters[j]) if save_dir == None else '%s/%s_%s_%s.gif' % (save_dir,save_filename,target_clusters[i],target_clusters[j])
+                filename = '%s_%s_%s' % (save_filename,target_clusters[i],target_clusters[j]) if save_dir == None else '%s/%s_%s_%s' % (save_dir,save_filename,target_clusters[i],target_clusters[j])
+                if len(target_genes): filename += '_TG' + str(len(target_genes))
+                filename += '.gif'
                 print('\nSaving gif animation as %s' % filename)
                 ani.save(filename)
             plt.close()
 
 def bifurcation_diagram(
         adata,
         source_cluster,
@@ -1790,8 +1770,187 @@
     ax.spines['left'].set_visible(False)
     ax.spines['top'].set_visible(False)
     ax.spines['bottom'].set_visible(False)
     ax.xaxis.set_label_position('top')
     ax.xaxis.tick_top()
     ax.yaxis.set_visible(False)
     ax.set_xticks(vlines)
-    ax.set_xticklabels(vline_labels,fontsize=fontsize_label)
+    ax.set_xticklabels(vline_labels,fontsize=fontsize_label)
+
+def gene_atlas(
+        adata,
+        source_cluster,
+        target_clusters,
+        target_genes = [],
+        gene_dynamics_key = 'gene_dynamics',
+        n_div = 100,
+        n_neighbors = 15,
+        min_dist = 0.3,
+        seed = 0,
+        threshold_min = 1,
+        n_clusters = 20,
+        n_components = 2,
+        pt_size = 5,
+    ):
+    gene_dynamics_ = adata.uns[gene_dynamics_key]
+
+    gene_dynamics_all_ = np.empty([0,n_div+1],dtype=float)
+    idx_gene_dynamics_ = [0]
+    for i in range(len(target_clusters)):
+        name_i_ = source_cluster + '_' + target_clusters[i]
+        max_ = np.max(gene_dynamics_[name_i_],axis=0)
+        idx_ = max_ > threshold_min
+        adata.var[name_i_+'_'+'expressed'] = idx_
+        idx_gene_dynamics_ = np.append(idx_gene_dynamics_,idx_gene_dynamics_[i]+sum(idx_))
+        gene_dynamics_all_ = np.vstack((gene_dynamics_all_,(gene_dynamics_[name_i_][:,idx_]/max_[idx_]).T))
+
+
+    umap_ = umap.UMAP(n_components=n_components,random_state=seed,n_neighbors=n_neighbors,min_dist=min_dist)
+    gene_dynamics_all_umap_ = umap_.fit_transform(gene_dynamics_all_)
+
+    data_ = gene_dynamics_all_umap_
+    gm = sklearn.mixture.GaussianMixture(n_components=n_clusters,random_state=0).fit(data_)
+    clusters_tmp_ = gm.predict(data_)
+    pc1_ = sklearn.decomposition.PCA(n_components=1).fit_transform(data_)
+    pc1_order_ = np.argsort([np.mean(pc1_[clusters_tmp_==i]) for i in range(n_clusters)])
+    dict_sort_ = dict(zip(pc1_order_,np.unique(clusters_tmp_)))
+    clusters_ = np.array([dict_sort_[c] for c in clusters_tmp_])
+    cluster_set_ = np.unique(clusters_)
+
+    x_data = gene_dynamics_all_umap_[:,0]
+    y_data = gene_dynamics_all_umap_[:,1]
+
+    color_clusters_ = np.array(['rgb'+str(tuple(int(i *255) for i in plt.get_cmap("tab20")(c))) for c in clusters_])
+    color_celltypes_ = np.empty(len(gene_dynamics_all_),dtype=object)
+
+    texts_ = []
+    s_,e_ = 0,0
+    annotations = [
+        go.layout.Annotation(
+            xref='paper',
+            yref='paper',
+            x=0.01,
+            y=0.99,
+            text='<b>Gene Atlas<b>',
+            font=dict(size=18,color='white'),
+            showarrow=False,
+        )
+    ]
+    for i in range(len(target_clusters)):
+        idx_ = adata.var[source_cluster + '_' + target_clusters[i]+'_'+'expressed']
+        gene_list_ = adata.var.index[idx_].values
+        e_ += sum(idx_)
+        color_celltypes_[s_:e_] = 'rgba'+str(plt.get_cmap("tab10")(i))
+        txt_ = gene_list_ + '<br>' + target_clusters[i]+'<br>cluster '+ np.array(clusters_[s_:e_]+1,dtype=str)#+ '<br><img src="'+image_+'" width="200">'
+        texts_= np.append(texts_,txt_)
+        for gene in target_genes:
+            if gene in gene_list_:
+                x_pos = x_data[np.arange(sum(idx_))[gene_list_==gene][0]+s_]
+                y_pos = y_data[np.arange(sum(idx_))[gene_list_==gene][0]+s_]
+                annotations.append(
+                    go.layout.Annotation(
+                        x=x_pos,
+                        y=y_pos,
+                        xref='x',
+                        yref='y',
+                        text='<b>%s_%s<b>' % (target_clusters[i],gene),
+                        showarrow=True,
+                        arrowhead=1,
+                        arrowcolor='white',
+                        font=dict(size=12,color='white'),
+                    )
+                )
+        s_ += sum(idx_)
+
+    data_clusters_ = [
+        go.Scatter(
+            x=x_data,
+            y=y_data,
+            mode='markers',
+            marker=dict(
+                color=color_clusters_,
+                size=30,
+                opacity=0.2,
+            ),
+            hoverinfo='skip',
+            showlegend=False,
+        )
+    ]
+    for c in cluster_set_:
+        idx_ = clusters_ ==c
+        data_clusters_.append(
+            go.Scatter(
+                x=x_data[idx_],
+                y=y_data[idx_],
+                text = texts_[idx_],
+                mode='markers',
+                name='cluster '+str(c+1),
+                marker=dict(
+                    color='rgb'+str(tuple(int(i*255) for i in plt.get_cmap("tab20")(c))),
+                    size=pt_size,
+                    opacity=1,
+                    line=dict(
+                        color='white',
+                        width=0.5,
+                    ),
+                ),
+            )
+        )
+
+    s_,e_ = 0,0
+    data_celltypes_ = []
+    for i in range(len(target_clusters)):
+        idx_ = adata.var[source_cluster + '_' + target_clusters[i]+'_'+'expressed']
+        gene_list_ = adata.var.index[idx_].values
+        e_ += sum(idx_)
+        data_celltypes_.append(
+            go.Scatter(
+                x=x_data[s_:e_],
+                y=y_data[s_:e_],
+                text = texts_[s_:e_],
+                mode='markers',
+                name=target_clusters[i],
+                marker=dict(
+                    color=color_celltypes_[s_:e_],
+                    size=pt_size,
+                    opacity=1,
+                    line=dict(
+                        color='white',
+                        width=0.5,
+                    ),
+                )
+            )
+        )
+        s_ += sum(idx_)
+
+
+    layout = go.Layout(
+        width=1200,
+        height=800,
+        plot_bgcolor='rgba(1,1,1,1)',
+        paper_bgcolor='rgba(0,0,0,0)',
+        xaxis=dict(
+            # showgrid=False,
+            gridcolor='gray',
+            gridwidth=1,
+            griddash='dot',
+            zeroline=False,
+            showticklabels=False,
+            layer='below traces',
+        ),
+        yaxis=dict(
+            # showgrid=False,
+            gridcolor='gray',
+            gridwidth=1,
+            griddash='dot',
+            zeroline=False,
+            showticklabels=False,
+            layer='below traces',
+        ),
+        annotations=annotations
+    )
+
+    fig = go.Figure(data=data_clusters_, layout=layout)
+    pio.show(fig)
+
+    fig = go.Figure(data=data_celltypes_, layout=layout)
+    pio.show(fig)
```

## Comparing `cellmap-1.0.1.dev202304280337.dist-info/METADATA` & `cellmap-1.0.1.dev202304281103.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304280337
+Version: 1.0.1.dev202304281103
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

