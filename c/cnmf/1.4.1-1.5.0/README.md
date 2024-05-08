# Comparing `tmp/cnmf-1.4.1.tar.gz` & `tmp/cnmf-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dkotliar/Desktop/cNMF/dist/.tmp-ucr4qfcj/cnmf-1.4.1.tar", last modified: Wed Dec 13 18:08:34 2023, max compression
+gzip compressed data, was "cnmf-1.5.0.tar", last modified: Wed May  8 01:43:24 2024, max compression
```

## Comparing `cnmf-1.4.1.tar` & `cnmf-1.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2023-12-13 18:08:34.000000 cnmf-1.4.1/
--rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2023-12-13 16:47:35.000000 cnmf-1.4.1/LICENSE
--rw-r--r--   0 dkotliar   (503) staff       (20)    17404 2023-12-13 18:08:34.000000 cnmf-1.4.1/PKG-INFO
--rw-r--r--   0 dkotliar   (503) staff       (20)    16946 2023-12-13 18:05:11.000000 cnmf-1.4.1/README.md
--rw-r--r--   0 dkotliar   (503) staff       (20)      103 2023-12-13 16:47:35.000000 cnmf-1.4.1/pyproject.toml
--rw-r--r--   0 dkotliar   (503) staff       (20)       38 2023-12-13 18:08:34.000000 cnmf-1.4.1/setup.cfg
--rw-r--r--   0 dkotliar   (503) staff       (20)     1016 2023-12-13 18:03:30.000000 cnmf-1.4.1/setup.py
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2023-12-13 18:08:34.000000 cnmf-1.4.1/src/
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2023-12-13 18:08:34.000000 cnmf-1.4.1/src/cnmf/
--rw-r--r--   0 dkotliar   (503) staff       (20)       28 2023-12-13 16:47:35.000000 cnmf-1.4.1/src/cnmf/__init__.py
--rwxr-xr-x   0 dkotliar   (503) staff       (20)    50559 2023-12-13 17:05:25.000000 cnmf-1.4.1/src/cnmf/cnmf.py
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2023-12-13 18:08:34.000000 cnmf-1.4.1/src/cnmf.egg-info/
--rw-r--r--   0 dkotliar   (503) staff       (20)    17404 2023-12-13 18:08:34.000000 cnmf-1.4.1/src/cnmf.egg-info/PKG-INFO
--rw-r--r--   0 dkotliar   (503) staff       (20)      273 2023-12-13 18:08:34.000000 cnmf-1.4.1/src/cnmf.egg-info/SOURCES.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)        1 2023-12-13 18:08:34.000000 cnmf-1.4.1/src/cnmf.egg-info/dependency_links.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)       35 2023-12-13 18:08:34.000000 cnmf-1.4.1/src/cnmf.egg-info/entry_points.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)       85 2023-12-13 18:08:34.000000 cnmf-1.4.1/src/cnmf.egg-info/requires.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)        5 2023-12-13 18:08:34.000000 cnmf-1.4.1/src/cnmf.egg-info/top_level.txt
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 01:43:24.434764 cnmf-1.5.0/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2024-05-07 19:11:38.000000 cnmf-1.5.0/LICENSE
+-rw-r--r--   0 dkotliar   (503) staff       (20)     9225 2024-05-08 01:43:24.433735 cnmf-1.5.0/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)     8519 2024-05-08 00:36:16.000000 cnmf-1.5.0/README.md
+-rw-r--r--   0 dkotliar   (503) staff       (20)      103 2024-05-07 19:11:38.000000 cnmf-1.5.0/pyproject.toml
+-rw-r--r--   0 dkotliar   (503) staff       (20)       38 2024-05-08 01:43:24.434978 cnmf-1.5.0/setup.cfg
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1035 2024-05-07 21:44:08.000000 cnmf-1.5.0/setup.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 01:43:24.424611 cnmf-1.5.0/src/
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 01:43:24.429215 cnmf-1.5.0/src/cnmf/
+-rw-r--r--   0 dkotliar   (503) staff       (20)       97 2024-05-07 19:12:10.000000 cnmf-1.5.0/src/cnmf/__init__.py
+-rwxr-xr-x   0 dkotliar   (503) staff       (20)    52529 2024-05-07 21:33:04.000000 cnmf-1.5.0/src/cnmf/cnmf.py
+-rw-r--r--   0 dkotliar   (503) staff       (20)    20172 2024-05-08 00:41:00.000000 cnmf-1.5.0/src/cnmf/preprocess.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 01:43:24.433030 cnmf-1.5.0/src/cnmf.egg-info/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     9225 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)      296 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/SOURCES.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        1 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/dependency_links.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       35 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/entry_points.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       98 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/requires.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        5 2024-05-08 01:43:24.000000 cnmf-1.5.0/src/cnmf.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cnmf-1.4.1/LICENSE` & `cnmf-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmf-1.4.1/setup.py` & `cnmf-1.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cnmf",
-    version="1.4.1",
+    version="1.5.0",
     author="Dylan Kotliar",
     author_email="dylkot@gmail.com",
     description="Consensus NMF for scRNA-Seq data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dylkot/cNMF",
     project_urls={
@@ -25,14 +25,15 @@
     entry_points={
         'console_scripts': [
             'cnmf = cnmf:main',
         ],
     },
     install_requires=[
    'scikit-learn>=1.0',
+   'anndata>=0.9',
    'scanpy',
    'pandas',
    'numpy',
    'fastcluster',
    'matplotlib',
    'palettable',
    'scipy',
```

### Comparing `cnmf-1.4.1/src/cnmf/cnmf.py` & `cnmf-1.5.0/src/cnmf/cnmf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import numpy as np
 import pandas as pd
-import os, errno
+import os, errno, sys
 import datetime
 import uuid
 import itertools
 import yaml
 import subprocess
 import scipy.sparse as sp
 
@@ -179,15 +179,15 @@
 
 
 def compute_tpm(input_counts):
     """
     Default TPM normalization
     """
     tpm = input_counts.copy()
-    sc.pp.normalize_per_cell(tpm, counts_per_cell_after=1e6)
+    sc.pp.normalize_total(tpm, target_sum=1e6)
     return(tpm)
 
 
 def factorize_mp_signature(args):
     """
     wrapper around factorize to be able to use mp pool.
     args is a list:
@@ -261,15 +261,15 @@
                 'k_selection_plot' :  os.path.join(self.output_dir, self.name, self.name+'.k_selection.png'),
                 'k_selection_stats' :  os.path.join(self.output_dir, self.name, self.name+'.k_selection_stats.df.npz'),
             }
 
 
     def prepare(self, counts_fn, components, n_iter = 100, densify=False, tpm_fn=None, seed=None,
                         beta_loss='frobenius',num_highvar_genes=2000, genes_file=None,
-                        alpha_usage=0.0, alpha_spectra=0.0, init='random'):
+                        alpha_usage=0.0, alpha_spectra=0.0, init='random', max_NMF_iter=1000):
         """
         Load input counts, reduce to high-variance genes, and variance normalize genes.
         Prepare file for distributing jobs over workers.
 
 
         Parameters
         ----------
@@ -301,14 +301,17 @@
             If provided will load high-variance genes from a list of these genes
             
         alpha_usage : float, optional (default=0.0)
             Regularization parameter for NMF corresponding to alpha_W in scikit-learn
 
         alpha_spectra : float, optional (default=0.0)
             Regularization parameter for NMF corresponding to alpha_H in scikit-learn
+
+        max_NMF_iter : int, optional (default=1000)
+            Maximum number of iterations per individual NMF run
         """
         
         
         if counts_fn.endswith('.h5ad'):
             input_counts = sc.read(counts_fn)
         else:
             ## Load txt or compressed dataframe and convert to scanpy object
@@ -372,15 +375,15 @@
 
         norm_counts = self.get_norm_counts(input_counts, tpm, num_highvar_genes=num_highvar_genes,
                                                high_variance_genes_filter=highvargenes)
 
         self.save_norm_counts(norm_counts)
         (replicate_params, run_params) = self.get_nmf_iter_params(ks=components, n_iter=n_iter, random_state_seed=seed,
                                                                   beta_loss=beta_loss, alpha_usage=alpha_usage,
-                                                                  alpha_spectra=alpha_spectra, init=init)
+                                                                  alpha_spectra=alpha_spectra, init=init, max_iter=max_NMF_iter)
         self.save_nmf_iter_params(replicate_params, run_params)
         
     
     def combine(self, components=None, skip_missing_files=False):
         """
         Combine NMF iterations for the same value of K
         Parameters
@@ -463,15 +466,15 @@
             if np.isnan(norm_counts.X).sum().sum() > 0:
                 print('Warning NaNs in normalized counts matrix')                    
         
         ## Save a \n-delimited list of the high-variance genes used for factorization
         open(self.paths['nmf_genes_list'], 'w').write('\n'.join(high_variance_genes_filter))
 
         ## Check for any cells that have 0 counts of the overdispersed genes
-        zerocells = norm_counts.X.sum(axis=1)==0
+        zerocells = np.array(norm_counts.X.sum(axis=1)==0).reshape(-1)
         if zerocells.sum()>0:
             examples = norm_counts.obs.index[np.ravel(zerocells)]
             raise Exception('Error: %d cells have zero counts of overdispersed genes. E.g. %s. Filter those cells and re-run or adjust the number of overdispersed genes. Quitting!' % (zerocells.sum(), ', '.join(examples[:4])))
         
         return(norm_counts)
 
     
@@ -480,15 +483,15 @@
         sc.write(self.paths['normalized_counts'], norm_counts)
 
         
     def get_nmf_iter_params(self, ks, n_iter = 100,
                                random_state_seed = None,
                                beta_loss = 'kullback-leibler',
                                alpha_usage=0.0, alpha_spectra=0.0,
-                               init='random'):
+                               init='random', max_iter=1000):
         """
         Create a DataFrame with parameters for NMF iterations.
 
 
         Parameters
         ----------
         ks : integer, or list-like.
@@ -514,29 +517,29 @@
 
         # Remove any repeated k values, and order.
         k_list = sorted(set(list(ks)))
 
         n_runs = len(ks)* n_iter
 
         np.random.seed(seed=random_state_seed)
-        nmf_seeds = np.random.randint(low=1, high=(2**32)-1, size=n_runs)
+        nmf_seeds = np.random.randint(low=1, high=(2**31)-1, size=n_runs)
 
         replicate_params = []
         for i, (k, r) in enumerate(itertools.product(k_list, range(n_iter))):
             replicate_params.append([k, r, nmf_seeds[i]])
         replicate_params = pd.DataFrame(replicate_params, columns = ['n_components', 'iter', 'nmf_seed'])
 
         _nmf_kwargs = dict(
                         alpha_W=alpha_usage,
                         alpha_H=alpha_spectra,
                         l1_ratio=0.0,
                         beta_loss=beta_loss,
                         solver='mu',
                         tol=1e-4,
-                        max_iter=1000,
+                        max_iter=max_iter,
                         init=init
                         )
         
         ## Coordinate descent is faster than multiplicative update but only works for frobenius
         if beta_loss == 'frobenius':
             _nmf_kwargs['solver'] = 'cd'
 
@@ -704,15 +707,15 @@
             Non-negative spectra of expression programs
         """
         return(self.refit_usage(X.T, usage.T).T)
 
 
     def consensus(self, k, density_threshold=0.5, local_neighborhood_size = 0.30,show_clustering = True,
                   skip_density_and_return_after_stats = False, close_clustergram_fig=False,
-                  refit_usage=True):
+                  refit_usage=True, normalize_tpm_spectra=False, norm_counts=None):
         """
         Obtain consensus estimates of spectra and usages from a cNMF run and output a clustergram of
         the consensus matrix. Assumes prepare, factorize, and combine steps have already been run.
 
 
         Parameters
         ----------
@@ -732,21 +735,32 @@
             True when running k_selection_plot to compute stability and error for input parameters without computing
             consensus spectra and usages
             
         close_clustergram_fig : boolean (default=False)
             If True, closes the clustergram figure from output after saving the image to a file
             
         refit_usage : boolean (default=True)
-            If True, refit the usage matrix one final time after finalizing the spectra_tpm matrix. Has been shown
-            to increase inference accuracy in simulations.
+            If True, refit the usage matrix one final time after finalizing the spectra_tpm matrix. Done by regressing 
+            the tpm matrix against the tpm_spectra including only high-variance genes and with both the tpm matrix
+            and tpm_spectra normalized by the standard deviations of the genes in tpm scale.
+            
+        normalize_tpm_spectra : boolean (default=False)
+            If True, renormalizes the tpm_spectra to sum to 1e6 for each program. This is done before refitting usages.
+            If not used, the tpm_spectra are exactly as calcuated when refitting the usage matrix against the tpm matrix
+            and typically will not sum to the same value for each program.
+            
+        norm_counts : AnnData (default=None)
+            Speed up calculation of k_selection_plot by avoiding reloading norm_counts for each K. Should not be used by
+            most users
         """
         
         
         merged_spectra = load_df_from_npz(self.paths['merged_spectra']%k)
