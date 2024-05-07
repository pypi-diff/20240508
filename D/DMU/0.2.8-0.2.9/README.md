# Comparing `tmp/DMU-0.2.8.tar.gz` & `tmp/dmu-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DMU-0.2.8.tar", last modified: Fri Mar 15 14:56:21 2024, max compression
+gzip compressed data, was "dmu-0.2.9.tar", last modified: Tue May  7 23:11:31 2024, max compression
```

## Comparing `DMU-0.2.8.tar` & `dmu-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 14:56:21.953249 DMU-0.2.8/
-drwxrwxrwx   0        0        0        0 2024-03-15 14:56:21.953249 DMU-0.2.8/DMU/
--rw-rw-rw-   0        0        0        0 2024-03-15 14:56:01.000000 DMU-0.2.8/DMU/__init__.py
--rw-rw-rw-   0        0        0     1093 2024-03-15 14:56:01.000000 DMU-0.2.8/DMU/custom_logger.py
--rw-rw-rw-   0        0        0     3577 2024-03-15 14:56:01.000000 DMU-0.2.8/DMU/graph_styles.py
--rw-rw-rw-   0        0        0    12834 2024-03-15 14:56:01.000000 DMU-0.2.8/DMU/plot_utils.py
--rw-rw-rw-   0        0        0   133546 2024-03-15 14:56:01.000000 DMU-0.2.8/DMU/utils.py
--rw-rw-rw-   0        0        0    10167 2024-03-15 14:56:01.000000 DMU-0.2.8/DMU/utils_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-15 14:56:21.953249 DMU-0.2.8/DMU.egg-info/
--rw-rw-rw-   0        0        0    11314 2024-03-15 14:56:21.000000 DMU-0.2.8/DMU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2024-03-15 14:56:21.000000 DMU-0.2.8/DMU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 14:56:21.000000 DMU-0.2.8/DMU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-03-15 14:56:21.000000 DMU-0.2.8/DMU.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-15 14:56:21.000000 DMU-0.2.8/DMU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1102 2024-03-15 14:56:01.000000 DMU-0.2.8/LICENSE
--rw-rw-rw-   0        0        0    11314 2024-03-15 14:56:21.953249 DMU-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    10503 2024-03-15 14:56:01.000000 DMU-0.2.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-15 14:56:21.953249 DMU-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     3748 2024-03-15 14:56:01.000000 DMU-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 23:11:31.801452 dmu-0.2.9/
+drwxrwxrwx   0        0        0        0 2024-05-07 23:11:31.785677 dmu-0.2.9/DMU/
+-rw-rw-rw-   0        0        0        0 2024-05-07 23:10:38.000000 dmu-0.2.9/DMU/__init__.py
+-rw-rw-rw-   0        0        0     1093 2024-05-07 23:10:38.000000 dmu-0.2.9/DMU/custom_logger.py
+-rw-rw-rw-   0        0        0     7017 2024-05-07 23:10:38.000000 dmu-0.2.9/DMU/graph_styles.py
+-rw-rw-rw-   0        0        0    13809 2024-05-07 23:10:38.000000 dmu-0.2.9/DMU/plot_utils.py
+-rw-rw-rw-   0        0        0   134401 2024-05-07 23:10:38.000000 dmu-0.2.9/DMU/utils.py
+-rw-rw-rw-   0        0        0    10167 2024-05-07 23:10:38.000000 dmu-0.2.9/DMU/utils_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 23:11:31.785677 dmu-0.2.9/DMU.egg-info/
+-rw-rw-rw-   0        0        0    11314 2024-05-07 23:11:31.000000 dmu-0.2.9/DMU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2024-05-07 23:11:31.000000 dmu-0.2.9/DMU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 23:11:31.000000 dmu-0.2.9/DMU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-07 23:11:31.000000 dmu-0.2.9/DMU.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-07 23:11:31.000000 dmu-0.2.9/DMU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1102 2024-05-07 23:10:38.000000 dmu-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0    11314 2024-05-07 23:11:31.785677 dmu-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10503 2024-05-07 23:10:38.000000 dmu-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 23:11:31.801452 dmu-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     3748 2024-05-07 23:10:38.000000 dmu-0.2.9/setup.py
```

### Comparing `DMU-0.2.8/DMU/custom_logger.py` & `dmu-0.2.9/DMU/custom_logger.py`

 * *Files identical despite different names*

### Comparing `DMU-0.2.8/DMU/plot_utils.py` & `dmu-0.2.9/DMU/plot_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,67 +97,71 @@
         leg_handles.append(lh)
     
     def flatten(xss):
         return [x for xs in xss for x in xs]
     return(flatten(leg_handles),flatten(leg_labels))
 
 # Automatically adjust tick locations to intervals that do not require two decimal places
