# Comparing `tmp/cell-gears-0.0.2.tar.gz` & `tmp/cell-gears-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cell-gears-0.0.2.tar", last modified: Wed Aug 17 04:13:46 2022, max compression
+gzip compressed data, was "cell-gears-0.0.3.tar", last modified: Sat Apr 15 23:25:39 2023, max compression
```

## Comparing `cell-gears-0.0.2.tar` & `cell-gears-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kexinhuang   (501) staff       (20)        0 2022-08-17 04:13:46.000000 cell-gears-0.0.2/
--rw-rw-r--   0 kexinhuang   (501) staff       (20)     1098 2022-08-17 04:09:03.000000 cell-gears-0.0.2/LICENSE
--rw-rw-r--   0 kexinhuang   (501) staff       (20)       69 2022-08-17 04:09:03.000000 cell-gears-0.0.2/MANIFEST.in
--rw-r--r--   0 kexinhuang   (501) staff       (20)     3608 2022-08-17 04:13:46.000000 cell-gears-0.0.2/PKG-INFO
--rw-rw-r--   0 kexinhuang   (501) staff       (20)     2746 2022-08-17 04:09:03.000000 cell-gears-0.0.2/README.md
-drwxr-xr-x   0 kexinhuang   (501) staff       (20)        0 2022-08-17 04:13:46.000000 cell-gears-0.0.2/cell_gears.egg-info/
--rw-r--r--   0 kexinhuang   (501) staff       (20)     3608 2022-08-17 04:13:46.000000 cell-gears-0.0.2/cell_gears.egg-info/PKG-INFO
--rw-r--r--   0 kexinhuang   (501) staff       (20)      404 2022-08-17 04:13:46.000000 cell-gears-0.0.2/cell_gears.egg-info/SOURCES.txt
--rw-r--r--   0 kexinhuang   (501) staff       (20)        1 2022-08-17 04:13:46.000000 cell-gears-0.0.2/cell_gears.egg-info/dependency_links.txt
--rw-r--r--   0 kexinhuang   (501) staff       (20)        1 2022-08-17 04:13:46.000000 cell-gears-0.0.2/cell_gears.egg-info/not-zip-safe
--rw-r--r--   0 kexinhuang   (501) staff       (20)       58 2022-08-17 04:13:46.000000 cell-gears-0.0.2/cell_gears.egg-info/requires.txt
--rw-r--r--   0 kexinhuang   (501) staff       (20)        6 2022-08-17 04:13:46.000000 cell-gears-0.0.2/cell_gears.egg-info/top_level.txt
-drwxr-xr-x   0 kexinhuang   (501) staff       (20)        0 2022-08-17 04:13:46.000000 cell-gears-0.0.2/gears/
--rw-rw-r--   0 kexinhuang   (501) staff       (20)       55 2022-08-17 04:09:03.000000 cell-gears-0.0.2/gears/__init__.py
--rw-rw-r--   0 kexinhuang   (501) staff       (20)    18809 2022-08-17 04:09:03.000000 cell-gears-0.0.2/gears/data_utils.py
--rw-rw-r--   0 kexinhuang   (501) staff       (20)    19411 2022-08-17 04:09:03.000000 cell-gears-0.0.2/gears/gears.py
--rw-rw-r--   0 kexinhuang   (501) staff       (20)    39585 2022-08-17 04:09:03.000000 cell-gears-0.0.2/gears/inference.py
--rw-rw-r--   0 kexinhuang   (501) staff       (20)     8188 2022-08-17 04:09:03.000000 cell-gears-0.0.2/gears/model.py
--rw-rw-r--   0 kexinhuang   (501) staff       (20)    13769 2022-08-17 04:09:03.000000 cell-gears-0.0.2/gears/pertdata.py
--rw-rw-r--   0 kexinhuang   (501) staff       (20)    13543 2022-08-17 04:09:03.000000 cell-gears-0.0.2/gears/utils.py
--rw-rw-r--   0 kexinhuang   (501) staff       (20)      536 2022-08-17 04:09:03.000000 cell-gears-0.0.2/gears/version.py
--rw-rw-r--   0 kexinhuang   (501) staff       (20)       57 2022-08-17 04:09:03.000000 cell-gears-0.0.2/requirements.txt
--rw-rw-r--   0 kexinhuang   (501) staff       (20)       79 2022-08-17 04:13:46.000000 cell-gears-0.0.2/setup.cfg
--rw-rw-r--   0 kexinhuang   (501) staff       (20)     1149 2022-08-17 04:09:03.000000 cell-gears-0.0.2/setup.py
+drwxr-xr-x   0 yhr      (20138) users      (100)        0 2023-04-15 23:25:39.315057 cell-gears-0.0.3/
+-rw-r--r--   0 yhr      (20138) users      (100)     1098 2023-04-15 23:05:14.000000 cell-gears-0.0.3/LICENSE
+-rw-r--r--   0 yhr      (20138) users      (100)       69 2023-04-15 23:05:14.000000 cell-gears-0.0.3/MANIFEST.in
+-rw-r--r--   0 yhr      (20138) users      (100)     3253 2023-04-15 23:25:39.322057 cell-gears-0.0.3/PKG-INFO
+-rw-r--r--   0 yhr      (20138) users      (100)     3008 2023-04-15 23:05:14.000000 cell-gears-0.0.3/README.md
+drwxr-xr-x   0 yhr      (20138) users      (100)        0 2023-04-15 23:25:39.156064 cell-gears-0.0.3/cell_gears.egg-info/
+-rw-r--r--   0 yhr      (20138) users      (100)     3253 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/PKG-INFO
+-rw-r--r--   0 yhr      (20138) users      (100)      404 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/SOURCES.txt
+-rw-r--r--   0 yhr      (20138) users      (100)        1 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/dependency_links.txt
+-rw-r--r--   0 yhr      (20138) users      (100)        1 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/not-zip-safe
+-rw-r--r--   0 yhr      (20138) users      (100)       58 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/requires.txt
+-rw-r--r--   0 yhr      (20138) users      (100)        6 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/top_level.txt
+drwxr-xr-x   0 yhr      (20138) users      (100)        0 2023-04-15 23:25:39.292058 cell-gears-0.0.3/gears/
+-rw-r--r--   0 yhr      (20138) users      (100)       55 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/__init__.py
+-rw-r--r--   0 yhr      (20138) users      (100)    18902 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/data_utils.py
+-rw-r--r--   0 yhr      (20138) users      (100)    22799 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/gears.py
+-rw-r--r--   0 yhr      (20138) users      (100)    39585 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/inference.py
+-rw-r--r--   0 yhr      (20138) users      (100)     9126 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/model.py
+-rw-r--r--   0 yhr      (20138) users      (100)    16994 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/pertdata.py
+-rw-r--r--   0 yhr      (20138) users      (100)    17572 2023-04-15 23:05:15.000000 cell-gears-0.0.3/gears/utils.py
+-rw-r--r--   0 yhr      (20138) users      (100)      537 2023-04-15 23:24:35.000000 cell-gears-0.0.3/gears/version.py
+-rw-r--r--   0 yhr      (20138) users      (100)       57 2023-04-15 23:05:15.000000 cell-gears-0.0.3/requirements.txt
+-rw-r--r--   0 yhr      (20138) users      (100)       79 2023-04-15 23:25:39.331056 cell-gears-0.0.3/setup.cfg
+-rw-r--r--   0 yhr      (20138) users      (100)     1149 2023-04-15 23:05:15.000000 cell-gears-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cell-gears-0.0.2/LICENSE` & `cell-gears-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cell-gears-0.0.2/README.md` & `cell-gears-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 gears_model.train(epochs = 20)
 
 # save/load model
 gears_model.save_model('gears')
 gears_model.load_pretrained('gears')
 
 # predict
-gears_model.predict([['FOX1A', 'AHR'], ['FEV']])
-gears_model.GI_predict([['FOX1A', 'AHR'], ['FEV', 'AHR']])
+gears_model.predict([['CBL', 'CNN1'], ['FEV']])
+gears_model.GI_predict([['CBL', 'CNN1'], ['FEV', 'AHR']])
 ```
 
 To use your own dataset, create a scanpy adata object with a `gene_name` column in `adata.var`, and two columns `condition`, `cell_type` in `adata.obs`. Then run:
 
 ```python
 pert_data.new_data_process(dataset_name = 'XXX', adata = adata)
 # to load the processed data
@@ -54,14 +54,21 @@
 |-----------------|-------------|
 | [Dataset Tutorial](demo/data_tutorial.ipynb) | Tutorial on how to use the dataset loader and read customized data|
 | [Model Tutorial](demo/model_tutorial.ipynb) | Tutorial on how to train GEARS |
 | [Plot top 20 DE genes](demo/tutorial_plot_top20_DE.ipynb) | Tutorial on how to plot the top 20 DE genes|
 | [Uncertainty](demo/tutorial_uncertainty.ipynb) | Tutorial on how to train an uncertainty-aware GEARS model |
 
 