-        norm_counts = sc.read(self.paths['normalized_counts'])
+        if norm_counts is None:
+            norm_counts = sc.read(self.paths['normalized_counts'])
 
         density_threshold_str = str(density_threshold)
         if skip_density_and_return_after_stats:
             density_threshold_str = '2'
         density_threshold_repl = density_threshold_str.replace('.', '_')
         n_neighbors = int(local_neighborhood_size * merged_spectra.shape[0]/k)
 
@@ -783,56 +797,53 @@
 
         # Find median usage for each gene across cluster
         median_spectra = l2_spectra.groupby(kmeans_cluster_labels).median()
 
         # Normalize median spectra to probability distributions.
         median_spectra = (median_spectra.T/median_spectra.sum(1)).T
 
-        # Compute the silhouette score
-        if len(np.unique(kmeans_cluster_labels)) == len(kmeans_cluster_labels):
-            stability = 0
-        else:
-            stability = silhouette_score(l2_spectra.values, kmeans_cluster_labels, metric='euclidean')
-
         # Obtain reconstructed count matrix by re-fitting usage and computing dot product: usage.dot(spectra)
         rf_usages = self.refit_usage(norm_counts.X, median_spectra)
         rf_usages = pd.DataFrame(rf_usages, index=norm_counts.obs.index, columns=median_spectra.index)        