-def adjust_ticks(ticks,axrange=None,numticks=12):
-    nums      = []
-    ooms      = []
+#%%
+def adjust_ticks(ax,which="both",Nx=4,Ny=4,xpad=1,ypad=1,respect_zero =True):
+    """
+    Input: 
+        ax: axis that we want to adjust ticks for, this should be done AFTER the axlims have been set.
+        which: which ticks to adjust any of - ["both","xticks","yticks"]
+        Nx: number of xticks, default = 7 (can be included even if which="yticks") 
+        Ny: number of yticks, default = 7 (can be included even if which="xticks")
+        xpad: symmetric overlap of extra xticks (so, if your range is [-0.5,0,0.5] then it will add [-1,0.5,0,0.5,1])
+        ypad: symmetric overlap of extra yticks (so, if your range is [-0.5,0,0.5] then it will add [-1,0.5,0,0.5,1])        
+        respect_zero: Forces the zero tick to be included
+    Output: Adjusted axticks such that the number of ticks is as close to your chosen Nx and Ny as possible, without using than 2 sig fig e.g. 0.25 
+    """
     
-    #First, we find out the highest oom that we will base all our nums on
-    if axrange == None:
-        axrange = [float(ticks[-1]),float( ticks[0])]
+    def limcalc(lim,N,pad,respect_zero=True):
+        proxvals = np.array([0.01,0.02,0.05,0.1,0.2,0.5,1.0,2.0,5.0,10,20,50,100])
+        rawspace = np.linspace(lim[0],lim[1],N)
+        rawdiff  = np.diff(rawspace)[0]
+        oom      = np.floor(np.log10(abs(rawdiff)))
+        oomdiff  = rawdiff/10**oom    
+        oomlim = lim/10**oom
+        padlim = [oomlim[0]-pad*oomdiff,oomlim[1]+pad*oomdiff]
+        prox = np.abs(proxvals - oomdiff)
+        tickdiff = proxvals[np.where(prox == np.min(prox))[0]][0]
         
-    for tick in ticks:
-        if tick != 0:
-            ooms.append(np.floor(np.log10(abs(tick))))
-    oom = np.max(ooms)
-    
-    nums = np.array(ticks)/(10**oom)
-    diffs = np.diff(nums)
-    
-    axrange = axrange/(10**oom)
-    diffnum = (axrange[1]-axrange[0])/numticks
-    
-    def diffnum_converter(diff,nums,numticks):
-        proxval = [0.01,0.02,0.05,0.1,0.2,0.5,1.0,2.0,5.0,10,20,50,100]
+        if respect_zero == False:
+            ticks = np.arange(round(padlim[0]/tickdiff)*tickdiff,round(padlim[1]/tickdiff)*tickdiff,tickdiff)
+            
+        elif respect_zero == True:
+            ticks = np.concatenate([np.flip(np.arange(0,padlim[0],-tickdiff)) ,  np.arange(0,padlim[1],tickdiff)])
         
-        diffnum = min(proxval, key=lambda x: abs(x - diff))  
-        new_low =  nums[0] - (nums[0] % diffnum)
-        new_high = (nums[-1] + diffnum) - (nums[-1] % diffnum)
+        return(ticks*10**oom,[f"{val:.1e}" for val in ticks],oom)
         