+### Colab
+
+| Name | Description |
+|-----------------|-------------|
+| [Using Trained Model](https://colab.research.google.com/drive/11LlzGEUGoBk_Uj6DzlzizAeWse5_E9MK?usp=sharing) | Use a model trained on Norman et al. 2019 to make predictions (Needs Colab Pro)|
+
+
 
 ### Cite Us
 
 ```
 @article {Roohani2022.07.12.499735,
 	author = {Roohani, Yusuf and Huang, Kexin and Leskovec, Jure},
 	title = {GEARS: Predicting transcriptional outcomes of novel multi-gene perturbations},
```

### Comparing `cell-gears-0.0.2/gears/data_utils.py` & `cell-gears-0.0.3/gears/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,19 +50,22 @@
 
     adata.uns[key_added] = gene_dict
 
     if return_dict:
         return gene_dict
 
     
-def get_DE_genes(adata):
+def get_DE_genes(adata, skip_calc_de):
     adata.obs.loc[:, 'dose_val'] = adata.obs.condition.apply(lambda x: '1+1' if len(x.split('+')) == 2 else '1')
     adata.obs.loc[:, 'control'] = adata.obs.condition.apply(lambda x: 0 if len(x.split('+')) == 2 else 1)
     adata.obs.loc[:, 'condition_name'] =  adata.obs.apply(lambda x: '_'.join([x.cell_type, x.condition, x.dose_val]), axis = 1) 
-    rank_genes_groups_by_cov(adata, 
+    
+    adata.obs = adata.obs.astype('category')
+    if not skip_calc_de:
+        rank_genes_groups_by_cov(adata, 
                          groupby='condition_name', 
                          covariate='cell_type', 
                          control_group='ctrl_1', 
                          n_genes=len(adata.var),
                          key_added = 'rank_genes_groups_cov_all')
     return adata
```

### Comparing `cell-gears-0.0.2/gears/gears.py` & `cell-gears-0.0.3/gears/gears.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 warnings.filterwarnings("ignore")
 
 class GEARS:
     def __init__(self, pert_data, 
                  device = 'cuda',
                  weight_bias_track = False, 
                  proj_name = 'GEARS', 
-                 exp_name = 'GEARS'):
+                 exp_name = 'GEARS',
+                 pred_scalar = False,
+                 gi_predict = False):
         
         self.weight_bias_track = weight_bias_track
         
         if self.weight_bias_track:
             import wandb
             wandb.init(project=proj_name, name=exp_name)  
             self.wandb = wandb
@@ -43,28 +45,47 @@
         
         self.device = device
         self.config = None
         
         self.dataloader = pert_data.dataloader
         self.adata = pert_data.adata
         self.node_map = pert_data.node_map
+        self.node_map_pert = pert_data.node_map_pert
         self.data_path = pert_data.data_path
         self.dataset_name = pert_data.dataset_name
         self.split = pert_data.split
         self.seed = pert_data.seed
         self.train_gene_set_size = pert_data.train_gene_set_size
         self.set2conditions = pert_data.set2conditions
         self.subgroup = pert_data.subgroup
+        self.gi_predict = gi_predict
         self.gene_list = pert_data.gene_names.values.tolist()
+        self.pert_list = pert_data.pert_names.tolist()
         self.num_genes = len(self.gene_list)
-        self.ctrl_expression = torch.tensor(np.mean(self.adata.X[self.adata.obs.condition == 'ctrl'], axis = 0)).reshape(-1,).to(self.device)
+        self.num_perts = len(self.pert_list)
+        self.default_GO_graph = pert_data.default_GO_graph
+        self.saved_pred = {}
+        self.saved_logvar_sum = {}
+        
+        self.ctrl_expression = torch.tensor(
+            np.mean(self.adata.X[self.adata.obs.condition == 'ctrl'],
+                    axis=0)).reshape(-1, ).to(self.device)
         pert_full_id2pert = dict(self.adata.obs[['condition_name', 'condition']].values)
-        self.dict_filter = {pert_full_id2pert[i]: j for i,j in self.adata.uns['non_zeros_gene_idx'].items()}
+        if gi_predict:
+            self.dict_filter = None
+        else:
+            self.dict_filter = {pert_full_id2pert[i]: j for i, j in
+                                self.adata.uns['non_zeros_gene_idx'].items() if
+                                i in pert_full_id2pert}
         self.ctrl_adata = self.adata[self.adata.obs['condition'] == 'ctrl']
-    
+        
+        gene_dict = {g:i for i,g in enumerate(self.gene_list)}
+        self.pert2gene = {p: gene_dict[pert] for p, pert in
+                          enumerate(self.pert_list) if pert in self.gene_list}
+
     def tunable_parameters(self):
         return {'hidden_size': 'hidden dimension, default 64',
                 'num_go_gnn_layers': 'number of GNN layers for GO graph, default 1',
                 'num_gene_gnn_layers': 'number of GNN layers for co-expression gene graph, default 1',
                 'decoder_hidden_size': 'hidden dimension for gene-specific decoder, default 16',
                 'num_similar_genes_go_graph': 'number of maximum similar K genes in the GO graph, default 20',
                 'num_similar_genes_co_express_graph': 'number of maximum similar K genes in the co expression graph, default 20',
@@ -83,15 +104,18 @@
                          coexpress_threshold = 0.4,
                          uncertainty = False, 
                          uncertainty_reg = 1,
                          direction_lambda = 1e-1,
                          G_go = None,
                          G_go_weight = None,
                          G_coexpress = None,
-                         G_coexpress_weight = None):
+                         G_coexpress_weight = None,
+                         no_perturb = False, 
+                         cell_fitness_pred = False,
+                        ):
         
         self.config = {'hidden_size': hidden_size,
                        'num_go_gnn_layers' : num_go_gnn_layers, 
                        'num_gene_gnn_layers' : num_gene_gnn_layers,
                        'decoder_hidden_size' : decoder_hidden_size,
                        'num_similar_genes_go_graph' : num_similar_genes_go_graph,
                        'num_similar_genes_co_express_graph' : num_similar_genes_co_express_graph,
@@ -100,42 +124,65 @@
                        'uncertainty_reg' : uncertainty_reg,
                        'direction_lambda' : direction_lambda,
                        'G_go': G_go,
                        'G_go_weight': G_go_weight,
                        'G_coexpress': G_coexpress,
                        'G_coexpress_weight': G_coexpress_weight,
                        'device': self.device,
-                       'num_genes': self.num_genes
+                       'num_genes': self.num_genes,
+                       'num_perts': self.num_perts,
+                       'no_perturb': no_perturb,
+                       'cell_fitness_pred': cell_fitness_pred,
                       }
         
         if self.wandb:
             self.wandb.config.update(self.config)
         
         if self.config['G_coexpress'] is None:
             ## calculating co expression similarity graph
-            edge_list = get_similarity_network(network_type = 'co-express', adata = self.adata, threshold = coexpress_threshold, k = num_similar_genes_co_express_graph, gene_list = self.gene_list, data_path = self.data_path, data_name = self.dataset_name, split = self.split, seed = self.seed, train_gene_set_size = self.train_gene_set_size, set2conditions = self.set2conditions)
+            edge_list = get_similarity_network(network_type='co-express',
+                                               adata=self.adata,
+                                               threshold=coexpress_threshold,
+                                               k=num_similar_genes_co_express_graph,
+                                               data_path=self.data_path,
+                                               data_name=self.dataset_name,
+                                               split=self.split, seed=self.seed,
+                                               train_gene_set_size=self.train_gene_set_size,
+                                               set2conditions=self.set2conditions)
+
             sim_network = GeneSimNetwork(edge_list, self.gene_list, node_map = self.node_map)
             self.config['G_coexpress'] = sim_network.edge_index
             self.config['G_coexpress_weight'] = sim_network.edge_weight
         
         if self.config['G_go'] is None:
             ## calculating gene ontology similarity graph
-            edge_list = get_similarity_network(network_type = 'go', adata = self.adata, threshold = coexpress_threshold, k = num_similar_genes_go_graph, gene_list = self.gene_list, data_path = self.data_path, data_name = self.dataset_name, split = self.split, seed = self.seed, train_gene_set_size = self.train_gene_set_size, set2conditions = self.set2conditions)
-            sim_network = GeneSimNetwork(edge_list, self.gene_list, node_map = self.node_map)
+            edge_list = get_similarity_network(network_type='go',
+                                               adata=self.adata,
+                                               threshold=coexpress_threshold,
+                                               k=num_similar_genes_go_graph,
+                                               pert_list=self.pert_list,
+                                               data_path=self.data_path,
+                                               data_name=self.dataset_name,
+                                               split=self.split, seed=self.seed,
+                                               train_gene_set_size=self.train_gene_set_size,
+                                               set2conditions=self.set2conditions,
+                                               default_GO_graph=self.default_GO_graph)
+
+            sim_network = GeneSimNetwork(edge_list, self.pert_list, node_map = self.node_map_pert)
             self.config['G_go'] = sim_network.edge_index
             self.config['G_go_weight'] = sim_network.edge_weight
             
         self.model = GEARS_Model(self.config).to(self.device)
         self.best_model = deepcopy(self.model)
         
     def load_pretrained(self, path):
         with open(os.path.join(path, 'config.pkl'), 'rb') as f:
             config = pickle.load(f)
         
