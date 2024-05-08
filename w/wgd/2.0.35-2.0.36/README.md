# Comparing `tmp/wgd-2.0.35.tar.gz` & `tmp/wgd-2.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wgd-2.0.35.tar", last modified: Wed May  1 10:50:20 2024, max compression
+gzip compressed data, was "dist/wgd-2.0.36.tar", last modified: Wed May  8 15:26:48 2024, max compression
```

## Comparing `wgd-2.0.35.tar` & `wgd-2.0.36.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2024-05-01 10:50:20.623255 wgd-2.0.35/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.35/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    97683 2024-05-01 10:50:20.623255 wgd-2.0.35/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    97445 2024-05-01 07:38:13.000000 wgd-2.0.35/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)    62375 2024-05-01 10:49:12.000000 wgd-2.0.35/cli.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2024-05-01 10:50:20.623255 wgd-2.0.35/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1949 2024-05-01 10:49:22.000000 wgd-2.0.35/setup.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2024-05-01 10:50:20.448243 wgd-2.0.35/test/
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-06-06 22:05:06.000000 wgd-2.0.35/test/test_core.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2024-05-01 10:50:20.607399 wgd-2.0.35/wgd/
--rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.35/wgd/__init__.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.35/wgd/beast.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.35/wgd/cluster.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    12579 2023-11-20 15:14:14.000000 wgd-2.0.35/wgd/codeml.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   157655 2024-04-22 13:37:59.000000 wgd-2.0.35/wgd/core.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17245 2024-04-22 09:47:26.000000 wgd-2.0.35/wgd/mcmctree.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.35/wgd/mix.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   120060 2024-05-01 09:43:52.000000 wgd-2.0.35/wgd/peak.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4722 2023-06-06 22:05:06.000000 wgd-2.0.35/wgd/postplot.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    54236 2024-04-16 08:22:14.000000 wgd-2.0.35/wgd/ratecorrect.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    18305 2024-03-04 04:24:50.000000 wgd-2.0.35/wgd/syn.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    21638 2023-10-09 15:32:16.000000 wgd-2.0.35/wgd/tree.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    31523 2023-06-23 20:25:14.000000 wgd-2.0.35/wgd/utils.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   176151 2024-05-01 10:43:46.000000 wgd-2.0.35/wgd/viz.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2024-05-01 10:50:20.623255 wgd-2.0.35/wgd.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    97683 2024-05-01 10:50:20.000000 wgd-2.0.35/wgd.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      416 2024-05-01 10:50:20.000000 wgd-2.0.35/wgd.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2024-05-01 10:50:20.000000 wgd-2.0.35/wgd.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2024-05-01 10:50:20.000000 wgd-2.0.35/wgd.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      774 2024-05-01 10:50:20.000000 wgd-2.0.35/wgd.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2024-05-01 10:50:20.000000 wgd-2.0.35/wgd.egg-info/top_level.txt
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2024-05-08 15:26:48.864812 wgd-2.0.36/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.36/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    97683 2024-05-08 15:26:48.864812 wgd-2.0.36/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    97445 2024-05-01 07:38:13.000000 wgd-2.0.36/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    62375 2024-05-01 10:49:12.000000 wgd-2.0.36/cli.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2024-05-08 15:26:48.864812 wgd-2.0.36/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1949 2024-05-08 15:26:21.000000 wgd-2.0.36/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2024-05-08 15:26:48.707654 wgd-2.0.36/test/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-06-06 22:05:06.000000 wgd-2.0.36/test/test_core.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2024-05-08 15:26:48.849295 wgd-2.0.36/wgd/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.36/wgd/__init__.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.36/wgd/beast.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.36/wgd/cluster.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    12579 2023-11-20 15:14:14.000000 wgd-2.0.36/wgd/codeml.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   157655 2024-04-22 13:37:59.000000 wgd-2.0.36/wgd/core.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17245 2024-04-22 09:47:26.000000 wgd-2.0.36/wgd/mcmctree.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.36/wgd/mix.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   121315 2024-05-03 06:53:28.000000 wgd-2.0.36/wgd/peak.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4722 2023-06-06 22:05:06.000000 wgd-2.0.36/wgd/postplot.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    54236 2024-04-16 08:22:14.000000 wgd-2.0.36/wgd/ratecorrect.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    18305 2024-03-04 04:24:50.000000 wgd-2.0.36/wgd/syn.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    21638 2023-10-09 15:32:16.000000 wgd-2.0.36/wgd/tree.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31523 2023-06-23 20:25:14.000000 wgd-2.0.36/wgd/utils.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   176151 2024-05-01 10:43:46.000000 wgd-2.0.36/wgd/viz.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2024-05-08 15:26:48.864812 wgd-2.0.36/wgd.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    97683 2024-05-08 15:26:48.000000 wgd-2.0.36/wgd.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      416 2024-05-08 15:26:48.000000 wgd-2.0.36/wgd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2024-05-08 15:26:48.000000 wgd-2.0.36/wgd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2024-05-08 15:26:48.000000 wgd-2.0.36/wgd.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      774 2024-05-08 15:26:48.000000 wgd-2.0.36/wgd.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2024-05-08 15:26:48.000000 wgd-2.0.36/wgd.egg-info/top_level.txt
```

### Comparing `wgd-2.0.35/LICENSE` & `wgd-2.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/PKG-INFO` & `wgd-2.0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7767 640a  : 2.1.Name: wgd.
-00000020: 5665 7273 696f 6e3a 2032 2e30 2e33 350a  Version: 2.0.35.
+00000020: 5665 7273 696f 6e3a 2032 2e30 2e33 360a  Version: 2.0.36.
 00000030: 5375 6d6d 6172 793a 2077 6764 0a48 6f6d  Summary: wgd.Hom
 00000040: 652d 7061 6765 3a20 6874 7470 3a2f 2f67  e-page: http://g
 00000050: 6974 6875 622e 636f 6d2f 6865 6368 652d  ithub.com/heche-
 00000060: 7073 622f 7767 640a 4175 7468 6f72 3a20  psb/wgd.Author: 
 00000070: 4865 6e67 6368 6920 4368 656e 0a41 7574  Hengchi Chen.Aut
 00000080: 686f 722d 656d 6169 6c3a 2068 6563 6865  hor-email: heche
 00000090: 4070 7362 2e76 6962 2d75 6765 6e74 2e62  @psb.vib-ugent.b