-        if len(np.arange(new_low,new_high,diffnum)) >=numticks+2:
-            try:
-                diffnum = proxval[proxval.index(diffnum) + 1]
-            except:
-                diffnum = 2*diffnum
-            
-            new_low =  nums[0] - (nums[0] % diffnum)
-            new_high = (nums[-1] + diffnum) - (nums[-1] % diffnum)
-            
-            if len(np.arange(new_low,new_high,diffnum)) >=numticks:
-                try:
-                    diffnum = proxval[proxval.index(diffnum) + 1]
-                except:
-                    diffnum = diffnum*2
-                
-            new_low =  nums[0] - (nums[0] % diffnum)
-            new_high = (nums[-1] + diffnum) - (nums[-1] % diffnum)
-            
-        new_nums = np.round(np.arange(new_low-5*diffnum,new_high+5*diffnum,diffnum),2)
-        return(new_nums)
-
-    new_nums = diffnum_converter(diffnum,nums,numticks)
     
-    for num in new_nums:
-        new_ticks = new_nums * np.power(10,oom)
-        
-    return(new_ticks)
+    xfmt = ScalarFormatterForceFormat(); xfmt.set_powerlimits((-2,2))
+    yfmt = ScalarFormatterForceFormat(); yfmt.set_powerlimits((-2,2))
+    
+    
+    if which == "both" or which == "xticks":
+        xlim = ax.get_xlim()
+        xticks,xticklabels,xoom = limcalc(xlim,Nx,xpad,respect_zero)
+        ax.set_xticks(xticks)
+        ax.set_xticklabels(xticklabels)
+        if xoom >1:
+            xfmt.set_format("%2d")
+        ax.xaxis.set_major_formatter(xfmt)
+        ax.set_xlim(xlim)
+        
+    if which == "both" or which == "yticks":
+        ylim = ax.get_ylim()
+        yticks,yticklabels,yoom = limcalc(ylim,Ny,ypad,respect_zero)
+        ax.set_yticks(yticks)
+        ax.set_yticklabels(yticklabels)
+        if yoom >1:
+            yfmt.set_format("%2d")
+        ax.yaxis.set_major_formatter(yfmt)
+        ax.set_ylim(ylim)
 
 
 def align_axis_zeros(axes):
 
     ylims_current = {}   #  Current ylims
     ylims_mod     = {}   #  Modified ylims
     deltas        = {}   #  ymax - ymin for ylims_current
@@ -173,24 +177,29 @@
         ylims_mod[ax]     = [np.nan,np.nan]   # Construct a blank list
         ylims_mod[ax][1]  = max(deltas[ax] * (1-np.array(list(ratios.values()))))
                         # Choose the max value among (delta for ax)*(1-ratios),
                         # and apply it to ymax for ax
         ylims_mod[ax][0]  = min(-deltas[ax] * np.array(list(ratios.values())))
                         # Do the same for ymin
         ax.set_ylim(tuple(ylims_mod[ax]))        
-        
+
 class ScalarFormatterForceFormat(mpl.ticker.ScalarFormatter):
-    def __init__(self, useOffset=True, useMathText=False):
+    def __init__(self, useOffset=True, useMathText=True):
         super().__init__(useOffset=useOffset, useMathText=useMathText)
-        self._set_format()
+        self.set_format()
 
-    def _set_format(self):
-        self.format = "%1.1f"  # Give format here
+    def set_format(self,form="%1.1f"):
+        self.format = form  # Give format here
         
 #%%
+def ClearAxis(fig):
+    for ax in fig.axes:
+        ax.grid(which='major', visible = False)
+        ax.grid(which='minor', visible = False)
+        
 def DefaultGrid(ax):
     ax.grid(which='major', color='darkgrey', linestyle='--')
     ax.grid(which='minor', color='#CCCCCC', linestyle=':')  
 
 
 #%%
 class cmap_seq(object):
@@ -353,7 +362,8 @@
     slices = [[inds[i],inds[i+1]+1] for i in range(len(inds)-1)]
     
     slices[-1][1] = len(L)
     for slc in slices:
         swdat.append(L[slc[0]:slc[1]])
     return(swdat)
 
+
```

### Comparing `DMU-0.2.8/DMU/utils.py` & `dmu-0.2.9/DMU/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from scipy import integrate, interpolate, constants
 import json
 from collections import Counter
 import natsort
 import csv
 import xlrd
 