-        rf_pred_norm_counts = rf_usages.dot(median_spectra)
+        
+        if skip_density_and_return_after_stats:
+            silhouette = silhouette_score(l2_spectra.values, kmeans_cluster_labels, metric='euclidean')
+            
+            # Compute prediction error as a frobenius norm
+            rf_pred_norm_counts = rf_usages.dot(median_spectra)        
+            if sp.issparse(norm_counts.X):
+                prediction_error = ((norm_counts.X.todense() - rf_pred_norm_counts)**2).sum().sum()
+            else:
+                prediction_error = ((norm_counts.X - rf_pred_norm_counts)**2).sum().sum()    
+                
+            consensus_stats = pd.DataFrame([k, density_threshold, silhouette,  prediction_error],
+                    index = ['k', 'local_density_threshold', 'silhouette', 'prediction_error'],
+                    columns = ['stats'])
+
+            return(consensus_stats)           
         
         # Re-order usage by total contribution
         norm_usages = rf_usages.div(rf_usages.sum(axis=1), axis=0)      
         reorder = norm_usages.sum(axis=0).sort_values(ascending=False)
         rf_usages = rf_usages.loc[:, reorder.index]
         norm_usages = norm_usages.loc[:, reorder.index]
         median_spectra = median_spectra.loc[reorder.index, :]
         rf_usages.columns = np.arange(1, rf_usages.shape[1]+1)
         norm_usages.columns = rf_usages.columns
         median_spectra.index = rf_usages.columns