```

### Comparing `wgd-2.0.35/README.md` & `wgd-2.0.36/README.md`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/cli.py` & `wgd-2.0.36/cli.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/setup.py` & `wgd-2.0.36/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='wgd',
-    version='2.0.35',
+    version='2.0.36',
     packages=['wgd'],
     url='http://github.com/heche-psb/wgd',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='wgd',
     long_description=long_description,
```

### Comparing `wgd-2.0.35/test/test_core.py` & `wgd-2.0.36/test/test_core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/__init__.py` & `wgd-2.0.36/wgd/__init__.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/beast.py` & `wgd-2.0.36/wgd/beast.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/cluster.py` & `wgd-2.0.36/wgd/cluster.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/codeml.py` & `wgd-2.0.36/wgd/codeml.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/core.py` & `wgd-2.0.36/wgd/core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/mcmctree.py` & `wgd-2.0.36/wgd/mcmctree.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/mix.py` & `wgd-2.0.36/wgd/mix.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/peak.py` & `wgd-2.0.36/wgd/peak.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,16 +397,16 @@
             mean,std,weight = means[num][0],np.sqrt(stds[num][0][0]),weights[num]
             if nums == 1: df_comp = df.copy()
             else: df_comp = df[df['AnchorKs_GMM_Component']==num]
             w = df_comp['weightoutlierexcluded']
             x = np.array(list(df_comp['dS']))
             y = x[np.isfinite(x)]
             w = w[np.isfinite(x)]
-            if len(y) < 2:
-                logging.info("Detected one component with less than 2 elements, will skip it")
+            if len(set(y)) < 2:
+                logging.info("Detected one component with less than 2 valid elements, will skip it")
                 continue
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, weights=w, alpha=0.5, rwidth=0.8, label = "component {}".format(num))
             CHF = get_totalH(Hs)
             scaling = CHF*0.1
             scalings.append(scaling)
             if safeylim:
                 Hs_max = max(Hs)
@@ -420,25 +420,27 @@
                 safe_max = max([max(y_lim_beforekde_s),max(Hs_maxs)])
                 ax.set_ylim(0, safe_max)
             if showCI and not hideci:
                 CI_95 = stats.lognorm.ppf([0.025, 0.975], scale=np.exp(mean), s=std)
                 CI_dict[num]=CI_95
                 CI_95_y0 = scaling*stats.lognorm.pdf(CI_95[0], scale=np.exp(mean),s=std)
                 CI_95_y1 = scaling*stats.lognorm.pdf(CI_95[1], scale=np.exp(mean),s=std)