-        del config['device'], config['num_genes']
+        del config['device'], config['num_genes'], config['num_perts']
         self.model_initialize(**config)
         self.config = config
         
         state_dict = torch.load(os.path.join(path, 'model.pt'), map_location = torch.device('cpu'))
         if next(iter(state_dict))[:7] == 'module.':
             # the pretrained model is from data-parallel module
             from collections import OrderedDict
@@ -164,79 +211,112 @@
     def predict(self, pert_list):
         ## given a list of single/combo genes, return the transcriptome
         ## if uncertainty mode is on, also return uncertainty score.
         
         self.ctrl_adata = self.adata[self.adata.obs['condition'] == 'ctrl']
         for pert in pert_list:
             for i in pert:
-                if i not in self.gene_list:
-                    raise ValueError("The gene is not in the perturbation graph. Please select from GEARS.gene_list!")
+                if i not in self.pert_list:
+                    raise ValueError(i+ " is not in the perturbation graph. "
+                                        "Please select from GEARS.gene_list!")
         
         if self.config['uncertainty']:
             results_logvar = {}
             
         self.best_model = self.best_model.to(self.device)
         self.best_model.eval()
         results_pred = {}
+        results_logvar_sum = {}
+        
         from torch_geometric.data import DataLoader
         for pert in pert_list:
-            cg = create_cell_graph_dataset_for_prediction(pert, self.ctrl_adata, self.gene_list, self.device)
+            try:
+                #If prediction is already saved, then skip inference
+                results_pred['_'.join(pert)] = self.saved_pred['_'.join(pert)]
+                if self.config['uncertainty']:
+                    results_logvar_sum['_'.join(pert)] = self.saved_logvar_sum['_'.join(pert)]
+                continue
+            except:
+                pass
+            
+            cg = create_cell_graph_dataset_for_prediction(pert, self.ctrl_adata,
+                                                    self.pert_list, self.device)
             loader = DataLoader(cg, 300, shuffle = False)
             batch = next(iter(loader))
             batch.to(self.device)
 
             with torch.no_grad():
                 if self.config['uncertainty']:
                     p, unc = self.best_model(batch)
                     results_logvar['_'.join(pert)] = np.mean(unc.detach().cpu().numpy(), axis = 0)
+                    results_logvar_sum['_'.join(pert)] = np.exp(-np.mean(results_logvar['_'.join(pert)]))
                 else:
                     p = self.best_model(batch)
                     
             results_pred['_'.join(pert)] = np.mean(p.detach().cpu().numpy(), axis = 0)
+                
+        self.saved_pred.update(results_pred)
         
         if self.config['uncertainty']:
-            results_logvar_sum = {i: np.exp(-np.mean(j)) for i,j in results_logvar.items()}    
+            self.saved_logvar_sum.update(results_logvar_sum)
             return results_pred, results_logvar_sum
         else:
             return results_pred
         
     def GI_predict(self, combo, GI_genes_file='./genes_with_hi_mean.npy'):
         ## given a gene pair, return (1) transcriptome of A,B,A+B and (2) GI scores. 
         ## if uncertainty mode is on, also return uncertainty score.
         
-        preds = self.predict([[combo[0]], [combo[1]], combo])
+        try:
+            # If prediction is already saved, then skip inference
+            pred = {}
+            pred[combo[0]] = self.saved_pred[combo[0]]
+            pred[combo[1]] = self.saved_pred[combo[1]]
+            pred['_'.join(combo)] = self.saved_pred['_'.join(combo)]
+        except:
+            if self.config['uncertainty']:
+                pred = self.predict([[combo[0]], [combo[1]], combo])[0]
+            else:
+                pred = self.predict([[combo[0]], [combo[1]], combo])
 
         mean_control = get_mean_control(self.adata).values  
-        preds = {p:preds[p]-mean_control for p in preds} 
+        pred = {p:pred[p]-mean_control for p in pred} 
 
         if GI_genes_file is not None:
             # If focussing on a specific subset of genes for calculating metrics
-            GI_genes_idx = get_GI_genes_idx(self.adata, GI_genes_file)
-            preds = {p:preds[p][GI_genes_idx] for p in preds} 
-
-        return get_GI_params(preds, combo)
+            GI_genes_idx = get_GI_genes_idx(self.adata, GI_genes_file)       
+        else:
+            GI_genes_idx = np.arange(len(self.adata.var.gene_name.values))
+            
+        pred = {p:pred[p][GI_genes_idx] for p in pred}
+        return get_GI_params(pred, combo)
     
     def plot_perturbation(self, query, save_file = None):
         import seaborn as sns
         import numpy as np
         import matplotlib.pyplot as plt
         
         sns.set_theme(style="ticks", rc={"axes.facecolor": (0, 0, 0, 0)}, font_scale=1.5)
 
         adata = self.adata
         gene2idx = self.node_map
         cond2name = dict(adata.obs[['condition', 'condition_name']].values)
         gene_raw2id = dict(zip(adata.var.index.values, adata.var.gene_name.values))
-        
-        de_idx = [gene2idx[gene_raw2id[i]] for i in adata.uns['top_non_dropout_de_20'][cond2name[query]]]
-        genes = [gene_raw2id[i] for i in adata.uns['top_non_dropout_de_20'][cond2name[query]]]
+
+        de_idx = [gene2idx[gene_raw2id[i]] for i in
+                  adata.uns['top_non_dropout_de_20'][cond2name[query]]]
+        genes = [gene_raw2id[i] for i in
+                 adata.uns['top_non_dropout_de_20'][cond2name[query]]]
         truth = adata[adata.obs.condition == query].X.toarray()[:, de_idx]
-        pred = self.predict([query.split('+')])['_'.join(query.split('+'))][de_idx]
-        ctrl_means = adata[adata.obs['condition'] == 'ctrl'].to_df().mean()[de_idx].values
         
+        query_ = [q for q in query.split('+') if q != 'ctrl']
+        pred = self.predict([query_])['_'.join(query_)][de_idx]
+        ctrl_means = adata[adata.obs['condition'] == 'ctrl'].to_df().mean()[
+            de_idx].values
+
         pred = pred - ctrl_means
         truth = truth - ctrl_means
         
         plt.figure(figsize=[16.5,4.5])
         plt.title(query)
         plt.boxplot(truth, showfliers=False,
                     medianprops = dict(linewidth=0))    
@@ -264,15 +344,15 @@
               weight_decay = 5e-4
              ):
         
         train_loader = self.dataloader['train_loader']
         val_loader = self.dataloader['val_loader']
             
         self.model = self.model.to(self.device)
-        
+        best_model = deepcopy(self.model)
         optimizer = optim.Adam(self.model.parameters(), lr=lr, weight_decay = weight_decay)
         scheduler = StepLR(optimizer, step_size=1, gamma=0.5)
 
         min_val = np.inf
         print_sys('Start Training...')
 
         for epoch in range(epochs):
@@ -304,16 +384,18 @@
 
                 if step % 50 == 0:
                     log = "Epoch {} Step {} Train Loss: {:.4f}" 
                     print_sys(log.format(epoch + 1, step + 1, loss.item()))
 
             scheduler.step()
             # Evaluate model performance on train and val set
-            train_res = evaluate(train_loader, self.model, self.config['uncertainty'], self.device)
-            val_res = evaluate(val_loader, self.model, self.config['uncertainty'], self.device)
+            train_res = evaluate(train_loader, self.model,
+                                 self.config['uncertainty'], self.device)
+            val_res = evaluate(val_loader, self.model,
+                                 self.config['uncertainty'], self.device)
             train_metrics, _ = compute_metrics(train_res)
             val_metrics, _ = compute_metrics(val_res)
 
             # Print epoch performance
             log = "Epoch {}: Train Overall MSE: {:.4f} " \
                   "Validation Overall MSE: {:.4f}. "
             print_sys(log.format(epoch + 1, train_metrics['mse'], 
@@ -343,15 +425,16 @@
         if 'test_loader' not in self.dataloader:
             print_sys('Done! No test dataloader detected.')
             return
             
         # Model testing
         test_loader = self.dataloader['test_loader']
         print_sys("Start Testing...")
-        test_res = evaluate(test_loader, self.best_model, self.config['uncertainty'], self.device)   
+        test_res = evaluate(test_loader, self.best_model,
+                            self.config['uncertainty'], self.device)
         test_metrics, test_pert_res = compute_metrics(test_res)    
         log = "Best performing model: Test Top 20 DE MSE: {:.4f}"
         print_sys(log.format(test_metrics['mse_de']))
         
         if self.wandb:
             metrics = ['mse', 'pearson']
             for m in metrics:
@@ -359,15 +442,17 @@
                            'test_de_'+m: test_metrics[m + '_de']                     
                           })
                 
         out = deeper_analysis(self.adata, test_res)
         out_non_dropout = non_dropout_analysis(self.adata, test_res)
         
         metrics = ['pearson_delta']