-
-        # Compute prediction error as a frobenius norm
-        if sp.issparse(norm_counts.X):
-            prediction_error = ((norm_counts.X.todense() - rf_pred_norm_counts)**2).sum().sum()
-        else:
-            prediction_error = ((norm_counts.X - rf_pred_norm_counts)**2).sum().sum()
-        
-        consensus_stats = pd.DataFrame([k, density_threshold, stability, prediction_error],
-                    index = ['k', 'local_density_threshold', 'stability', 'prediction_error'],
-                    columns = ['stats'])
-
-        if skip_density_and_return_after_stats:
-            return consensus_stats
         
         # Convert spectra to TPM units, and obtain results for all genes by running last step of NMF
         # with usages fixed and TPM as the input matrix
         tpm = sc.read(self.paths['tpm'])
         tpm_stats = load_df_from_npz(self.paths['tpm_stats'])
         spectra_tpm = self.refit_spectra(tpm.X, norm_usages.astype(tpm.X.dtype))
         spectra_tpm = pd.DataFrame(spectra_tpm, index=rf_usages.columns, columns=tpm.var.index)
-        spectra_tpm = spectra_tpm.div(spectra_tpm.sum(axis=1), axis=0) * 1e6
-        
+        if normalize_tpm_spectra:
+            spectra_tpm = spectra_tpm.div(spectra_tpm.sum(axis=1), axis=0) * 1e6
+                    
         # Convert spectra to Z-score units, and obtain results for all genes by running last step of NMF
         # with usages fixed and Z-scored TPM as the input matrix
         if sp.issparse(tpm.X):
             norm_tpm = (np.array(tpm.X.todense()) - tpm_stats['__mean'].values) / tpm_stats['__std'].values
         else:
             norm_tpm = (tpm.X - tpm_stats['__mean'].values) / tpm_stats['__std'].values
         