-                plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} lower {}%CI {:.2f}'.format(num,95,CI_95[0]))
-                plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} upper {}%CI {:.2f}'.format(num,95,CI_95[1]))
+                #plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} lower {}%CI {:.2f}'.format(num,95,CI_95[0]))
+                plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='c{} {}%CI {:.2f}-{:.2f}'.format(num,95,CI_95[0],CI_95[1]))
+                plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1)
+                #plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} upper {}%CI {:.2f}'.format(num,95,CI_95[1]))
     else:
         for num,color in zip(range(nums),colors):
             mean,std,weight = means[num][0],np.sqrt(stds[num][0][0]),weights[num]
             if nums == 1: df_comp = df.drop_duplicates(subset=['family','node'])
             else: df_comp = df[df['AnchorKs_GMM_Component']==num].drop_duplicates(subset=['family','node'])
             x = np.array(list(df_comp['node_averaged_dS_outlierexcluded']))
             y = x[np.isfinite(x)]
-            if len(y) < 2:
-                logging.info("Detected one component with less than 2 elements, will skip it")
+            if len(set(y)) < 2:
+                logging.info("Detected one component with less than 2 valid elements, will skip it")
                 continue
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, alpha=0.5, rwidth=0.8, label = "component {}".format(num))
             CHF = get_totalH(Hs)
             scaling = CHF*0.1
             scalings.append(scaling)
             if safeylim:
                 Hs_max = max(Hs)
@@ -461,16 +463,18 @@
             #        plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='Peak {} lower {}%CI {:.2f}'.format(num,95,CI_95[0]))
             #        plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1,label='Peak {} upper {}%CI {:.2f}'.format(num,95,CI_95[1]))
             if showCI and not hideci:
                 CI_95 = stats.lognorm.ppf([0.025, 0.975], scale=np.exp(mean), s=std)
                 CI_dict[num]=CI_95
                 CI_95_y0 = scaling*stats.lognorm.pdf(CI_95[0], scale=np.exp(mean),s=std)
                 CI_95_y1 = scaling*stats.lognorm.pdf(CI_95[1], scale=np.exp(mean),s=std)
-                plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} lower {}%CI {:.2f}'.format(num,95,CI_95[0]))
-                plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} upper {}%CI {:.2f}'.format(num,95,CI_95[1]))
+                #plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} lower {}%CI {:.2f}'.format(num,95,CI_95[0]))
+                #plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1,label='component {} upper {}%CI {:.2f}'.format(num,95,CI_95[1]))
+                plt.plot([CI_95[0],CI_95[0]],[0,CI_95_y0], color = color, alpha = 0.8, ls = ':', lw = 1,label='c{} {}%CI {:.2f}-{:.2f}'.format(num,95,CI_95[0],CI_95[1]))
+                plt.plot([CI_95[1],CI_95[1]],[0,CI_95_y1],color = color, alpha = 0.8, ls = ':', lw = 1)
     ax.set_xlim(0, 5)
     ax.legend(loc='upper right',frameon=False)
     #if nums<2: ax.legend(loc='upper right',frameon=False)
     #else: ax.legend(loc='upper right',frameon=False,fontsize='x-small')
     #ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
     ax.set_xlabel("$K_\mathrm{S}$")
     ax.set_ylabel(ylabel)
@@ -493,15 +497,15 @@
     for i,weight in enumerate(weights):
         cum_weight = cum_weight + weight
         if cum_weight >= half_weight:
             medianx = kdex[i]
             break
     return medianx
 
-def plot_ak_component_kde(df,nums,hdr,bins=50,ylabel="Duplication events",weighted=True,regime='multiplicon',user_xlim=None,user_ylim=None,hidehdr=False,notscale=False,safeylim=False):
+def plot_ak_component_kde(df,nums,hdr,bins=50,ylabel="Duplication events",weighted=True,regime='multiplicon',user_xlim=None,user_ylim=None,hidehdr=False,notscale=False,safeylim=False, cutoff=3):
     colors = cm.viridis(np.linspace(0, 1, nums))
     kdesity = 100
     kde_x = np.linspace(0,5,num=bins*kdesity)
     fig, ax = plt.subplots()
     Hs_maxs,y_lim_beforekde_s,HDRs = [],[],{}
     scalings,kdes = [],[]
     if weighted:
@@ -509,16 +513,16 @@
             #if nums == 1: df_comp = df.drop_duplicates(subset=['family','node'])
             if nums == 1: df_comp = df.copy()
             else: df_comp = df[df['AnchorKs_GMM_Component']==num]
             w = df_comp['weightoutlierexcluded']
             x = np.array(list(df_comp['dS']))
             y = x[np.isfinite(x)]
             w = w[np.isfinite(x)]
-            if len(y) < 2:
-                logging.info("Detected one component with less than 2 elements, will skip it")
+            if len(set(y)) < 2:
+                logging.info("Detected one component with less than 2 valid elements, will skip it")
                 continue
             kde = stats.gaussian_kde(y,weights=w,bw_method='scott')
             kdes.append(kde)
             kde_y = kde(kde_x)
             mode, maxim = kde_mode(kde_x, kde_y)
             #median = getmediankdexy(kde_x,kde_y)
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, weights=w, alpha=0.5, rwidth=0.8, label = "component {} (mode {:.2f})".format(num,mode))
@@ -537,27 +541,28 @@
                 safe_max = max([max(y_lim_beforekde_s),max(Hs_maxs)])
                 ax.set_ylim(0, safe_max)
             #ax.axvline(x = mode, ymin=0,ymax=scaling*maxim/Hs_max, color = color, alpha = 0.8, ls = ':', lw = 1)
             plt.plot([mode,mode], [0,scaling*maxim], color=color,alpha = 0.8,linestyle='-.')
             #plt.plot([median,median], [0,scaling*kde(median)], color=color,alpha = 0.8,linestyle='-.')
             if not hidehdr:
                 upper_HPD,lower_HPD = calculateHPD(y,hdr)
-                plt.plot([upper_HPD,upper_HPD], [0,scaling*kde(upper_HPD)], color=color,alpha = 0.8,linestyle=':')
+                if upper_HPD>cutoff: upper_HPD=cutoff
+                plt.plot([upper_HPD,upper_HPD], [0,scaling*kde(upper_HPD)], color=color,alpha = 0.8,linestyle=':',label='{}% HDR of c{} {:.2f}-{:.2f}'.format(hdr,num,lower_HPD,upper_HPD))
                 plt.plot([lower_HPD,lower_HPD], [0,scaling*kde(lower_HPD)], color=color,alpha = 0.8,linestyle=':')
             #ax.axvline(x = upper_HPD, ymin=0, ymax=upper_HPD_y, color = color, alpha = 0.8, ls = '-.', lw = 1,label='HDR {:.2f}-{:.2f}'.format(lower_HPD,upper_HPD))
             #ax.axvline(x = lower_HPD, ymin=0, ymax=lower_HPD_y, color = color, alpha = 0.8, ls = '-.', lw = 1)
                 HDRs[num] = (lower_HPD,upper_HPD)
     else:
         for num,color in zip(range(nums),colors):
             if nums == 1: df_comp = df.drop_duplicates(subset=['family','node'])
             else: df_comp = df[df['AnchorKs_GMM_Component']==num].drop_duplicates(subset=['family','node'])
             x = np.array(list(df_comp['node_averaged_dS_outlierexcluded']))
             y = x[np.isfinite(x)]
-            if len(y) < 2:
-                logging.info("Detected one component with less than 2 elements, will skip it")
+            if len(set(y)) < 2:
+                logging.info("Detected one component with less than 2 valid elements, will skip it")
                 continue
             kde = stats.gaussian_kde(y,bw_method='scott')
             kdes.append(kde)
             kde_y = kde(kde_x)
             mode, maxim = kde_mode(kde_x, kde_y)
             #median = getmediankdexy(kde_x,kde_y)
             Hs, Bins, patches = ax.hist(y, bins = np.linspace(0, 50, num=bins+1,dtype=int)/10, color = color, alpha=0.5, rwidth=0.8, label = "component {} (mode {:.2f})".format(num,mode))
