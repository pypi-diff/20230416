# Comparing `tmp/lycoris_lora-0.1.5.dev5.tar.gz` & `tmp/lycoris_lora-0.1.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-0.1.5.dev5.tar", last modified: Tue Apr 11 14:47:33 2023, max compression
+gzip compressed data, was "lycoris_lora-0.1.6.dev1.tar", last modified: Sun Apr 16 15:51:22 2023, max compression
```

## Comparing `lycoris_lora-0.1.5.dev5.tar` & `lycoris_lora-0.1.6.dev1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 14:47:33.751890 lycoris_lora-0.1.5.dev5/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.5.dev5/Algo.md
--rw-rw-rw-   0        0        0      552 2023-03-29 07:12:55.000000 lycoris_lora-0.1.5.dev5/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.5.dev5/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-04-11 14:47:33.751387 lycoris_lora-0.1.5.dev5/PKG-INFO
--rw-rw-rw-   0        0        0     6498 2023-04-10 10:28:19.000000 lycoris_lora-0.1.5.dev5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 14:47:33.720668 lycoris_lora-0.1.5.dev5/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.5.dev5/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.5.dev5/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.5.dev5/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.5.dev5/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.5.dev5/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.5.dev5/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.5.dev5/experiments/time_test.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:47:33.727698 lycoris_lora-0.1.5.dev5/lycoris/
--rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/lycoris/__init__.py
--rw-rw-rw-   0        0        0     5731 2023-04-11 14:46:32.000000 lycoris_lora-0.1.5.dev5/lycoris/dylora.py
--rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.5.dev5/lycoris/ia3.py
--rw-rw-rw-   0        0        0    21360 2023-04-11 04:27:42.000000 lycoris_lora-0.1.5.dev5/lycoris/kohya.py
--rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.5.dev5/lycoris/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/lycoris/kohya_utils.py
--rw-rw-rw-   0        0        0     3178 2023-04-07 16:38:33.000000 lycoris_lora-0.1.5.dev5/lycoris/locon.py
--rw-rw-rw-   0        0        0     7657 2023-04-07 16:38:27.000000 lycoris_lora-0.1.5.dev5/lycoris/loha.py
--rw-rw-rw-   0        0        0     8974 2023-04-08 05:53:19.000000 lycoris_lora-0.1.5.dev5/lycoris/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-04-10 16:04:23.000000 lycoris_lora-0.1.5.dev5/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:47:33.749383 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-04-11 14:47:33.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      773 2023-04-11 14:47:33.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 14:47:33.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-04-11 14:47:33.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 14:47:33.000000 lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.5.dev5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 14:47:33.752392 lycoris_lora-0.1.5.dev5/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-04-11 14:46:58.000000 lycoris_lora-0.1.5.dev5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:47:33.750383 lycoris_lora-0.1.5.dev5/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.5.dev5/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-04-10 15:31:09.000000 lycoris_lora-0.1.5.dev5/tools/merge.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.484260 lycoris_lora-0.1.6.dev1/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.6.dev1/Algo.md
+-rw-rw-rw-   0        0        0      552 2023-03-29 07:12:55.000000 lycoris_lora-0.1.6.dev1/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.6.dev1/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-04-16 15:51:22.484260 lycoris_lora-0.1.6.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     6498 2023-04-10 10:28:19.000000 lycoris_lora-0.1.6.dev1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.470741 lycoris_lora-0.1.6.dev1/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.6.dev1/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.6.dev1/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.6.dev1/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.6.dev1/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.6.dev1/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.6.dev1/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.6.dev1/experiments/time_test.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.475241 lycoris_lora-0.1.6.dev1/lycoris/
+-rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2514 2023-04-11 15:07:08.000000 lycoris_lora-0.1.6.dev1/lycoris/config.py
+-rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.6.dev1/lycoris/dylora.py
+-rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.6.dev1/lycoris/ia3.py
+-rw-rw-rw-   0        0        0    21664 2023-04-16 14:10:06.000000 lycoris_lora-0.1.6.dev1/lycoris/kohya.py
+-rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.6.dev1/lycoris/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/lycoris/kohya_utils.py
+-rw-rw-rw-   0        0        0     3178 2023-04-07 16:38:33.000000 lycoris_lora-0.1.6.dev1/lycoris/locon.py
+-rw-rw-rw-   0        0        0     7657 2023-04-07 16:38:27.000000 lycoris_lora-0.1.6.dev1/lycoris/loha.py
+-rw-rw-rw-   0        0        0     8974 2023-04-08 05:53:19.000000 lycoris_lora-0.1.6.dev1/lycoris/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-04-10 16:04:23.000000 lycoris_lora-0.1.6.dev1/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.483260 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 15:51:22.484260 lycoris_lora-0.1.6.dev1/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-04-16 15:51:09.000000 lycoris_lora-0.1.6.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.483760 lycoris_lora-0.1.6.dev1/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.6.dev1/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-04-10 15:31:09.000000 lycoris_lora-0.1.6.dev1/tools/merge.py
```

### Comparing `lycoris_lora-0.1.5.dev5/.gitignore` & `lycoris_lora-0.1.6.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/Algo.md` & `lycoris_lora-0.1.6.dev1/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/Change.md` & `lycoris_lora-0.1.6.dev1/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/Demo.md` & `lycoris_lora-0.1.6.dev1/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/LICENSE.md` & `lycoris_lora-0.1.6.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/README.md` & `lycoris_lora-0.1.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/experiments/better_conv.py` & `lycoris_lora-0.1.6.dev1/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/experiments/better_conv_extract.py` & `lycoris_lora-0.1.6.dev1/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/experiments/concept_neuron.py` & `lycoris_lora-0.1.6.dev1/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/experiments/locon_extract_test.py` & `lycoris_lora-0.1.6.dev1/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/experiments/locon_merge_test.py` & `lycoris_lora-0.1.6.dev1/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/experiments/singular_value_test.py` & `lycoris_lora-0.1.6.dev1/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/experiments/sparse_bias_test.py` & `lycoris_lora-0.1.6.dev1/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/experiments/time_test.py` & `lycoris_lora-0.1.6.dev1/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/lycoris/dylora.py` & `lycoris_lora-0.1.6.dev1/lycoris/dylora.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,30 +13,34 @@
     Hadamard product Implementaion for Dynamic Low Rank adaptation
     """
 
     def __init__(
         self, 
         lora_name, 
         org_module: nn.Module, 
-        multiplier=1.0, lora_dim=4, alpha=1, dropout=0.,
-        use_cp=False,
+        multiplier=1.0, 
+        lora_dim=4, alpha=1, 
+        dropout=0.,
+        use_cp=False, 
+        block_size=1,
         **kwargs,
     ):
         """ if alpha == 0 or None, alpha is rank (no scaling). """
         super().__init__()
         self.lora_name = lora_name
         self.lora_dim = lora_dim
-        self.cp=False
+        assert lora_dim % block_size == 0, 'lora_dim must be a multiple of block_size'
+        self.block_count = lora_dim//block_size
+        self.block_size = block_size
         
         self.shape = org_module.weight.shape
         if org_module.__class__.__name__ == 'Conv2d':
             in_dim = org_module.in_channels
             k_size = org_module.kernel_size
             out_dim = org_module.out_channels
-            self.cp = use_cp and k_size!=(1, 1)
             shape = (out_dim, in_dim*k_size[0]*k_size[1])
             self.op = F.conv2d
             self.extra_args = {
                 "stride": org_module.stride,
                 "padding": org_module.padding,
                 "dilation": org_module.dilation,
                 "groups": org_module.groups
@@ -124,38 +128,47 @@
 
     def apply_to(self):
         self.org_module[0].forward = self.forward
     
     def apply_train(self, b:int):
         self.up_list.requires_grad_(False)
         self.down_list.requires_grad_(False)
-        
-        self.up_list[b].copy_(self.up_update[b])
-        self.down_list[b].copy_(self.down_update[b])
-        self.up_update[self.index].copy_(self.up_list[self.index])
-        self.down_update[self.index].copy_(self.down_list[self.index])
+            
+        for i in range(self.index*self.block_size, (self.index+1)*self.block_size):
+            self.up_update[i].copy_(self.up_list[i])
+            self.down_update[i].copy_(self.down_list[i])
+        
+        for i in range(b*self.block_size, (b+1)*self.block_size):
+            self.up_list[i].copy_(self.up_update[i])
+            self.down_list[i].copy_(self.down_update[i])
         
         self.up_list.requires_grad_(True)
         self.down_list.requires_grad_(True)
-        
         self.index = b
 
     @torch.enable_grad()
     def forward(self, x):
-        b = random.randint(0, self.lora_dim-1)
+        b = random.randint(0, self.block_count-1)
         if self.up_update[b].device != self.up_list[b].device:
             device = self.up_list[b].device
             for i in range(self.lora_dim):
                 self.up_update[i] = self.up_update[i].to(device)
                 self.down_update[i] = self.down_update[i].to(device)
         
         if self.training:
             self.apply_train(b)
-        down = torch.concat(list(self.down_update[:b]) + [self.down_list[b]])
-        up = torch.concat(list(self.up_update[:b]) + [self.up_list[b]], dim=1)
+        down = torch.concat(
+            list(self.down_update[:b*self.block_size]) 
+            + list(self.down_list[b*self.block_size:(b+1)*self.block_size])
+        )
+        up = torch.concat(
+            list(self.up_update[:b*self.block_size]) 
+            + list(self.up_list[b*self.block_size:(b+1)*self.block_size]),
+            dim=1
+        )
         
         bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
         return self.op(
             x, 
             self.org_module[0].weight + (up@down).view(self.shape) * self.alpha/(b+1),
             bias,
             **self.extra_args
```

### Comparing `lycoris_lora-0.1.5.dev5/lycoris/ia3.py` & `lycoris_lora-0.1.6.dev1/lycoris/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/lycoris/kohya.py` & `lycoris_lora-0.1.6.dev1/lycoris/kohya.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 
 def create_network(multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs):
     if network_dim is None:
         network_dim = 4                     # default
     conv_dim = int(kwargs.get('conv_dim', network_dim))
     conv_alpha = float(kwargs.get('conv_alpha', network_alpha))
     dropout = float(kwargs.get('dropout', 0.))
-    algo = kwargs.get('algo', 'lora')
+    algo = kwargs.get('algo', 'lora').lower()
     use_cp = (not kwargs.get('disable_conv_cp', True) 
               or kwargs.get('use_conv_cp', False))
+    block_size = int(kwargs.get('block_size', 4))
     network_module = {
         'lora': LoConModule,
         'locon': LoConModule,
         'loha': LohaModule,
         'ia3':  IA3Module,
         'lokr': LokrModule,
         'dylora': DyLoraModule,
@@ -66,14 +67,15 @@
             lora_dim=network_dim, conv_lora_dim=conv_dim, 
             alpha=network_alpha, conv_alpha=conv_alpha,
             dropout=dropout,
             use_cp=use_cp,
             network_module=network_module,
             decompose_both=kwargs.get('decompose_both', False),
             factor=kwargs.get('factor', -1),
+            block_size = block_size
         )
     
     return network
 
 
 class LycorisNetwork(torch.nn.Module):
     '''
@@ -138,57 +140,63 @@
                 if module.__class__.__name__ in target_replace_modules:
                     for child_name, child_module in module.named_modules():
                         lora_name = prefix + '.' + name + '.' + child_name
                         lora_name = lora_name.replace('.', '_')
                         if child_module.__class__.__name__ == 'Linear' and lora_dim>0:
                             lora = network_module(
                                 lora_name, child_module, self.multiplier, 
-                                self.lora_dim, self.alpha, self.dropout, use_cp,
+                                self.lora_dim, self.alpha, 
+                                self.dropout, use_cp,
                                 **kwargs
                             )
                         elif child_module.__class__.__name__ == 'Conv2d':
                             k_size, *_ = child_module.kernel_size
                             if k_size==1 and lora_dim>0:
                                 lora = network_module(
                                     lora_name, child_module, self.multiplier, 
-                                    self.lora_dim, self.alpha, self.dropout, use_cp,
+                                    self.lora_dim, self.alpha, 
+                                    self.dropout, use_cp,
                                     **kwargs
                                 )
                             elif conv_lora_dim>0:
                                 lora = network_module(
                                     lora_name, child_module, self.multiplier, 
-                                    self.conv_lora_dim, self.conv_alpha, self.dropout, use_cp,
+                                    self.conv_lora_dim, self.conv_alpha, 
+                                    self.dropout, use_cp,
                                     **kwargs
                                 )
                             else:
                                 continue
                         else:
                             continue
                         loras.append(lora)
                 elif name in target_replace_names:
                     lora_name = prefix + '.' + name
                     lora_name = lora_name.replace('.', '_')
                     if module.__class__.__name__ == 'Linear' and lora_dim>0:
                         lora = network_module(
                             lora_name, module, self.multiplier, 
-                            self.lora_dim, self.alpha, self.dropout, use_cp,
+                            self.lora_dim, self.alpha, 
+                            self.dropout, use_cp,
                             **kwargs
                         )
                     elif module.__class__.__name__ == 'Conv2d':
                         k_size, *_ = module.kernel_size
                         if k_size==1 and lora_dim>0:
                             lora = network_module(
                                 lora_name, module, self.multiplier, 
-                                self.lora_dim, self.alpha, self.dropout, use_cp,
+                                self.lora_dim, self.alpha, 
+                                self.dropout, use_cp,
                                 **kwargs
                             )
                         elif conv_lora_dim>0:
                             lora = network_module(
                                 lora_name, module, self.multiplier, 
-                                self.conv_lora_dim, self.conv_alpha, self.dropout, use_cp,
+                                self.conv_lora_dim, self.conv_alpha, 
+                                self.dropout, use_cp,
                                 **kwargs
                             )
                         else:
                             continue
                     else:
                         continue
                     loras.append(lora)
```

### Comparing `lycoris_lora-0.1.5.dev5/lycoris/kohya_model_utils.py` & `lycoris_lora-0.1.6.dev1/lycoris/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/lycoris/kohya_utils.py` & `lycoris_lora-0.1.6.dev1/lycoris/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/lycoris/locon.py` & `lycoris_lora-0.1.6.dev1/lycoris/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/lycoris/loha.py` & `lycoris_lora-0.1.6.dev1/lycoris/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/lycoris/lokr.py` & `lycoris_lora-0.1.6.dev1/lycoris/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/lycoris/utils.py` & `lycoris_lora-0.1.6.dev1/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 experiments/concept_neuron.py
 experiments/locon_extract_test.py
 experiments/locon_merge_test.py
 experiments/singular_value_test.py
 experiments/sparse_bias_test.py
 experiments/time_test.py
 lycoris/__init__.py
+lycoris/config.py
 lycoris/dylora.py
 lycoris/ia3.py
 lycoris/kohya.py
 lycoris/kohya_model_utils.py
 lycoris/kohya_utils.py
 lycoris/locon.py
 lycoris/loha.py
```

### Comparing `lycoris_lora-0.1.5.dev5/setup.py` & `lycoris_lora-0.1.6.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='0.1.5-dev5',
+    version='0.1.6.dev1',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-0.1.5.dev5/tools/extract_locon.py` & `lycoris_lora-0.1.6.dev1/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.5.dev5/tools/merge.py` & `lycoris_lora-0.1.6.dev1/tools/merge.py`

 * *Files identical despite different names*