@@ -848,20 +859,20 @@
                 sc.pp.scale(norm_tpm, zero_center=False)                       
             else:
                 norm_tpm.X /= norm_tpm.X.std(axis=0, ddof=1)
                 
             spectra_tpm_rf = spectra_tpm.loc[:,hvgs]
 
             spectra_tpm_rf = spectra_tpm_rf.div(tpm_stats.loc[hvgs, '__std'], axis=1)
-            rf_usages = self.refit_usage(norm_tpm.X, spectra_tpm_rf)
+            rf_usages = self.refit_usage(norm_tpm.X, spectra_tpm_rf.astype(norm_tpm.X.dtype))
             rf_usages = pd.DataFrame(rf_usages, index=norm_counts.obs.index, columns=spectra_tpm_rf.index)                                                                  
                
         save_df_to_npz(median_spectra, self.paths['consensus_spectra']%(k, density_threshold_repl))
         save_df_to_npz(rf_usages, self.paths['consensus_usages']%(k, density_threshold_repl))
-        save_df_to_npz(consensus_stats, self.paths['consensus_stats']%(k, density_threshold_repl))
+        #save_df_to_npz(consensus_stats, self.paths['consensus_stats']%(k, density_threshold_repl))
         save_df_to_text(median_spectra, self.paths['consensus_spectra__txt']%(k, density_threshold_repl))
         save_df_to_text(rf_usages, self.paths['consensus_usages__txt']%(k, density_threshold_repl))
         save_df_to_npz(spectra_tpm, self.paths['gene_spectra_tpm']%(k, density_threshold_repl))
         save_df_to_text(spectra_tpm, self.paths['gene_spectra_tpm__txt']%(k, density_threshold_repl))
         save_df_to_npz(usage_coef, self.paths['gene_spectra_score']%(k, density_threshold_repl))
         save_df_to_text(usage_coef, self.paths['gene_spectra_score__txt']%(k, density_threshold_repl))
         if show_clustering:
@@ -963,30 +974,31 @@
     def k_selection_plot(self, close_fig=False):
         '''
         Borrowed from Alexandrov Et Al. 2013 Deciphering Mutational Signatures
         publication in Cell Reports
         '''
         run_params = load_df_from_npz(self.paths['nmf_replicate_parameters'])
         stats = []