@@ -579,15 +584,16 @@
             plt.plot([mode,mode], [0,scaling*maxim], color=color,alpha = 0.8,linestyle='-.')
             #plt.plot([median,median], [0,scaling*kde(median)], color=color,alpha = 0.8,linestyle='-.')
             #ax.axvline(x = mode, ymin=0, ymax=scaling*maxim/Hs_max, color = color, alpha = 0.8, ls = ':', lw = 1)
             if not hidehdr:
                 upper_HPD,lower_HPD = calculateHPD(y,hdr)
                 #upper_HPD_y = scaling*kde(upper_HPD)/Hs_max
                 #lower_HPD_y = scaling*kde(lower_HPD)/Hs_max
-                plt.plot([upper_HPD,upper_HPD], [0,scaling*kde(upper_HPD)], color=color,alpha = 0.8,linestyle=':')
+                if upper_HPD>cutoff: upper_HPD=cutoff
+                plt.plot([upper_HPD,upper_HPD], [0,scaling*kde(upper_HPD)], color=color,alpha = 0.8,linestyle=':',label='{}% HDR of c{} {:.2f}-{:.2f}'.format(hdr,num,lower_HPD,upper_HPD))
                 plt.plot([lower_HPD,lower_HPD], [0,scaling*kde(lower_HPD)], color=color,alpha = 0.8,linestyle=':')
             #ax.axvline(x = upper_HPD, ymin=0, ymax=upper_HPD_y, color = color, alpha = 0.8, ls = '-.', lw = 1,label='HDR {:.2f}-{:.2f}'.format(lower_HPD,upper_HPD))
             #ax.axvline(x = lower_HPD, ymin=0, ymax=lower_HPD_y, color = color, alpha = 0.8, ls = '-.', lw = 1)
                 HDRs[num] = (lower_HPD,upper_HPD)
     #ax.legend(loc='upper right', fontsize='small',frameon=False)
     ax.legend(loc='upper right', frameon=False)
     #ax.legend(loc='center left',bbox_to_anchor=(1.0, 0.5),frameon=False)
@@ -1280,14 +1286,18 @@
         fig, ax = plt.subplots(figsize=(10, 10))
         ax.set_xlim(-5,2)
         ax.set_title('KDE and spline of log-transformed anchor $K_\mathrm{S}$ of species '+ '{}'.format(sp))
         ax.set_xlabel("ln $K_\mathrm{S}$")
         ax.set_ylabel("Density of retained duplicates")
     max_ks,min_ks = ks.max(),ks.min()
     ks_refed,cutoff,w_refed = reflect_logks(ks,w)
+    if len(set(ks_refed)) < 2:
+        logging.warning("Less than 2 valid elements, will skip it")
+        lower95CI,upper95CI = None,None
+        return lower95CI,upper95CI 
     kde = stats.gaussian_kde(ks_refed, bw_method="scott", weights=w_refed)
     bw_modifier = 0.4
     kde.set_bandwidth(kde.factor * bw_modifier)
     kde_x = np.linspace(min_ks-cutoff, max_ks+cutoff,num=500)
     kde_y = kde(kde_x)
     if withfig: ax.plot(kde_x, kde_y, color="k", lw=1, label="KDE")
     spl = interpolate.UnivariateSpline(kde_x, kde_y)
@@ -1785,22 +1795,22 @@
         plt.close()
         fig = plot_ak_component(df_c.dropna(),n,bins=50,plot = plot,ylabel="Duplication events",weighted=weighted,regime=guide,user_xlim=user_xlim,user_ylim=user_ylim)
         outdir2 = _mkdir(os.path.join(outdir,"HDR_CI"))
         if weighted: fname = os.path.join(outdir2, "{}_guided_AnchorKs_GMM_Component{}_node_weighted.pdf".format(guide,n))
         else: fname = os.path.join(outdir2, "{}_guided_AnchorKs_GMM_Component{}_node_averaged.pdf".format(guide,n))
         fig.savefig(fname)
         plt.close()
-        fig,HDRs = plot_ak_component_kde(df_c.dropna(),n,hdr,bins=50,ylabel="Duplication events",weighted=weighted,regime=guide,user_xlim=user_xlim,user_ylim=user_ylim)
+        fig,HDRs = plot_ak_component_kde(df_c.dropna(),n,hdr,bins=50,ylabel="Duplication events",weighted=weighted,regime=guide,user_xlim=user_xlim,user_ylim=user_ylim,cutoff=cutoff,safeylim=True)
         getGuided_AP_HDR(HDRs,hdr,n,df_c,outdir2,guide,cutoff)
         if weighted: fname = os.path.join(outdir2, "{}_guided_AnchorKs_GMM_Component{}_node_weighted_kde.pdf".format(guide,n))
         else: fname = os.path.join(outdir2, "{}_guided_AnchorKs_GMM_Component{}_node_averaged_kde.pdf".format(guide,n))
         fig.savefig(fname)
         plt.close()