-
 #%% Importing and executing logging
 import logging
 from . custom_logger import get_custom_logger
 logger = get_custom_logger("DMU_UTILS")
 
 #%% Importing plot tools 
 from . plot_utils import *
@@ -63,14 +62,16 @@
         P_tot.append(np.sum(BivarSpline))
     
     return(P_tot)
   
 #%%
 
 def bias_plotter(data,FIG,**kwargs): 
+    rcLinewidth = plt.rcParams['lines.linewidth']
+    
     FIG.hold_on = False
     IFIG = False
     IDF = None
     keys = list(data.keys())
     kwargdict = {'fwd':'fwd','f':'fwd','forward':'fwd',
                  'bwd':'rev','rev':'rev','reverse':'rev',
                  'title':'title','tit':'title',
@@ -133,22 +134,23 @@
             ax.set_ylabel(ykey[fwdbwd[0]])
             ax.legend()
             ax.set_title(kw.title)
         
         if kw.ideality == True:
         
             tab20 = mpl.colormaps["tab20c"]
+
             IDF = Ideality_Factor(data[ykey[0]],data[xkey[0]])
             
             if kw.plot == True:
                 IFIG = True
                 IFIG = ezplot()
-    
-                IFIG.ax[0].semilogy(IDF['V_new'],IDF['I_new'],'.-',linewidth=2,color=tab20(1),label='ideality='+"{0:.5g}".format(IDF['n']))
-                IFIG.ax[0].semilogy(IDF['V'],IDF['I'],'.',linewidth=2,c=tab20(5),label='IV data')
+                
+                IFIG.ax[0].semilogy(IDF['V_new'],IDF['I_new'],'.-',linewidth=rcLinewidth,color=tab20(1),label='ideality='+"{0:.5g}".format(IDF['n']))
+                IFIG.ax[0].semilogy(IDF['V'],IDF['I'],'.',linewidth=rcLinewidth*0.75,c=tab20(5),label='IV data')
     
     
                 IFIG.ax[0].legend()
             
                 
     elif kw.tool == "Keithley":
         keys = data['col headers']
@@ -204,17 +206,17 @@
                         tab20 = mpl.colormaps["tab20c"]
                         
                         IDF = Ideality_Factor(data[ykey[0]][0],data[xkey[0]][0],T=273,plot_range =None,fit_range = None,N=100,p0=None)
                         if kw.plot == True:
                             IFIG = ezplot()
                             Vneg = IDF['V'][np.where(IDF['I']<0)]
                             Ineg = np.abs(IDF['I'][np.where(IDF['I']<0)])
-                            IFIG.ax[0].semilogy(IDF['V_new'],IDF['I_new'],'--',linewidth=2,color=tab20(5),label='ideality='+"{0:.5g}".format(IDF['n']),zorder=5)
-                            IFIG.ax[0].semilogy(IDF['V'],IDF['I'],'.',linewidth=2,c=tab20(1),label='IV data')
-                            IFIG.ax[0].semilogy(Vneg,Ineg,'.',linewidth=2,c=tab20(9),label='abs(IV data)')
+                            IFIG.ax[0].semilogy(IDF['V_new'],IDF['I_new'],'--',linewidth=rcLinewidth,color=tab20(5),label='ideality='+"{0:.5g}".format(IDF['n']),zorder=5)
+                            IFIG.ax[0].semilogy(IDF['V'],IDF['I'],'.',linewidth=rcLinewidth,c=tab20(1),label='IV data')
+                            IFIG.ax[0].semilogy(Vneg,Ineg,'.',linewidth=rcLinewidth,c=tab20(9),label='abs(IV data)')
                             IFIG.ax[0].set_xlabel("Voltage [V]")
                             IFIG.ax[0].set_ylabel("Current [A]")
                             IFIG.ax[0].legend()
                         
                     except:
                         None
                     
@@ -271,23 +273,23 @@
                         ax_top_r = ax_top.twinx()
                         ax_bottom_r = ax_bottom.twinx()
                         
                         axyy  = [ax_top,ax_bottom]
                         axxy  = [ax_top_r,ax_bottom_r]
                     
                         
-                        ax_top.plot(data["Time"],Det_I,label='$I_{Detector}$ [I]',color=cols["ID"][1],**plotkwargs)
+                        ax_top.plot(data["Time"],Det_I,label='$I_{Detector}$ [A]',color=cols["ID"][1],**plotkwargs)
                         ax_top_r.plot(data["Time"],Em_V,label='$V_{Emitter}$ [V]',color=cols["VE"][1]**plotkwargs)
-                        ax_top.set_ylabel('$I_{Detector}$ [I]',color=cols["ID"][0])
+                        ax_top.set_ylabel('$I_{Detector}$ [A]',color=cols["ID"][0])
                         ax_top_r.set_ylabel('$V_{Emitter}$ [V]',color=cols["VE"][0])
                         
-                        ax_bottom.plot(data["Time"],Em_I,label='$I_{Emitter}$ [I]',color=cols["IE"][1],**plotkwargs)
+                        ax_bottom.plot(data["Time"],Em_I,label='$I_{Emitter}$ [A]',color=cols["IE"][1],**plotkwargs)
                         ax_bottom_r.plot(data["Time"],Em_V,label='$V_{Emitter}$ [V]',color=cols["VE"][1],**plotkwargs)
                         
-                        ax_bottom.set_ylabel('$I_{Emitter}$ [I]',   color  = cols["IE"][0])
+                        ax_bottom.set_ylabel('$I_{Emitter}$ [A]',   color  = cols["IE"][0])
                         ax_bottom_r.set_ylabel('$V_{Emitter}$ V [V]',color = cols["VE"][0])
                         
                         
                             #Fix colours
                         if len(Pkwargs['c'])<4:
                             Pkwargs['c'] = mpl.colormaps["tab20"]
                         for axis in axyy:
@@ -308,79 +310,86 @@
 
                         FIG.fig,FIG.ax[0] = plt.subplots()
                         
                         FIG.ax[1] = FIG.ax[0].twinx()
                         FIG.ax[2] = FIG.ax[0].twinx()
                         
                         #TIME = data[]
-                        p1, = FIG.ax[0].plot(data["Time"],Det_I,label='$I_{Detector}$ [I]',color=cols["ID"][1],**plotkwargs)
-                        p2, = FIG.ax[1].plot(data["Time"],Em_I,label='$I_{Emitter}$ [I]',color=cols["IE"][1],**plotkwargs)
-                        p3, = FIG.ax[2].plot(data["Time"],Em_V,'-.',label='$V_{Emitter}$ [V]',color=cols["VE"][1],linewidth = 1)
+                        p1, = FIG.ax[0].plot(data["Time"],Det_I,label='$I_{Detector}$ [A]',color=cols["ID"][1],**plotkwargs,linewidth=rcLinewidth)
+                        p2, = FIG.ax[1].plot(data["Time"],Em_I,label='$I_{Emitter}$ [A]',color=cols["IE"][1],**plotkwargs,linewidth=rcLinewidth)
+                        p3, = FIG.ax[2].plot(data["Time"],Em_V,'-.',label='$V_{Emitter}$ [V]',color=cols["VE"][1],linewidth = rcLinewidth*0.5)
                         
                         FIG.ax[0].set_xlabel("Time [s]")
-                        FIG.ax[0].set_ylabel("$I_{Detector}$ [I]" ,color=cols["ID"][0])
-                        FIG.ax[1].set_ylabel('$I_{Emitter}$ [I]'  , color=cols["IE"][0])
+                        FIG.ax[0].set_ylabel("$I_{Detector}$ [A]" ,color=cols["ID"][0])
+                        FIG.ax[1].set_ylabel('$I_{Emitter}$ [A]'  , color=cols["IE"][0])
                         FIG.ax[2].set_ylabel('$V_{Emitter}$ [V]',color=cols["VE"][0])
                         
    
-                        # Get the right spine of ax[1]
+                        # Get the right spine of ax[1] 
                         bboxes = {}
                         for ax in FIG.ax:
                             bbox = FIG.ax[ax].get_position()
                             
                             bbox.x0 = kw.bounds_padding[0]; bbox.x1 = kw.bounds_padding[1]; 
                             bbox.y0 = kw.bounds_padding[2]; bbox.y1 = kw.bounds_padding[3]; 
                             FIG.ax[ax].set_position(bbox)
                             bboxes[ax] = bbox
 
                         
+                        
                         #We want to set axis limits so that Voltage = 90% of the ylim
                         def rpad(data,ratio):
                             drange = np.max(data)-np.min(data)
                             dpad   = (drange*(1/ratio) - drange)/2
                             return([np.min(data)-dpad,np.max(data)+dpad],dpad)
 
-
-                        Vlim,Vpad = rpad(Em_V,0.9)
+                        V_range = 0.95
+                        
+                        Vlim,Vpad = rpad(Em_V,0.95)
+                        
                         FIG.ax[2].set_ylim(Vlim)
-
-
+                        
+                                                    
                         #This is the ratio of the positive axis over the negative one such that the currents fit underneath the voltage every time 
+                        
                         try: 
-                            RatioMod = (np.max(Em_V) + Vpad)/(Vlim[1] - Vlim[0])
+                            RM1 = np.array([(np.min(Em_V) - Vpad)/(Vlim[1] - Vlim[0]) ,(np.max(Em_V) + Vpad)/(Vlim[1] - Vlim[0])])  
+                            RM2 = np.array([(np.min(Em_I))/(np.max(Em_I) - np.min(Em_I)) ,(np.max(Em_I))/(np.max(Em_I) - np.min(Em_I))])  
                         except:
                             None
-
-                        FIG.ax[0].set_ylim(rpad(Det_I,0.8*RatioMod)[0])
-                        FIG.ax[1].set_ylim(rpad(Em_I,0.85*RatioMod)[0])
+                        #NOTE: 0.5 RATIO MOD means that 0.5 of the TOTAL RANGE should fit.
+                            
+                        maxmod = 1 - np.abs(RM1[1] - RM2[1])
+                        minmod = -(1-np.max(np.abs(RM1)))
+                        #%%
+                        def mod_mod(val):
+                            #0.5 = 2, 1 = 1
+                            mod = 1/val
+                            return(mod)
+                        #%%
+
+                        DetIMod = 1.4*mod_mod(RM1[1])
+                        EmIMod  = 1.2*mod_mod(RM1[1])
+                        
+                        FIG.ax[0].set_ylim(np.max(np.abs(Det_I))*minmod*DetIMod, 
+                                           np.max(np.abs(Det_I))*maxmod*DetIMod)  
+                        FIG.ax[1].set_ylim(np.max(np.abs(Em_I))*minmod*EmIMod,
+                                           np.max(np.abs(Em_I))*maxmod*EmIMod)  
                         
                         align_axis_zeros([FIG.ax[0],FIG.ax[1],FIG.ax[2]])
                         
-                        TICKS = []
-                        for key in FIG.ax.keys():
-                            TICKS.append(FIG.ax[key].get_yticks())
-
-                        align_axis_zeros([FIG.ax[0],FIG.ax[1],FIG.ax[2]])
+                        for nax in FIG.ax:
+                            adjust_ticks(FIG.ax[nax],which="both",Nx=5,Ny=5,xpad=1,ypad=1,respect_zero =True)       #adjust ticks based on original ticks
 
-                        for i,oticks in enumerate(TICKS):
-                            current_ylim = FIG.ax[i].get_ylim()                         #Get current limits
-                            ticks = adjust_ticks(oticks,current_ylim,numticks=12)       #adjust ticks based on original ticks
-                            FIG.ax[i].set_yticks(ticks)                                 #set new tick locations
-                            FIG.ax[i].set_yticklabels([f"{val:.1e}" for val in ticks])  #set new ticklabels
-                            #use the scalar formatter 
-                            yfmt = ScalarFormatterForceFormat()
-                            yfmt.set_powerlimits((-2,2))
-                            FIG.ax[i].yaxis.set_major_formatter(yfmt)
-                            FIG.ax[i].set_ylim(current_ylim)
 
                         ticklabelwidth = dummy_text_params("−0.00",FIG,fontsize=plt.rcParams["ytick.labelsize"],usetex=plt.rcParams["text.usetex"])["width"] # Get the width of the bounding box in figure coordinates
                         #We will get the width of a single "-" in figure coordinates too.
                         minuslabelwidth = dummy_text_params("−",FIG,fontsize=plt.rcParams["ytick.labelsize"],usetex=plt.rcParams["text.usetex"])["width"] # Get the width of the bounding box in figure coordinates
                         
-                        FIG.ax[2].spines.right.set_position(("outward",FIG.fig.dpi*5*ticklabelwidth))
+                        FIG.ax[2].spines.right.set_position(("outward",FIG.fig.dpi*4*ticklabelwidth))
                         
                         
                         #Setting Spine colours and tickparameters
                         FIG.ax[0].yaxis.label.set_color(cols["ID"][0])
                         FIG.ax[1].yaxis.label.set_color(cols["IE"][0])
                         FIG.ax[2].yaxis.label.set_color(cols["VE"][0])
                         
@@ -390,40 +399,43 @@
                         FIG.ax[1].tick_params(axis='y', colors=cols["IE"][0], **tkw)
                         FIG.ax[1].spines["right"].set_color(cols["IE"][0])
                         
                         
                         FIG.ax[2].tick_params(axis='y', colors=cols["VE"][0], **tkw)
                         FIG.ax[2].spines["right"].set_color(cols["VE"][0])
                         FIG.ax[0].tick_params(axis='x', **tkw)
-                        legend = FIG.ax[0].legend(ncol=kw.ncols,handles=[p1, p2, p3],loc=kw.legend_loc,frameon=False) 
+                        legend = FIG.ax[0].legend(ncol=kw.ncols,handles=[p1, p2, p3],loc=kw.legend_loc,frameon=False,columnspacing=0.8,handlelength=1.5) 
                         # Get the font size for the legend text
+                       
                         if kw.legend_loc == "upper center":
                             legendheight = dummy_text_params("DUMMY",FIG,fontsize=plt.rcParams["legend.fontsize"])["height"] # Get the width of the bounding box in figure coordinates
-                            legend.set_bbox_to_anchor((0, 0.75*legendheight, 1, 1))
-                        
+                            for t in legend.get_texts(): t.set_va('bottom')
+                            legend.set_bbox_to_anchor((0, 0.6*legendheight, 1, 1))
+                        t1 = FIG.ax[0].yaxis.get_offset_text().get_position()
+                        t2 = FIG.ax[1].yaxis.get_offset_text().get_position()
+                        FIG.ax[0].yaxis.get_offset_text().set_position((t1[0] - 0.125,t1[1] + 0.125))
+                        FIG.ax[1].yaxis.get_offset_text().set_position((t2[0] + 0.125,t2[1] + 0.125))
+
                         for ax in FIG.ax:
                             FIG.ax[ax].spines["left"].set_color(cols["ID"][0])
-                            FIG.ax[ax].yaxis.grid(False, which='both')
-                            FIG.ax[0].yaxis.grid(True, which='both',color=cmaps["tab20c"](11))
-                        
                         
                         for ax in FIG.ax:
                             if ax != 0:
 
                                 for j, tickobj in enumerate(FIG.ax[ax].get_yticklabels()):
 
                                     ticktext   = tickobj.get_text()
                                     if ticktext == "":
                                         ticktext = "-1"
                                         
-                                    if float(ticktext.replace("−","-"))>=0:
+                                    if float(ticktext.replace("$\\mathdefault{","").replace("}$","").replace("−","-"))>=0:
                                         tick_position = tickobj.get_position()
 
                                         # Create a new position with the x-axis translation
-                                        new_position = (tick_position[0] + minuslabelwidth, tick_position[1])
+                                        new_position = (tick_position[0] + 0.8*minuslabelwidth, tick_position[1])
                          
                                         # Set the new position for the tick label
                                         tickobj.set_position(new_position)
                                         #ticktrans = mpl.transforms.Affine2D().translate(minuslabelwidth*FIG.fig.dpi,0) 
                                         #tickobj.set_transform(tickobj.get_transform() + ticktrans)
             elif "Voltage Linear Sweep" in data["Settings"]["Operation Mode"] and "5_emitter_sweep" in data["Settings"]["Test Name"]:
                 FIG.hold_on = True
@@ -458,22 +470,22 @@
                     Det_I     =  data[Det_I_key][0]
                     #We want all currents to show "foward current", so we must check if the abs(min) > abs(max)
                     
                     if abs(np.max(Det_I)) < abs(np.min(Det_I)):
                         Det_I = -np.array(Det_I)
                     
                     if abs(np.max(Em_I)) < abs(np.min(Em_I)):
-                        if Em_V(Em_I.index(np.min(Em_I))) < 0:
+                        if Em_V[Em_I.index(np.min(Em_I))] < 0:
                             Em_V = -np.array(Em_V)
                             
                         Em_I = -np.array(Em_I)
                     Det_Vmean = np.mean(Det_V)
                     FIG.ax[0].semilogy(Em_V,Det_I,color=cols[FIG.iteration],label="$V_{Det}=$"+f'{Det_Vmean:.3f}')
                     FIG.ax[0].set_xlabel("$V_{Emitter}$ [V]")
-                    FIG.ax[0].set_ylabel("$I_{Detector}$ [I]")
+                    FIG.ax[0].set_ylabel("$I_{Detector}$ [A]")
                     FIG.ax[0].legend()
                     FIG.iteration+=1
         if type(IFIG) != bool:
             # Get the right spine of ax[1]
             bboxes = {}
             for ax in IFIG.ax:
                 bbox = IFIG.ax[ax].get_position()
```

### Comparing `DMU-0.2.8/DMU/utils_utils.py` & `dmu-0.2.9/DMU/utils_utils.py`

 * *Files identical despite different names*

### Comparing `DMU-0.2.8/DMU.egg-info/PKG-INFO` & `dmu-0.2.9/DMU.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: DMU
-Version: 0.2.8
+Version: 0.2.9
 Summary: This package is used to store commonly used functions on pip for the sake of easy pulling for other code.
 Home-page: https://github.com/DeltaMod/DMU
 Author: Atli Vidar Már FLodgren
 Author-email: vidar.flodgren@sljus.lu.se
 Keywords: hello world example examples
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: h5py
-Requires-Dist: matplotlib
-Requires-Dist: hdf5storage
-Requires-Dist: xlrd
 Requires-Dist: natsort
-Requires-Dist: numpy
+Requires-Dist: hdf5storage
 Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: h5py
+Requires-Dist: xlrd
 Requires-Dist: docutils>=0.3
 
 # ATTENTION
 This is just a code-storage repository for small functions I use normally. 
  
 # LDI
```

### Comparing `DMU-0.2.8/LICENSE` & `dmu-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `DMU-0.2.8/PKG-INFO` & `dmu-0.2.9/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: DMU
-Version: 0.2.8
+Version: 0.2.9
 Summary: This package is used to store commonly used functions on pip for the sake of easy pulling for other code.
 Home-page: https://github.com/DeltaMod/DMU
 Author: Atli Vidar Már FLodgren
 Author-email: vidar.flodgren@sljus.lu.se
 Keywords: hello world example examples
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: h5py
-Requires-Dist: matplotlib
-Requires-Dist: hdf5storage
-Requires-Dist: xlrd
 Requires-Dist: natsort
-Requires-Dist: numpy
+Requires-Dist: hdf5storage
 Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: h5py
+Requires-Dist: xlrd
 Requires-Dist: docutils>=0.3
 
 # ATTENTION
 This is just a code-storage repository for small functions I use normally. 
  
 # LDI
```

### Comparing `DMU-0.2.8/README.md` & `dmu-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `DMU-0.2.8/setup.py` & `dmu-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 
 installREQ = [module_filter(modules)+["docutils>=0.3"]]
 installREQ = [[item for item in installREQ[0] if item not in ["logging"]]]
 
 setup(
     name="DMU",
-    version="0.2.8",
+    version="0.2.9",
     packages=find_packages(),
     scripts=[TrgtScr],
 
     # Project uses reStructuredText, so ensure that the docutils get
     # installed or upgraded on the target machine
     install_requires =installREQ,
     package_data={
```