+        norm_counts = sc.read(self.paths['normalized_counts'])
         for k in sorted(set(run_params.n_components)):
-
             stats.append(self.consensus(k, skip_density_and_return_after_stats=True,
-                                        show_clustering=False, close_clustergram_fig=True).stats)
+                                        show_clustering=False, close_clustergram_fig=True,
+                                        norm_counts=norm_counts).stats)
 
         stats = pd.DataFrame(stats)
         stats.reset_index(drop = True, inplace = True)
 
         save_df_to_npz(stats, self.paths['k_selection_stats'])
 
         fig = plt.figure(figsize=(6, 4))
         ax1 = fig.add_subplot(111)
         ax2 = ax1.twinx()
 
 
-        ax1.plot(stats.k, stats.stability, 'o-', color='b')
+        ax1.plot(stats.k, stats.silhouette, 'o-', color='b')
         ax1.set_ylabel('Stability', color='b', fontsize=15)
         for tl in ax1.get_yticklabels():
             tl.set_color('b')
         #ax1.set_xlabel('K', fontsize=15)
 
         ax2.plot(stats.k, stats.prediction_error, 'o-', color='r')
         ax2.set_ylabel('Error', color='r', fontsize=15)
@@ -997,35 +1009,52 @@
         ax1.grid('on')
         plt.tight_layout()
         fig.savefig(self.paths['k_selection_plot'], dpi=250)
         if close_fig:
             plt.close(fig)
             
             
-    def load_results(self, K, density_threshold, n_top_genes=100):
+    def load_results(self, K, density_threshold, n_top_genes=100, norm_usage = True):
         """
         Loads normalized usages and gene_spectra_scores for a given choice of K and 
         local_density_threshold for the cNMF run. Additionally returns a DataFrame of
-        the top genes linked to each program with the number of genes indicated by the
-        `n_top_genes` parameter
+        the top genes linked to each program
+        
+        Parameters
+        ----------
+        K : int
+            Number of programs (must be within the k values specified in previous steps)
+
+        density_threshold : float
+            Threshold for filtering outlier spectra (must be within the values specified in consensus step)
+
+        n_top_genes : integer, optional (default=100)
+            Number of top genes per program to return
+
+        norm_usage : boolean, optional (default=True)
+            If True, normalize cNMF usages to sum to 1
         
         Returns
-        usage - cNMF usages (cells X K) normalized to sum to 1
-        spectra - Z-score regressed coeffecients for each program (K x genes) with higher values cooresponding
+        ----------
+        usage - cNMF usages (cells X K)
+        spectra_scores - Z-score coeffecients for each program (K x genes) with high values cooresponding
                     to better marker genes
+        spectra_tpm - Coeffecients for contribution of each gene to each program (K x genes) in TPM units
         top_genes - ranked list of marker genes per GEP (n_top_genes X K)
         """
         scorefn = self.paths['gene_spectra_score__txt'] % (K, str(density_threshold).replace('.', '_'))
         tpmfn = self.paths['gene_spectra_tpm__txt'] % (K, str(density_threshold).replace('.', '_'))
         usagefn = self.paths['consensus_usages__txt'] % (K, str(density_threshold).replace('.', '_'))
         spectra_scores = pd.read_csv(scorefn, sep='\t', index_col=0).T
         spectra_tpm = pd.read_csv(tpmfn, sep='\t', index_col=0).T
 
         usage = pd.read_csv(usagefn, sep='\t', index_col=0)
-        usage = usage.div(usage.sum(axis=1), axis=0)
+        
+        if norm_usage:
+            usage = usage.div(usage.sum(axis=1), axis=0)
         
         try:
             usage.columns = [int(x) for x in usage.columns]
         except:
             print('Usage matrix columns include non integer values')
     
         top_genes = []