-        fig2,ax2,kdes,scalings = plot_ak_component_kde(df_c.dropna(),n,hdr,bins=50,ylabel="Duplication events",weighted=weighted,regime=guide,user_xlim=user_xlim,user_ylim=user_ylim,hidehdr=True,notscale=True)
-        get_peak_SegGuidedGMM(guide,kdes,scalings,fig2,ax2,df_c,n,outdir,peak_threshold,weighted,rel_height,keeptmp=keeptmp)
+        fig2,ax2,kdes,scalings = plot_ak_component_kde(df_c.dropna(),n,hdr,bins=50,ylabel="Duplication events",weighted=weighted,regime=guide,user_xlim=user_xlim,user_ylim=user_ylim,hidehdr=True,notscale=True,safeylim=True)
+        get_peak_SegGuidedGMM(guide,kdes,scalings,fig2,ax2,df_c,n,outdir,peak_threshold,weighted,rel_height,keeptmp=keeptmp,cutoff=cutoff)
     plot_Elbow_loss(Losses,outdir,n1=components[0],n2=components[1],method='GMM',regime=guide)
     return df
 
 def getGuided_AP_HDR(HDRs,hdr,n,df_c,outdir,regime,cutoff):
     for num in HDRs.keys():
         df_tmp = df_c[df_c['AnchorKs_GMM_Component']==num]
         df_tmp = df_tmp.loc[(df_tmp['dS']<=min([cutoff,HDRs[num][1]])) & (df_tmp['dS']>=HDRs[num][0]),:]
@@ -1835,43 +1845,44 @@
         Losses.append(Elbow_lossf(X_log,[i[0] for i in means],labels))
         df_c = add_apgmmlabels_pairs(df,df_withindex,labels,outdir,n)
         fig = plot_ak_component(df_c,n,bins=50,plot = plot,ylabel="Duplication events",weighted=weighted,regime='original',user_xlim=user_xlim,user_ylim=user_ylim)
         if weighted: fname = os.path.join(outdir, "Original_AnchorKs_GMM_Component{}_node_weighted.pdf".format(n))
         else: fname = os.path.join(outdir, "Original_AnchorKs_GMM_Component{}_node_averaged.pdf".format(n))
         fig.savefig(fname)
         plt.close()
-        fig, CI, ax, _ = plot_ak_component_lognormal(df_c.dropna(),means,stds,weights,n,bins=50,ylabel="Duplication events",weighted=weighted,regime='original',showCI=showCI,peak_threshold=peak_threshold,rel_height=rel_height,user_xlim=user_xlim,user_ylim=user_ylim,hideci=True)
+        fig, CI, ax, _ = plot_ak_component_lognormal(df_c.dropna(),means,stds,weights,n,bins=50,ylabel="Duplication events",weighted=weighted,regime='original',showCI=showCI,peak_threshold=peak_threshold,rel_height=rel_height,user_xlim=user_xlim,user_ylim=user_ylim,hideci=True,safeylim=True)
         if weighted: fname = os.path.join(outdir, "Original_AnchorKs_GMM_Component{}_node_weighted_Lognormal.pdf".format(n))
         else: fname = os.path.join(outdir, "Original_AnchorKs_GMM_Component{}_node_averaged_Lognormal.pdf".format(n))
         fig.savefig(fname)
         plt.close()