-        metrics_non_dropout = ['frac_opposite_direction_top20_non_dropout', 'frac_sigma_below_1_non_dropout', 'mse_top20_de_non_dropout']
+        metrics_non_dropout = ['frac_opposite_direction_top20_non_dropout',
+                               'frac_sigma_below_1_non_dropout',
+                               'mse_top20_de_non_dropout']
         
         if self.wandb:
             for m in metrics:
                 self.wandb.log({'test_' + m: np.mean([j[m] for i,j in out.items() if m in j])})
 
             for m in metrics_non_dropout:
                 self.wandb.log({'test_' + m: np.mean([j[m] for i,j in out_non_dropout.items() if m in j])})
```

### Comparing `cell-gears-0.0.2/gears/inference.py` & `cell-gears-0.0.3/gears/inference.py`

 * *Files identical despite different names*

### Comparing `cell-gears-0.0.2/gears/model.py` & `cell-gears-0.0.3/gears/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,27 +31,30 @@
     GEARS
     """
 
     def __init__(self, args):
         super(GEARS_Model, self).__init__()
         self.args = args       
         self.num_genes = args['num_genes']
+        self.num_perts = args['num_perts']
         hidden_size = args['hidden_size']
         self.uncertainty = args['uncertainty']
         self.num_layers = args['num_go_gnn_layers']
         self.indv_out_hidden_size = args['decoder_hidden_size']
         self.num_layers_gene_pos = args['num_gene_gnn_layers']
+        self.no_perturb = args['no_perturb']
+        self.cell_fitness_pred = args['cell_fitness_pred']
         self.pert_emb_lambda = 0.2
         
         # perturbation positional embedding added only to the perturbed genes
         self.pert_w = nn.Linear(1, hidden_size)
            
         # gene/globel perturbation embedding dictionary lookup            
         self.gene_emb = nn.Embedding(self.num_genes, hidden_size, max_norm=True)
-        self.pert_emb = nn.Embedding(self.num_genes, hidden_size, max_norm=True)
+        self.pert_emb = nn.Embedding(self.num_perts, hidden_size, max_norm=True)
         
         # transformation layer
         self.emb_trans = nn.ReLU()
         self.pert_base_trans = nn.ReLU()
         self.transform = nn.ReLU()
         self.emb_trans_v2 = MLP([hidden_size, hidden_size, hidden_size], last_layer_act='ReLU')
         self.pert_fuse = MLP([hidden_size, hidden_size, hidden_size], last_layer_act='ReLU')
@@ -99,95 +102,107 @@
         self.bn_pert_base = nn.BatchNorm1d(hidden_size)
         self.bn_pert_base_trans = nn.BatchNorm1d(hidden_size)
         
         # uncertainty mode
         if self.uncertainty:
             self.uncertainty_w = MLP([hidden_size, hidden_size*2, hidden_size, 1], last_layer_act='linear')
         
+        #if self.cell_fitness_pred:
+        self.cell_fitness_mlp = MLP([self.num_genes, hidden_size*2, hidden_size, 1], last_layer_act='linear')
 
     def forward(self, data):
-        x, batch = data.x, data.batch
-        num_graphs = len(data.batch.unique())
-
-        ## get base gene embeddings
-        emb = self.gene_emb(torch.LongTensor(list(range(self.num_genes))).repeat(num_graphs, ).to(self.args['device']))        
-        emb = self.bn_emb(emb)
-        base_emb = self.emb_trans(emb)        
-        
-        pos_emb = self.emb_pos(torch.LongTensor(list(range(self.num_genes))).repeat(num_graphs, ).to(self.args['device']))
-        for idx, layer in enumerate(self.layers_emb_pos):
-            pos_emb = layer(pos_emb, self.G_coexpress, self.G_coexpress_weight)
-            if idx < len(self.layers_emb_pos) - 1:
-                pos_emb = pos_emb.relu()
-
-        base_emb = base_emb + 0.2 * pos_emb
-        base_emb = self.emb_trans_v2(base_emb)
-
-        ## get perturbation index and embeddings
-        pert = x[:, 1].reshape(-1,1)
-        pert_index = torch.where(pert.reshape(num_graphs, int(x.shape[0]/num_graphs)) == 1)
-        pert_global_emb = self.pert_emb(torch.LongTensor(list(range(self.num_genes))).to(self.args['device']))        
-        
-        ## augment global perturbation embedding with GNN
-        for idx, layer in enumerate(self.sim_layers):
-            pert_global_emb = layer(pert_global_emb, self.G_sim, self.G_sim_weight)
-            if idx < self.num_layers - 1:
-                pert_global_emb = pert_global_emb.relu()
-
-        ## add global perturbation embedding to each gene in each cell in the batch
-        base_emb = base_emb.reshape(num_graphs, self.num_genes, -1)
+        x, pert_idx = data.x, data.pert_idx
+        if self.no_perturb:
+            out = x.reshape(-1,1)
+            out = torch.split(torch.flatten(out), self.num_genes)           
+            return torch.stack(out)
+        else:
+            num_graphs = len(data.batch.unique())
+
+            ## get base gene embeddings
+            emb = self.gene_emb(torch.LongTensor(list(range(self.num_genes))).repeat(num_graphs, ).to(self.args['device']))        
+            emb = self.bn_emb(emb)
+            base_emb = self.emb_trans(emb)        
+
+            pos_emb = self.emb_pos(torch.LongTensor(list(range(self.num_genes))).repeat(num_graphs, ).to(self.args['device']))
+            for idx, layer in enumerate(self.layers_emb_pos):
+                pos_emb = layer(pos_emb, self.G_coexpress, self.G_coexpress_weight)
+                if idx < len(self.layers_emb_pos) - 1:
+                    pos_emb = pos_emb.relu()
+
+            base_emb = base_emb + 0.2 * pos_emb
+            base_emb = self.emb_trans_v2(base_emb)
+
+            ## get perturbation index and embeddings
+
+            pert_index = []
+            for idx, i in enumerate(pert_idx):
+                for j in i:
+                    if j != -1:
+                        pert_index.append([idx, j])
+            pert_index = torch.tensor(pert_index).T
+
+            pert_global_emb = self.pert_emb(torch.LongTensor(list(range(self.num_perts))).to(self.args['device']))        
+
+            ## augment global perturbation embedding with GNN
+            for idx, layer in enumerate(self.sim_layers):
+                pert_global_emb = layer(pert_global_emb, self.G_sim, self.G_sim_weight)
+                if idx < self.num_layers - 1:
+                    pert_global_emb = pert_global_emb.relu()
+
+            ## add global perturbation embedding to each gene in each cell in the batch
+            base_emb = base_emb.reshape(num_graphs, self.num_genes, -1)
+
+            if pert_index.shape[0] != 0:
+                ### in case all samples in the batch are controls, then there is no indexing for pert_index.
+                pert_track = {}
+                for i, j in enumerate(pert_index[0]):
+                    if j.item() in pert_track:
+                        pert_track[j.item()] = pert_track[j.item()] + pert_global_emb[pert_index[1][i]]
+                    else:
+                        pert_track[j.item()] = pert_global_emb[pert_index[1][i]]
+
+                if len(list(pert_track.values())) > 0:
+                    if len(list(pert_track.values())) == 1:
+                        # circumvent when batch size = 1 with single perturbation and cannot feed into MLP
+                        emb_total = self.pert_fuse(torch.stack(list(pert_track.values()) * 2))
+                    else:
+                        emb_total = self.pert_fuse(torch.stack(list(pert_track.values())))
+
+                    for idx, j in enumerate(pert_track.keys()):
+                        base_emb[j] = base_emb[j] + emb_total[idx]
+
+            base_emb = base_emb.reshape(num_graphs * self.num_genes, -1)
+            base_emb = self.bn_pert_base(base_emb)
+
+            ## apply the first MLP
+            base_emb = self.transform(base_emb)        
+            out = self.recovery_w(base_emb)
+            out = out.reshape(num_graphs, self.num_genes, -1)
+            out = out.unsqueeze(-1) * self.indv_w1
+            w = torch.sum(out, axis = 2)
+            out = w + self.indv_b1
+
+            # Cross gene
+            cross_gene_embed = self.cross_gene_state(out.reshape(num_graphs, self.num_genes, -1).squeeze(2))
+            cross_gene_embed = cross_gene_embed.repeat(1, self.num_genes)
+
+            cross_gene_embed = cross_gene_embed.reshape([num_graphs,self.num_genes, -1])
+            cross_gene_out = torch.cat([out, cross_gene_embed], 2)
+
+            cross_gene_out = cross_gene_out * self.indv_w2
+            cross_gene_out = torch.sum(cross_gene_out, axis=2)
+            out = cross_gene_out + self.indv_b2        
+            out = out.reshape(num_graphs * self.num_genes, -1) + x.reshape(-1,1)
+            out = torch.split(torch.flatten(out), self.num_genes)
+
+            ## uncertainty head
+            if self.uncertainty:
+                out_logvar = self.uncertainty_w(base_emb)
+                out_logvar = torch.split(torch.flatten(out_logvar), self.num_genes)
+                return torch.stack(out), torch.stack(out_logvar)
             
-        pert_track = {}
-        for i, j in enumerate(pert_index[0]):
-            if j in pert_track:
-                pert_track[j] = pert_track[j] + pert_global_emb[pert_index[1][i]]
-            else:
-                pert_track[j] = pert_global_emb[pert_index[1][i]]
-
-        if len(list(pert_track.values())) > 0:
-            if len(list(pert_track.values())) == 1:
-                # circumvent when batch size = 1 with single perturbation and cannot feed into MLP
-                emb_total = self.pert_fuse(torch.stack(list(pert_track.values()) * 2))
-            else:
-                emb_total = self.pert_fuse(torch.stack(list(pert_track.values())))
-
-            for idx, j in enumerate(pert_track.keys()):
-                base_emb[j] = base_emb[j] + emb_total[idx]
-
-        base_emb = base_emb.reshape(num_graphs * self.num_genes, -1)
-        
-        ## add the perturbation positional embedding
-        pert_emb = self.pert_w(pert)
-        combined = pert_emb+base_emb
-        combined = self.bn_pert_base_trans(combined)
-        base_emb = self.pert_base_trans(combined)
-        base_emb = self.bn_pert_base(base_emb)
-        
-        ## apply the first MLP
-        base_emb = self.transform(base_emb)        
-        out = self.recovery_w(base_emb)
-        out = out.reshape(num_graphs, self.num_genes, -1)
-        out = out.unsqueeze(-1) * self.indv_w1
-        w = torch.sum(out, axis = 2)
-        out = w + self.indv_b1
-
-        # Cross gene
-        cross_gene_embed = self.cross_gene_state(out.reshape(num_graphs, self.num_genes, -1).squeeze(2))
-        cross_gene_embed = cross_gene_embed.repeat(1, self.num_genes)
-
-        cross_gene_embed = cross_gene_embed.reshape([num_graphs,self.num_genes, -1])
-        cross_gene_out = torch.cat([out, cross_gene_embed], 2)
-
-        cross_gene_out = cross_gene_out * self.indv_w2
-        cross_gene_out = torch.sum(cross_gene_out, axis=2)
-        out = cross_gene_out + self.indv_b2        
-        out = out.reshape(num_graphs * self.num_genes, -1) + x[:, 0].reshape(-1,1)
-        out = torch.split(torch.flatten(out), self.num_genes)
-
-        ## uncertainty head
-        if self.uncertainty:
-            out_logvar = self.uncertainty_w(base_emb)
-            out_logvar = torch.split(torch.flatten(out_logvar), self.num_genes)
-            return torch.stack(out), torch.stack(out_logvar)
-
-        return torch.stack(out)
+            if self.cell_fitness_pred:
+                return torch.stack(out), self.cell_fitness_mlp(torch.stack(out))
+            
+            return torch.stack(out)
```

### Comparing `cell-gears-0.0.2/gears/pertdata.py` & `cell-gears-0.0.3/gears/pertdata.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,31 +3,71 @@
 import numpy as np
 import pickle
 from torch_geometric.data import DataLoader
 import os
 import scanpy as sc
 import networkx as nx
 from tqdm import tqdm
+import pandas as pd
 
 import warnings
 warnings.filterwarnings("ignore")
 sc.settings.verbosity = 0
 
 from .data_utils import get_DE_genes, get_dropout_non_zero_genes, DataSplitter
-from .utils import print_sys, zip_data_download_wrapper
+from .utils import print_sys, zip_data_download_wrapper, dataverse_download, filter_pert_in_go
 
 class PertData:
     
-    def __init__(self, data_path):
+    def __init__(self, data_path, gene_set_path = None):
+        
+        # Dataset/Dataloader attributes
         self.data_path = data_path
+        self.default_GO_graph = True
+        self.dataset_name = None
+        self.dataset_path = None
+        self.adata = None
+        self.dataset_processed = None
+        self.ctrl_adata = None
+        self.gene_names = []
+        self.node_map = {}
+
+        # Split attributes
+        self.split = None
+        self.seed = None
+        self.subgroup = None
+        self.train_gene_set_size = None
+
         if not os.path.exists(self.data_path):
             os.mkdir(self.data_path)
+        server_path = 'https://dataverse.harvard.edu/api/access/datafile/6153417'
+        dataverse_download(server_path,
+                           os.path.join(self.data_path, 'gene2go_all.pkl'))
+        with open(os.path.join(self.data_path, 'gene2go_all.pkl'), 'rb') as f:
+            gene2go = pickle.load(f)
+        
+        if gene_set_path is not None:
+            # If gene set specified for GO graph, use that
+            gene_set_path = gene_set_path
+            self.default_GO_graph = False
+        else:
+            # Otherwise, use a large set of genes to create GO
+            server_path = 'https://dataverse.harvard.edu/api/access/datafile/6934320'
+            gene_set_path = os.path.join(self.data_path,
+                                     'essential_all_data_pert_genes.pkl')
+            dataverse_download(server_path, gene_set_path)
+        with open(gene_set_path, 'rb') as f:
+            essential_genes = pickle.load(f)
+    
+        gene2go = {i: gene2go[i] for i in essential_genes if i in gene2go}
+
+        self.pert_names = np.unique(list(gene2go.keys()))
+        self.node_map_pert = {x: it for it, x in enumerate(self.pert_names)}
             
-    def load(self, data_name = None, 
-             data_path = None):
+    def load(self, data_name = None, data_path = None):
         if data_name in ['norman', 'adamson', 'dixit']:
             ## load from harvard dataverse
             if data_name == 'norman':
                 url = 'https://dataverse.harvard.edu/api/access/datafile/6154020'
             elif data_name == 'adamson':
                 url = 'https://dataverse.harvard.edu/api/access/datafile/6154417'
             elif data_name == 'dixit':
@@ -41,36 +81,51 @@
 
         elif os.path.exists(data_path):
             adata_path = os.path.join(data_path, 'perturb_processed.h5ad')
             self.adata = sc.read_h5ad(adata_path)
             self.dataset_name = data_path.split('/')[-1]
             self.dataset_path = data_path
         else:
-            raise ValueError("data is either Norman/Adamson/Dixit or a path to an h5ad file")
+            raise ValueError("data attribute is either Norman/Adamson/Dixit "
+                             "or a path to an h5ad file")
         
+        print_sys('These perturbations are not in the GO graph and their '
+                  'perturbation can thus not be predicted')
+        not_in_go_pert = np.array(self.adata.obs[
+                                  self.adata.obs.condition.apply(
+                                  lambda x:not filter_pert_in_go(x,
+                                        self.pert_names))].condition.unique())
+        print_sys(not_in_go_pert)
+        
+        filter_go = self.adata.obs[self.adata.obs.condition.apply(
+                              lambda x: filter_pert_in_go(x, self.pert_names))]
+        self.adata = self.adata[filter_go.index.values, :]
         pyg_path = os.path.join(data_path, 'data_pyg')
         if not os.path.exists(pyg_path):
             os.mkdir(pyg_path)
         dataset_fname = os.path.join(pyg_path, 'cell_graphs.pkl')
                 
         if os.path.isfile(dataset_fname):
             print_sys("Local copy of pyg dataset is detected. Loading...")
             self.dataset_processed = pickle.load(open(dataset_fname, "rb"))        
             print_sys("Done!")
         else:
             self.ctrl_adata = self.adata[self.adata.obs['condition'] == 'ctrl']
             self.gene_names = self.adata.var.gene_name
+            
+            
             print_sys("Creating pyg object for each cell in the data...")
             self.dataset_processed = self.create_dataset_file()
             print_sys("Saving new dataset pyg object at " + dataset_fname) 
             pickle.dump(self.dataset_processed, open(dataset_fname, "wb"))    
             print_sys("Done!")
             
     def new_data_process(self, dataset_name,
-                         adata = None):
+                         adata = None,
+                         skip_calc_de = False):
         
         if 'condition' not in adata.obs.columns.values:
             raise ValueError("Please specify condition")
         if 'gene_name' not in adata.var.columns.values:
             raise ValueError("Please specify gene name")
         if 'cell_type' not in adata.obs.columns.values:
             raise ValueError("Please specify cell type")
@@ -78,16 +133,17 @@
         dataset_name = dataset_name.lower()
         self.dataset_name = dataset_name
         save_data_folder = os.path.join(self.data_path, dataset_name)
         
         if not os.path.exists(save_data_folder):
             os.mkdir(save_data_folder)
         self.dataset_path = save_data_folder
-        self.adata = get_DE_genes(adata)
-        self.adata = get_dropout_non_zero_genes(self.adata)
+        self.adata = get_DE_genes(adata, skip_calc_de)
+        if not skip_calc_de:
+            self.adata = get_dropout_non_zero_genes(self.adata)
         self.adata.write_h5ad(os.path.join(save_data_folder, 'perturb_processed.h5ad'))
         
         self.ctrl_adata = self.adata[self.adata.obs['condition'] == 'ctrl']
         self.gene_names = self.adata.var.gene_name
         pyg_path = os.path.join(save_data_folder, 'data_pyg')
         if not os.path.exists(pyg_path):
             os.mkdir(pyg_path)
@@ -102,27 +158,29 @@
                       seed = 1, 
                       train_gene_set_size = 0.75,
                       combo_seen2_train_frac = 0.75,
                       combo_single_split_test_set_fraction = 0.1,
                       test_perts = None,
                       only_test_set_perts = False,
                       test_pert_genes = None):
-        available_splits = ['simulation', 'simulation_single', 'combo_seen0', 'combo_seen1', 
-                            'combo_seen2', 'single', 'no_test', 'no_split']
+        available_splits = ['simulation', 'simulation_single', 'combo_seen0',
+                            'combo_seen1', 'combo_seen2', 'single', 'no_test',
+                            'no_split']
         if split not in available_splits:
             raise ValueError('currently, we only support ' + ','.join(available_splits))
         self.split = split
         self.seed = seed
         self.subgroup = None
         self.train_gene_set_size = train_gene_set_size
         
         split_folder = os.path.join(self.dataset_path, 'splits')
         if not os.path.exists(split_folder):
             os.mkdir(split_folder)
-        split_file = self.dataset_name + '_' + split + '_' + str(seed) + '_' + str(train_gene_set_size) + '.pkl'
+        split_file = self.dataset_name + '_' + split + '_' + str(seed) + '_' \
+                                       +  str(train_gene_set_size) + '.pkl'
         split_path = os.path.join(split_folder, split_file)
         
         if test_perts:
             split_path = split_path[:-4] + '_' + test_perts + '.pkl'
         
         if os.path.exists(split_path):
             print_sys("Local copy of split is detected. Loading...")
@@ -160,25 +218,28 @@
                 adata = DS.split_data(test_size=combo_single_split_test_set_fraction,
                                       test_perts=test_perts,
                                       test_pert_genes=test_pert_genes,
                                       seed=seed)
             
             elif split == 'single':
                 DS = DataSplitter(self.adata, split_type=split)
-                adata = DS.split_data(test_size=combo_single_split_test_set_fraction, seed=seed)
+                adata = DS.split_data(test_size=combo_single_split_test_set_fraction,
+                                      seed=seed)
             
             elif split == 'no_test':
                 DS = DataSplitter(self.adata, split_type=split)
-                adata = DS.split_data(test_size=combo_single_split_test_set_fraction, seed=seed)
+                adata = DS.split_data(test_size=combo_single_split_test_set_fraction,
+                                      seed=seed)
             
             elif split == 'no_split':          
                 adata = self.adata
                 adata.obs['split'] = 'test'
             
-            set2conditions = dict(adata.obs.groupby('split').agg({'condition': lambda x: x}).condition)
+            set2conditions = dict(adata.obs.groupby('split').agg({'condition':
+                                                        lambda x: x}).condition)
             set2conditions = {i: j.unique().tolist() for i,j in set2conditions.items()} 
             pickle.dump(set2conditions, open(split_path, "wb"))
             print_sys("Saving new splits at " + split_path)
             
         self.set2conditions = set2conditions
 
         if split == 'simulation':
@@ -189,15 +250,15 @@
         
     def get_dataloader(self, batch_size, test_batch_size = None):
         if test_batch_size is None:
             test_batch_size = batch_size
             
         self.node_map = {x: it for it, x in enumerate(self.adata.var.gene_name)}
         self.gene_names = self.adata.var.gene_name
-        
+       
         # Create cell graphs
         cell_graphs = {}
         if self.split == 'no_split':
             i = 'test'
             cell_graphs[i] = []
             for p in self.set2conditions[i]:
                 if p != 'ctrl':
@@ -235,64 +296,84 @@
                                     'val_loader': val_loader,
                                     'test_loader': test_loader}
 
             else: 
                 self.dataloader =  {'train_loader': train_loader,
                                     'val_loader': val_loader}
             print_sys("Done!")
-        del self.dataset_processed # clean up some memory
+        #del self.dataset_processed # clean up some memory
     
         
     def create_dataset_file(self):
         dl = {}
         for p in tqdm(self.adata.obs['condition'].unique()):
             cell_graph_dataset = self.create_cell_graph_dataset(self.adata, p, num_samples=1)
             dl[p] = cell_graph_dataset
         return dl
     
     def get_pert_idx(self, pert_category, adata_):
-        pert_idx = [np.where(p == self.gene_names)[0][0]
+        try:
+            pert_idx = [np.where(p == self.pert_names)[0][0]
                     for p in pert_category.split('+')
                     if p != 'ctrl']
+        except:
+            print(pert_category)
+            pert_idx = None
+            
         return pert_idx
 
     # Set up feature matrix and output
+        
     def create_cell_graph(self, X, y, de_idx, pert, pert_idx=None):
-        pert_feats = np.zeros(len(X[0]))
+
+        #pert_feats = np.expand_dims(pert_feats, 0)
+        #feature_mat = torch.Tensor(np.concatenate([X, pert_feats])).T
+        feature_mat = torch.Tensor(X).T
+        
+        '''
+        pert_feats = np.zeros(len(self.pert_names))
         if pert_idx is not None:
             for p in pert_idx:
                 pert_feats[int(np.abs(p))] = 1
-        pert_feats = np.expand_dims(pert_feats, 0)
-        feature_mat = torch.Tensor(np.concatenate([X, pert_feats])).T
-
-        return Data(x=feature_mat, edge_index=None, edge_attr=None,
+        pert_feats = torch.Tensor(pert_feats).T
+        '''
+        if pert_idx is None:
+            pert_idx = [-1]
+        return Data(x=feature_mat, pert_idx=pert_idx,
                     y=torch.Tensor(y), de_idx=de_idx, pert=pert)
 
     def create_cell_graph_dataset(self, split_adata, pert_category,
                                   num_samples=1):
         """
         Combine cell graphs to create a dataset of cell graphs
         """
 
-        num_de_genes = 20
+        num_de_genes = 20        
         adata_ = split_adata[split_adata.obs['condition'] == pert_category]
-        de_genes = adata_.uns['rank_genes_groups_cov_all']
+        if 'rank_genes_groups_cov_all' in adata_.uns:
+            de_genes = adata_.uns['rank_genes_groups_cov_all']
+            de = True
+        else:
+            de = False
+            num_de_genes = 1
         Xs = []
         ys = []
 
         # When considering a non-control perturbation
         if pert_category != 'ctrl':
             # Get the indices of applied perturbation
             pert_idx = self.get_pert_idx(pert_category, adata_)
 
             # Store list of genes that are most differentially expressed for testing
             pert_de_category = adata_.obs['condition_name'][0]
-            de_idx = np.where(adata_.var_names.isin(
+            if de:
+                de_idx = np.where(adata_.var_names.isin(
                 np.array(de_genes[pert_de_category][:num_de_genes])))[0]
-
+            else:
+                de_idx = [-1] * num_de_genes
             for cell_z in adata_.X:
                 # Use samples from control as basal expression
                 ctrl_samples = self.ctrl_adata[np.random.randint(0,
                                         len(self.ctrl_adata), num_samples), :]
                 for c in ctrl_samples.X:
                     Xs.append(c)
                     ys.append(cell_z)
@@ -307,8 +388,8 @@
 
         # Create cell graphs
         cell_graphs = []
         for X, y in zip(Xs, ys):
             cell_graphs.append(self.create_cell_graph(X.toarray(),
                                 y.toarray(), de_idx, pert_category, pert_idx))
 
-        return cell_graphs
+        return cell_graphs
```

### Comparing `cell-gears-0.0.2/gears/utils.py` & `cell-gears-0.0.3/gears/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import torch
 import numpy as np
 import pandas as pd
-from sklearn.linear_model import TheilSenRegressor
-import torch.nn as nn
 import networkx as nx
 from tqdm import tqdm
 import pickle
 import sys, os
 import requests
 from torch_geometric.data import Data
-from zipfile import ZipFile 
-
-import statsmodels.api as sm
-from sklearn.linear_model import LinearRegression, TheilSenRegressor
-from dcor import distance_correlation, partial_distance_correlation
-from sklearn.metrics import r2_score
+from zipfile import ZipFile
+import tarfile
+from sklearn.linear_model import TheilSenRegressor
+from dcor import distance_correlation
+from multiprocessing import Pool
+from functools import partial
 
 def parse_single_pert(i):
     a = i.split('+')[0]
     b = i.split('+')[1]
     if a == 'ctrl':
         pert = b
     else:
@@ -81,14 +79,25 @@
     else:
         dataverse_download(url, save_path + '.zip')
         print_sys('Extracting zip file...')
         with ZipFile((save_path + '.zip'), 'r') as zip:
             zip.extractall(path = data_path)
         print_sys("Done!")  
         
+def tar_data_download_wrapper(url, save_path, data_path):
+
+    if os.path.exists(save_path):
+        print_sys('Found local copy...')
+    else:
+        dataverse_download(url, save_path + '.tar.gz')
+        print_sys('Extracting tar file...')
+        with tarfile.open(save_path  + '.tar.gz') as tar:
+            tar.extractall(path= data_path)
+        print_sys("Done!")  
+        
 def get_go_auto(gene_list, data_path, data_name):
     go_path = os.path.join(data_path, data_name, 'go.csv')
     
     if os.path.exists(go_path):
         return pd.read_csv(go_path)
     else:
         ## download gene2go.pkl
@@ -98,47 +107,58 @@
         with open(os.path.join(data_path, 'gene2go.pkl'), 'rb') as f:
             gene2go = pickle.load(f)
 
         gene2go = {i: list(gene2go[i]) for i in gene_list if i in gene2go}
         edge_list = []
         for g1 in tqdm(gene2go.keys()):
             for g2 in gene2go.keys():
-                edge_list.append((g1, g2, len(np.intersect1d(gene2go[g1], gene2go[g2]))/len(np.union1d(gene2go[g1], gene2go[g2]))))
+                edge_list.append((g1, g2, len(np.intersect1d(gene2go[g1],
+                   gene2go[g2]))/len(np.union1d(gene2go[g1], gene2go[g2]))))
 
         edge_list_filter = [i for i in edge_list if i[2] > 0]
         further_filter = [i for i in edge_list if i[2] > 0.1]
-        df_edge_list = pd.DataFrame(further_filter).rename(columns = {0: 'gene1', 1: 'gene2', 2: 'score'})
-
-        df_edge_list = df_edge_list.rename(columns = {'gene1': 'source', 'gene2': 'target', 'score': 'importance'})
+        df_edge_list = pd.DataFrame(further_filter).rename(columns = {0: 'gene1',
+                                                                      1: 'gene2',
+                                                                      2: 'score'})
+
+        df_edge_list = df_edge_list.rename(columns = {'gene1': 'source',
+                                                      'gene2': 'target',
+                                                      'score': 'importance'})
         df_edge_list.to_csv(go_path, index = False)        
         return df_edge_list
 
 def get_go(df_gene2go):
     df_gene2go['Entry name'] = df_gene2go['Entry name'].apply(lambda x: x.split('_')[0])
     df_gene2go = df_gene2go[df_gene2go['Gene ontology IDs'].notnull()]
-    df_gene2go = df_gene2go.rename(columns = {[i for i in df_gene2go.columns.values if 'yourlist' in i][0]: 'gene_id'})
+    df_gene2go = df_gene2go.rename(columns = {[i for i in df_gene2go.columns.values
+                                            if 'yourlist' in i][0]: 'gene_id'})
     geneid2go = dict(df_gene2go[['gene_id', 'Gene ontology IDs']].values)
 
     gene2go = {}
     for i,j in geneid2go.items():
         j = [k.strip() for k in j.split(';')]
         for k in i.split(','):
             gene2go[ensembl2genename[k]] = j
 
     from tqdm import tqdm
     edge_list = []
     for g1 in tqdm(gene2go.keys()):
         for g2 in gene2go.keys():
-            edge_list.append((g1, g2, len(np.intersect1d(gene2go[g1], gene2go[g2]))/len(np.union1d(gene2go[g1], gene2go[g2]))))
+            edge_list.append((g1, g2, len(np.intersect1d(gene2go[g1],
+                    gene2go[g2]))/len(np.union1d(gene2go[g1], gene2go[g2]))))
 
     edge_list_filter = [i for i in edge_list if i[2] > 0]
     further_filter = [i for i in edge_list if i[2] > 0.1]
-    df_edge_list = pd.DataFrame(further_filter).rename(columns = {0: 'gene1', 1: 'gene2', 2: 'score'})
-
-    df_edge_list = df_edge_list.rename(columns = {'gene1': 'source', 'gene2': 'target', 'score': 'importance'})
+    df_edge_list = pd.DataFrame(further_filter).rename(columns = {0: 'gene1',
+                                                                  1: 'gene2',
+                                                                  2: 'score'})
+
+    df_edge_list = df_edge_list.rename(columns = {'gene1': 'source',
+                                                  'gene2': 'target',
+                                                  'score': 'importance'})
     return df_edge_list
 
 class GeneSimNetwork():
     def __init__(self, edge_list, gene_list, node_map):
         self.edge_list = edge_list
         self.G = nx.from_pandas_edgelist(self.edge_list, source='source',
                         target='target', edge_attr=['importance'],
@@ -153,27 +173,89 @@
         self.edge_index = torch.tensor(edge_index_, dtype=torch.long).T
         #self.edge_weight = torch.Tensor(self.edge_list['importance'].values)
         
         edge_attr = nx.get_edge_attributes(self.G, 'importance') 
         importance = np.array([edge_attr[e] for e in self.G.edges])
         self.edge_weight = torch.Tensor(importance)
 
-def get_similarity_network(network_type, adata, threshold, k, gene_list, data_path, data_name, split, seed, train_gene_set_size, set2conditions):
+def get_GO_edge_list(args):
+    g1, gene2go = args
+    edge_list = []
+    for g2 in gene2go.keys():
+        score = len(gene2go[g1].intersection(gene2go[g2])) / len(
+            gene2go[g1].union(gene2go[g2]))
+        if score > 0.1:
+            edge_list.append((g1, g2, score))
+    return edge_list
+        
+def make_GO(data_path, pert_list, data_name, num_workers=25, save=True):
+    """
+    Creates Gene Ontology graph from a custom set of genes
+    """
+
+    fname = './data/go_essential_' + data_name + '.csv'
+    if os.path.exists(fname):
+        return pd.read_csv(fname)
+
+    with open(os.path.join(data_path, 'gene2go_all.pkl'), 'rb') as f:
+        gene2go = pickle.load(f)
+    gene2go = {i: gene2go[i] for i in pert_list}
+
+    print('Creating custom GO graph, this can take a few minutes')
+    with Pool(num_workers) as p:
+        all_edge_list = list(
+            tqdm(p.imap(get_GO_edge_list, ((g, gene2go) for g in gene2go.keys())),
+                      total=len(gene2go.keys())))
+    edge_list = []
+    for i in all_edge_list:
+        edge_list = edge_list + i
+
+    df_edge_list = pd.DataFrame(edge_list).rename(
+        columns={0: 'source', 1: 'target', 2: 'importance'})
+    
+    if save:
+        print('Saving edge_list to file')
+        df_edge_list.to_csv(fname, index=False)
+
+    return df_edge_list
+
+def get_similarity_network(network_type, adata, threshold, k,
+                           data_path, data_name, split, seed, train_gene_set_size,
+                           set2conditions, default_GO_graph=True, pert_list=None):
     
     if network_type == 'co-express':
-        df_out = get_coexpression_network_from_train(adata, threshold, k, data_path, data_name, split, seed, train_gene_set_size, set2conditions)
+        df_out = get_coexpression_network_from_train(adata, threshold, k,
+                                                     data_path, data_name, split,
+                                                     seed, train_gene_set_size,
+                                                     set2conditions)
     elif network_type == 'go':
-        df_jaccard = get_go_auto(gene_list, data_path, data_name)
-        df_out = df_jaccard.groupby('target').apply(lambda x: x.nlargest(k + 1,['importance'])).reset_index(drop = True)
+        if default_GO_graph:
+            server_path = 'https://dataverse.harvard.edu/api/access/datafile/6934319'
+            tar_data_download_wrapper(server_path, 
+                                     os.path.join(data_path, 'go_essential_all'),
+                                     data_path)
+            df_jaccard = pd.read_csv(os.path.join(data_path, 
+                                     'go_essential_all/go_essential_all.csv'))
+
+        else:
+            df_jaccard = make_GO(data_path, pert_list, data_name)
+
+        df_out = df_jaccard.groupby('target').apply(lambda x: x.nlargest(k + 1,
+                                    ['importance'])).reset_index(drop = True)
 
     return df_out
 
-def get_coexpression_network_from_train(adata, threshold, k, data_path, data_name, split, seed, train_gene_set_size, set2conditions):
+def get_coexpression_network_from_train(adata, threshold, k, data_path,
+                                        data_name, split, seed, train_gene_set_size,
+                                        set2conditions):
     
-    fname = os.path.join(os.path.join(data_path, data_name), split + '_' + str(seed) + '_' + str(train_gene_set_size) + '_' + str(threshold) + '_' + str(k) + '_co_expression_network.csv')
+    fname = os.path.join(os.path.join(data_path, data_name), split + '_'  +
+                         str(seed) + '_' + str(train_gene_set_size) + '_' +
+                         str(threshold) + '_' + str(k) +
+                         '_co_expression_network.csv')
     
     if os.path.exists(fname):
         return pd.read_csv(fname)
     else:
         gene_list = [f for f in adata.var.gene_name.values]
         idx2gene = dict(zip(range(len(gene_list)), gene_list)) 
         X = adata.X
@@ -192,20 +274,35 @@
         df_g = []
         for i in range(out_sort_idx.shape[0]):
             target = idx2gene[i]
             for j in range(out_sort_idx.shape[1]):
                 df_g.append((idx2gene[out_sort_idx[i, j]], target, out_sort_val[i, j]))
 
         df_g = [i for i in df_g if i[2] > threshold]
-        df_co_expression = pd.DataFrame(df_g).rename(columns = {0: 'source', 1: 'target', 2: 'importance'})
+        df_co_expression = pd.DataFrame(df_g).rename(columns = {0: 'source',
+                                                                1: 'target',
+                                                                2: 'importance'})
         df_co_expression.to_csv(fname, index = False)
         return df_co_expression
     
-
-def uncertainty_loss_fct(pred, logvar, y, perts, reg = 0.1, ctrl = None, direction_lambda = 1e-3, dict_filter = None):
+def filter_pert_in_go(condition, pert_names):
+    if condition == 'ctrl':
+        return True
+    else:
+        cond1 = condition.split('+')[0]
+        cond2 = condition.split('+')[1]
+        num_ctrl = (cond1 == 'ctrl') + (cond2 == 'ctrl')
+        num_in_perts = (cond1 in pert_names) + (cond2 in pert_names)
+        if num_ctrl + num_in_perts == 2:
+            return True
+        else:
+            return False
+        
+def uncertainty_loss_fct(pred, logvar, y, perts, reg = 0.1, ctrl = None,
+                         direction_lambda = 1e-3, dict_filter = None):
     gamma = 2                     
     perts = np.array(perts)
     losses = torch.tensor(0.0, requires_grad=True).to(pred.device)
     for p in set(perts):
         if p!= 'ctrl':
             retain_idx = dict_filter[p]
             pred_p = pred[np.where(perts==p)[0]][:, retain_idx]
@@ -213,74 +310,84 @@
             logvar_p = logvar[np.where(perts==p)[0]][:, retain_idx]
         else:
             pred_p = pred[np.where(perts==p)[0]]
             y_p = y[np.where(perts==p)[0]]
             logvar_p = logvar[np.where(perts==p)[0]]
                          
         # uncertainty based loss
-        losses += torch.sum((pred_p - y_p)**(2 + gamma) + reg * torch.exp(-logvar_p) * (pred_p - y_p)**(2 + gamma))/pred_p.shape[0]/pred_p.shape[1]
+        losses += torch.sum((pred_p - y_p)**(2 + gamma) + reg * torch.exp(
+            -logvar_p)  * (pred_p - y_p)**(2 + gamma))/pred_p.shape[0]/pred_p.shape[1]
                          
         # direction loss                 
         if p!= 'ctrl':
-            losses += torch.sum(direction_lambda * (torch.sign(y_p - ctrl[retain_idx]) - torch.sign(pred_p - ctrl[retain_idx]))**2)/pred_p.shape[0]/pred_p.shape[1]
+            losses += torch.sum(direction_lambda *
+                                (torch.sign(y_p - ctrl[retain_idx]) -
+                                 torch.sign(pred_p - ctrl[retain_idx]))**2)/\
+                                 pred_p.shape[0]/pred_p.shape[1]
         else:
-            losses += torch.sum(direction_lambda * (torch.sign(y_p - ctrl) - torch.sign(pred_p - ctrl))**2)/pred_p.shape[0]/pred_p.shape[1]
+            losses += torch.sum(direction_lambda *
+                                (torch.sign(y_p - ctrl) -
+                                 torch.sign(pred_p - ctrl))**2)/\
+                                 pred_p.shape[0]/pred_p.shape[1]
             
     return losses/(len(set(perts)))
 
 
 def loss_fct(pred, y, perts, ctrl = None, direction_lambda = 1e-3, dict_filter = None):
     gamma = 2
     mse_p = torch.nn.MSELoss()
     perts = np.array(perts)
     losses = torch.tensor(0.0, requires_grad=True).to(pred.device)
 
     for p in set(perts):
         pert_idx = np.where(perts == p)[0]
         
-        # during training, we remove the all zero genes into calculation of loss. this gives a cleaner direction loss. empirically, the performance stays the same.
+        # during training, we remove the all zero genes into calculation of loss.
+        # this gives a cleaner direction loss. empirically, the performance stays the same.
         if p!= 'ctrl':
             retain_idx = dict_filter[p]
             pred_p = pred[pert_idx][:, retain_idx]
             y_p = y[pert_idx][:, retain_idx]
         else:
             pred_p = pred[pert_idx]
             y_p = y[pert_idx]
-        
-        losses += torch.sum((pred_p - y_p)**(2 + gamma))/pred_p.shape[0]/pred_p.shape[1]
+        #losses += torch.sum((torch.mean(pred_p, 0) - y_p)**(2+gamma))/pred_p.shape[1]
+        losses = losses + torch.sum((pred_p - y_p)**(2 + gamma))/pred_p.shape[0]/pred_p.shape[1]
                          
         ## direction loss
         if (p!= 'ctrl'):
-            losses += torch.sum(direction_lambda * (torch.sign(y_p - ctrl[retain_idx]) - torch.sign(pred_p - ctrl[retain_idx]))**2)/pred_p.shape[0]/pred_p.shape[1]
+            losses = losses + torch.sum(direction_lambda *
+                                (torch.sign(y_p - ctrl[retain_idx]) -
+                                 torch.sign(pred_p - ctrl[retain_idx]))**2)/\
+                                 pred_p.shape[0]/pred_p.shape[1]
         else:
-            losses += torch.sum(direction_lambda * (torch.sign(y_p - ctrl) - torch.sign(pred_p - ctrl))**2)/pred_p.shape[0]/pred_p.shape[1]
+            losses = losses + torch.sum(direction_lambda * (torch.sign(y_p - ctrl) -
+                                                torch.sign(pred_p - ctrl))**2)/\
+                                                pred_p.shape[0]/pred_p.shape[1]
     return losses/(len(set(perts)))
 
 
 def print_sys(s):
     """system print
 
     Args:
         s (str): the string to print
     """
     print(s, flush = True, file = sys.stderr)
     
 def create_cell_graph_for_prediction(X, pert_idx, pert_gene):
 
-    # If perturbations will be represented as node features
-    pert_feats = np.zeros(len(X))
-    for p in pert_idx:
-        pert_feats[int(np.abs(p))] = np.sign(p)
-    feature_mat = torch.Tensor(np.vstack([X, pert_feats])).T
-
-    return Data(x=feature_mat, pert=pert_gene)
+    if pert_idx is None:
+        pert_idx = [-1]
+    return Data(x=torch.Tensor(X).T, pert_idx = pert_idx, pert=pert_gene)
     
 
-def create_cell_graph_dataset_for_prediction(pert_gene, ctrl_adata, gene_names, device, num_samples = 300):
-    Xs = []
+def create_cell_graph_dataset_for_prediction(pert_gene, ctrl_adata, gene_names,
+                                             device, num_samples = 300):
+
     # Get the indices (and signs) of applied perturbation
     pert_idx = [np.where(p == np.array(gene_names))[0][0] for p in pert_gene]
 
     Xs = ctrl_adata[np.random.randint(0, len(ctrl_adata), num_samples), :].X.toarray()
     # Create cell graphs
     cell_graphs = [create_cell_graph_for_prediction(X, pert_idx, pert_gene).to(device) for X in Xs]
     return cell_graphs
```

### Comparing `cell-gears-0.0.2/gears/version.py` & `cell-gears-0.0.3/gears/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '0.0.2'  # pragma: no cover
+__version__ = '0.0.3'  # pragma: no cover
```

### Comparing `cell-gears-0.0.2/setup.py` & `cell-gears-0.0.3/setup.py`

 * *Files identical despite different names*