@@ -1063,35 +1092,36 @@
     parser = argparse.ArgumentParser()
 
     parser.add_argument('command', type=str, choices=['prepare', 'factorize', 'combine', 'consensus', 'k_selection_plot'])
     parser.add_argument('--name', type=str, help='[all] Name for analysis. All output will be placed in [output-dir]/[name]/...', nargs='?', default='cNMF')
     parser.add_argument('--output-dir', type=str, help='[all] Output directory. All output will be placed in [output-dir]/[name]/...', nargs='?', default='.')
     parser.add_argument('-c', '--counts', type=str, help='[prepare] Input (cell x gene) counts matrix as df.npz or tab delimited text file')
     parser.add_argument('-k', '--components', type=int, help='[prepare] Numper of components (k) for matrix factorization. Several can be specified with "-k 8 9 10"', nargs='+')
-    parser.add_argument('-n', '--n-iter', type=int, help='[prepare] Numper of factorization replicates', default=100)
+    parser.add_argument('-n', '--n-iter', type=int, help='[prepare] Number of factorization replicates', default=100)
     parser.add_argument('--total-workers', type=int, help='[all] Total number of workers to distribute jobs to', default=1)
     parser.add_argument('--seed', type=int, help='[prepare] Seed for pseudorandom number generation', default=None)
     parser.add_argument('--genes-file', type=str, help='[prepare] File containing a list of genes to include, one gene per line. Must match column labels of counts matrix.', default=None)
     parser.add_argument('--numgenes', type=int, help='[prepare] Number of high variance genes to use for matrix factorization.', default=2000)
     parser.add_argument('--tpm', type=str, help='[prepare] Pre-computed (cell x gene) TPM values as df.npz or tab separated txt file. If not provided TPM will be calculated automatically', default=None)
-    parser.add_argument('--beta-loss', type=str, choices=['frobenius', 'kullback-leibler', 'itakura-saito'], help='[prepare] Loss function for NMF.', default='frobenius')
-    parser.add_argument('--init', type=str, choices=['random', 'nndsvd'], help='[prepare] Initialization algorithm for NMF.', default='random')
-    parser.add_argument('--densify', dest='densify', help='[prepare] Treat the input data as non-sparse', action='store_true', default=False) 
+    parser.add_argument('--max-nmf-iter', type=int, help='[prepare] Max number of iterations per individual NMF run (default 1000)', default=1000)
+    parser.add_argument('--beta-loss', type=str, choices=['frobenius', 'kullback-leibler', 'itakura-saito'], help='[prepare] Loss function for NMF (default frobenius)', default='frobenius')
+    parser.add_argument('--init', type=str, choices=['random', 'nndsvd'], help='[prepare] Initialization algorithm for NMF (default random)', default='random')
+    parser.add_argument('--densify', dest='densify', help='[prepare] Treat the input data as non-sparse (default False)', action='store_true', default=False) 
     parser.add_argument('--worker-index', type=int, help='[factorize] Index of current worker (the first worker should have index 0)', default=0)
     parser.add_argument('--local-density-threshold', type=float, help='[consensus] Threshold for the local density filtering. This string must convert to a float >0 and <=2', default=0.5)
     parser.add_argument('--local-neighborhood-size', type=float, help='[consensus] Fraction of the number of replicates to use as nearest neighbors for local density filtering', default=0.30)
     parser.add_argument('--show-clustering', dest='show_clustering', help='[consensus] Produce a clustergram figure summarizing the spectra clustering', action='store_true')
-
+    
     args = parser.parse_args()
 
     cnmf_obj = cNMF(output_dir=args.output_dir, name=args.name)
     
     if args.command == 'prepare':
         cnmf_obj.prepare(args.counts, components=args.components, n_iter=args.n_iter, densify=args.densify,
-                         tpm_fn=args.tpm, seed=args.seed, beta_loss=args.beta_loss,
+                         tpm_fn=args.tpm, seed=args.seed, beta_loss=args.beta_loss, max_NMF_iter=args.max_nmf_iter,
                          num_highvar_genes=args.numgenes, genes_file=args.genes_file, init=args.init)
 
     elif args.command == 'factorize':
         cnmf_obj.factorize(worker_i=args.worker_index, total_workers=args.total_workers)
 
     elif args.command == 'combine':
         cnmf_obj.combine(components=args.components)
```