-        fig2, CI, ax2, _ = plot_ak_component_lognormal(df_c.dropna(),means,stds,weights,n,bins=50,ylabel="Duplication events",weighted=weighted,regime='original',showCI=showCI,peak_threshold=peak_threshold,rel_height=rel_height,user_xlim=user_xlim,user_ylim=user_ylim)
+        fig2, CI, ax2, _ = plot_ak_component_lognormal(df_c.dropna(),means,stds,weights,n,bins=50,ylabel="Duplication events",weighted=weighted,regime='original',showCI=showCI,peak_threshold=peak_threshold,rel_height=rel_height,user_xlim=user_xlim,user_ylim=user_ylim,safeylim=True)
         if weighted: fname = os.path.join(_mkdir(os.path.join(outdir,"LogGMM_CI")), "GMM_Component{}_node_weighted_Lognormal.pdf".format(n))
         else: fname = os.path.join(outdir,"LogGMM_CI", "GMM_Component{}_node_averaged_Lognormal.pdf".format(n))
         if showCI: df_c_CI = add_apCI(df_c,outdir,CI,n,cutoff,weighted)
         fig2.savefig(fname)
         plt.close()
-        fig3, CI, ax3, scalings = plot_ak_component_lognormal(df_c.dropna(),means,stds,weights,n,bins=50,ylabel="Duplication events",weighted=weighted,regime='original',showCI=showCI,peak_threshold=peak_threshold,rel_height=rel_height,user_xlim=user_xlim,user_ylim=user_ylim,hideci=True)
-        get_peak_AnchGMM(means,stds,scalings,fig3,ax3,df_c,n,outdir,peak_threshold,weighted,rel_height,keeptmp=keeptmp)
+        fig3, CI, ax3, scalings = plot_ak_component_lognormal(df_c.dropna(),means,stds,weights,n,bins=50,ylabel="Duplication events",weighted=weighted,regime='original',showCI=showCI,peak_threshold=peak_threshold,rel_height=rel_height,user_xlim=user_xlim,user_ylim=user_ylim,hideci=True,safeylim=True)
+        get_peak_AnchGMM(means,stds,scalings,fig3,ax3,df_c,n,outdir,peak_threshold,weighted,rel_height,keeptmp=keeptmp,cutoff=cutoff)
         plt.close()
     plot_Elbow_loss(Losses,outdir,n1=components[0],n2=components[1],method='GMM',regime='original')
     return df
 
-def get_peak_SegGuidedGMM(regime,kdes,scalings,fig,ax,df_c,n,outdir,peak_threshold,weighted,rel_height,keeptmp=False):
+def get_peak_SegGuidedGMM(regime,kdes,scalings,fig,ax,df_c,n,outdir,peak_threshold,weighted,rel_height,keeptmp=False,cutoff=3):
     outdir = _mkdir(os.path.join(outdir,"HighMass_CI"))
     na=False if weighted else True
     #Components = list(set(df_c['AnchorKs_GMM_Component']))
     colors = cm.viridis(np.linspace(0, 1, n))
     for cp,color,scaling,kde in zip(range(n),colors,scalings,kdes):
         df = df_c[df_c['AnchorKs_GMM_Component']==cp]
         lower_CI, upper_CI = find_apeak(df,None,None,outdir,peak_threshold=peak_threshold,na=na,rel_height=rel_height,withfig=False,loglabel="{}-Components Model Peak {}".format(n,cp),keeptmp=keeptmp)
         if lower_CI is None:
             logging.warning("No qualified peak detected")
             continue
         if upper_CI> 5: upper_CI=5
+        if upper_CI > cutoff: upper_CI=cutoff
         #ax.axvline(lower_CI, color = color, alpha = 0.8, ls = '--', lw = 0.8,label='Peak of c{} {}%CI {:.2f}-{:.2f}'.format(cp,95,lower_CI,upper_CI))
         #ax.axvline(upper_CI, color = color, alpha = 0.8, ls = '--', lw = 0.8)
         lower_CI_y0 = scaling*kde(lower_CI)
         upper_CI_y1 = scaling*kde(upper_CI)
         ax.plot([lower_CI,lower_CI],[0,lower_CI_y0], color = color, alpha = 0.8, ls = '--', lw = 1,label='HighMass of c{} {}%CI {:.2f}-{:.2f}'.format(cp,95,lower_CI,upper_CI))
         ax.plot([upper_CI,upper_CI],[0,upper_CI_y1], color = color, alpha = 0.8, ls = '--', lw = 1)
         if weighted: df = df[(df['dS']>=lower_CI)&(df['dS']<=upper_CI)]
@@ -1880,27 +1891,28 @@
         df = df.rename(columns={'gene1':'gene_x','gene2':'gene_y','AnchorKs_GMM_Component':'SegmentKs_GMM_Component'})
         df.to_csv(fname,header=True,index=True,sep='\t')
     fname = os.path.join(outdir,'{}_guided_{}components_HighMass_95%CI.pdf'.format(regime,n))
     ax.legend(loc='upper right',frameon=False)
     fig.tight_layout()
     fig.savefig(fname)
 
