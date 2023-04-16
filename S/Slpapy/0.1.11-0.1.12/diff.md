# Comparing `tmp/Slpapy-0.1.11.tar.gz` & `tmp/Slpapy-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.1.11.tar", last modified: Fri Apr 14 08:19:47 2023, max compression
+gzip compressed data, was "Slpapy-0.1.12.tar", last modified: Sun Apr 16 10:52:03 2023, max compression
```

## Comparing `Slpapy-0.1.11.tar` & `Slpapy-0.1.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:19:47.753194 Slpapy-0.1.11/
--rw-rw-rw-   0        0        0      160 2023-04-14 08:19:47.752195 Slpapy-0.1.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 08:19:47.744194 Slpapy-0.1.11/Slpapy/
--rw-rw-rw-   0        0        0     1972 2023-04-14 08:19:22.000000 Slpapy-0.1.11/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.11/Slpapy/MZ_ppm_match.py
--rw-rw-rw-   0        0        0      525 2023-04-14 06:21:10.000000 Slpapy-0.1.11/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5164 2023-04-14 08:17:47.000000 Slpapy-0.1.11/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:19:47.751194 Slpapy-0.1.11/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-04-14 08:19:47.000000 Slpapy-0.1.11/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-14 08:19:47.000000 Slpapy-0.1.11/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:19:47.000000 Slpapy-0.1.11/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-14 08:19:47.000000 Slpapy-0.1.11/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 08:19:47.000000 Slpapy-0.1.11/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 08:19:47.753194 Slpapy-0.1.11/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-04-14 08:19:39.000000 Slpapy-0.1.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:52:03.903423 Slpapy-0.1.12/
+-rw-rw-rw-   0        0        0      160 2023-04-16 10:52:03.902424 Slpapy-0.1.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 10:52:03.890437 Slpapy-0.1.12/Slpapy/
+-rw-rw-rw-   0        0        0     1972 2023-04-14 08:19:22.000000 Slpapy-0.1.12/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.12/Slpapy/MZ_ppm_match.py
+-rw-rw-rw-   0        0        0      525 2023-04-14 06:21:10.000000 Slpapy-0.1.12/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5129 2023-04-16 10:50:55.000000 Slpapy-0.1.12/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:52:03.900424 Slpapy-0.1.12/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-04-16 10:52:03.000000 Slpapy-0.1.12/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-16 10:52:03.000000 Slpapy-0.1.12/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 10:52:03.000000 Slpapy-0.1.12/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-16 10:52:03.000000 Slpapy-0.1.12/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 10:52:03.000000 Slpapy-0.1.12/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 10:52:03.903423 Slpapy-0.1.12/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-04-15 13:30:30.000000 Slpapy-0.1.12/setup.py
```

### Comparing `Slpapy-0.1.11/Slpapy/Data_reconstruction.py` & `Slpapy-0.1.12/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.11/Slpapy/MZ_ppm_match.py` & `Slpapy-0.1.12/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.11/Slpapy/__init__.py` & `Slpapy-0.1.12/Slpapy/__init__.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.11/Slpapy/processing_analyze.py` & `Slpapy-0.1.12/Slpapy/processing_analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,16 @@
     # 存储数据
     adata.raw = adata
     sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
     sc.pl.highly_variable_genes(adata, save='_highly_variable_lipid.png')
     adata = adata[:, adata.var.highly_variable]
     # 回归每个细胞的总计数和表达的线粒体基因的百分比的影响。
     #sc.pp.regress_out(adata, ['total_counts', 'pct_counts_mt'])
-    mz=pd.DataFrame()
     #保存mz值
-    mz['mz']=adata.var_names
+    mz=adata.var
     mz.to_csv('mz.csv')
     adata.write('./pp_done.h5ad')
     return adata
 
 
 def se_analyze(adata):
     # 将每个脂质缩放到单位方差。阈值超过标准偏差 10。，如非高斯分布，则不建议使用
@@ -93,23 +92,23 @@
     if use_spacial == True:
         adata = XYadata(adata)
         adata = se_analyze(adata)
         sc.pl.pca_variance_ratio(adata, log=True, save='_spacial.png')
         sc.pl.umap(adata, color=['leiden'], save='_spacial.png')
         sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
         sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_spacial_Wilcoxon.png')
-        Spatial_map(adata, 'leiden')
+        adata.obs['leidenXY'] = adata.obs['leiden']
+        Spatial_map(adata, 'leidenXY')
     else:
         adata = se_analyze(adata)
         sc.pl.pca_variance_ratio(adata, log=True, save='_general.png')
         sc.pl.umap(adata, color=['leiden'], save='_general.png')
         sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
         sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_Wilcoxon.png')
-        adata.obs['leidenXY'] = adata.obs['leiden']
-        Spatial_map(adata, 'leidenXY')
+        Spatial_map(adata, 'leiden')
 
     if orgknn == True:
         adata = se_analyze(adata)
         estimator = KMeans(n_clusters=adata.obs['leiden'].values.codes.max() + 1)  # 构造聚类器
         estimator.fit(
             np.c_[adata.X, preprocessing.normalize(np.c_[np.array(adata.obs['X']), np.array(adata.obs['Y'])])])
         label_pred = estimator.labels_  # 获取聚类标签
```