-def get_peak_AnchGMM(means,stds,scalings,fig,ax,df_c,n,outdir,peak_threshold,weighted,rel_height,keeptmp=False):
+def get_peak_AnchGMM(means,stds,scalings,fig,ax,df_c,n,outdir,peak_threshold,weighted,rel_height,keeptmp=False,cutoff=3):
     outdir = _mkdir(os.path.join(outdir,"HighMass_CI"))
     na=False if weighted else True
     #Components = sorted(list(set(df_c['AnchorKs_GMM_Component'])))
     colors = cm.viridis(np.linspace(0, 1, n))
     for cp,color,scaling in zip(range(n),colors,scalings):
         mean,std = means[cp][0],np.sqrt(stds[cp][0][0])
         df = df_c[df_c['AnchorKs_GMM_Component']==cp]
         lower_CI, upper_CI = find_apeak(df,None,None,outdir,peak_threshold=peak_threshold,na=na,rel_height=rel_height,withfig=False,loglabel="{}-Components Model Peak {}".format(n,cp),keeptmp=keeptmp)
         if lower_CI is None:
             logging.warning("No qualified peak detected")
             continue
         if upper_CI > 5: upper_CI=5
+        if upper_CI>cutoff: upper_CI=cutoff
         #ax.axvline(lower_CI, color = color, alpha = 0.8, ls = '--', lw = 0.8,label='Peak of c{} {}%CI {:.2f}-{:.2f}'.format(cp,95,lower_CI,upper_CI))
         #ax.axvline(upper_CI, color = color, alpha = 0.8, ls = '--', lw = 0.8)
         lower_CI_y0 = scaling*stats.lognorm.pdf(lower_CI, scale=np.exp(mean),s=std)
         upper_CI_y1 = scaling*stats.lognorm.pdf(upper_CI, scale=np.exp(mean),s=std)
         ax.plot([lower_CI,lower_CI],[0,lower_CI_y0], color = color, alpha = 0.8, ls = '--', lw = 1,label='HighMass of c{} {}%CI {:.2f}-{:.2f}'.format(cp,95,lower_CI,upper_CI))
         ax.plot([upper_CI,upper_CI],[0,upper_CI_y1], color = color, alpha = 0.8, ls = '--', lw = 1)
         if weighted: df = df[(df['dS']>=lower_CI)&(df['dS']<=upper_CI)]
```

### Comparing `wgd-2.0.35/wgd/postplot.py` & `wgd-2.0.36/wgd/postplot.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/ratecorrect.py` & `wgd-2.0.36/wgd/ratecorrect.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/syn.py` & `wgd-2.0.36/wgd/syn.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/tree.py` & `wgd-2.0.36/wgd/tree.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/utils.py` & `wgd-2.0.36/wgd/utils.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd/viz.py` & `wgd-2.0.36/wgd/viz.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.35/wgd.egg-info/PKG-INFO` & `wgd-2.0.36/wgd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7767 640a  : 2.1.Name: wgd.
-00000020: 5665 7273 696f 6e3a 2032 2e30 2e33 350a  Version: 2.0.35.
+00000020: 5665 7273 696f 6e3a 2032 2e30 2e33 360a  Version: 2.0.36.
 00000030: 5375 6d6d 6172 793a 2077 6764 0a48 6f6d  Summary: wgd.Hom
 00000040: 652d 7061 6765 3a20 6874 7470 3a2f 2f67  e-page: http://g
 00000050: 6974 6875 622e 636f 6d2f 6865 6368 652d  ithub.com/heche-
 00000060: 7073 622f 7767 640a 4175 7468 6f72 3a20  psb/wgd.Author: 
 00000070: 4865 6e67 6368 6920 4368 656e 0a41 7574  Hengchi Chen.Aut
 00000080: 686f 722d 656d 6169 6c3a 2068 6563 6865  hor-email: heche
 00000090: 4070 7362 2e76 6962 2d75 6765 6e74 2e62  @psb.vib-ugent.b
```

### Comparing `wgd-2.0.35/wgd.egg-info/requires.txt` & `wgd-2.0.36/wgd.egg-info/requires.txt`

 * *Files identical despite different names*

