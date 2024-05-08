# Comparing `tmp/whatshow_phy_mod_otfs-2.1.1.tar.gz` & `tmp/whatshow_phy_mod_otfs-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshow_phy_mod_otfs-2.1.1.tar", last modified: Sat May  4 06:55:03 2024, max compression
+gzip compressed data, was "whatshow_phy_mod_otfs-2.1.2.tar", last modified: Tue May  7 14:02:55 2024, max compression
```

## Comparing `whatshow_phy_mod_otfs-2.1.1.tar` & `whatshow_phy_mod_otfs-2.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 06:55:03.186038 whatshow_phy_mod_otfs-2.1.1/
--rw-rw-rw-   0        0        0    13032 2024-05-04 06:55:03.183699 whatshow_phy_mod_otfs-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    12916 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 06:55:03.186038 whatshow_phy_mod_otfs-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      408 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 06:55:03.161924 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/
--rw-rw-rw-   0        0        0    26618 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/OTFS.py
--rw-rw-rw-   0        0        0    15905 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/OTFSDetector.py
--rw-rw-rw-   0        0        0    27873 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/OTFSResGrid.py
--rw-rw-rw-   0        0        0      100 2024-05-04 06:54:49.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 06:55:03.180700 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/
--rw-rw-rw-   0        0        0    13032 2024-05-04 06:55:02.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-05-04 06:55:02.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 06:55:02.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-04 06:55:02.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-04 06:55:02.000000 whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 14:02:55.327736 whatshow_phy_mod_otfs-2.1.2/
+-rw-rw-rw-   0        0        0    13032 2024-05-07 14:02:55.325726 whatshow_phy_mod_otfs-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12916 2024-05-07 14:02:54.000000 whatshow_phy_mod_otfs-2.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:02:55.327736 whatshow_phy_mod_otfs-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      408 2024-05-07 14:02:54.000000 whatshow_phy_mod_otfs-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:02:55.306728 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs/
+-rw-rw-rw-   0        0        0    26618 2024-05-07 14:02:54.000000 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs/OTFS.py
+-rw-rw-rw-   0        0        0    15922 2024-05-07 14:02:54.000000 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs/OTFSDetector.py
+-rw-rw-rw-   0        0        0    28494 2024-05-07 14:02:54.000000 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs/OTFSResGrid.py
+-rw-rw-rw-   0        0        0      100 2024-05-07 14:02:54.000000 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:02:55.322726 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs.egg-info/
+-rw-rw-rw-   0        0        0    13032 2024-05-07 14:02:55.000000 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-05-07 14:02:55.000000 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:02:55.000000 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-07 14:02:55.000000 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-07 14:02:55.000000 whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs.egg-info/top_level.txt
```

### Comparing `whatshow_phy_mod_otfs-2.1.1/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow_phy_mod_otfs
-Version: 2.1.1
+Version: 2.1.2
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.1-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.1-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.2-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.2-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

### Comparing `whatshow_phy_mod_otfs-2.1.1/README.md` & `whatshow_phy_mod_otfs-2.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.1-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.1-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.2-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.2-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delay–Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

### Comparing `whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/OTFS.py` & `whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs/OTFS.py`

 * *Files identical despite different names*

### Comparing `whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/OTFSDetector.py` & `whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs/OTFSDetector.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,15 @@
             
     ###########################################################################
     # detectors
     '''
     MP base (proposed by P. Raviteja in 2017) from Emanuele Viterbo Research Group
     '''
     def detectMPBase(self):
+        # TODO:
         # input check
         if self.No is None or self.No.ndim != 0:
             raise Exception("The noise power must be a scalar.");
         # set data
         conv_rate_prev = -0.1 if self.batch_size == self.BATCH_SIZE_NO else np.tile(-0.1, self.batch_size);
         Y_DD = self.y_rg.getContent();
         pg_num, pg_l_beg, pg_l_end, pg_k_beg, pg_k_end = self.y_rg.getAreaPG();   # PG
```

### Comparing `whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs/OTFSResGrid.py` & `whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs/OTFSResGrid.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     @pilots_pow:    pilot power to generate random pilots
     '''
     def map(self, symbols, *, pilots=[], pilots_pow=None):
         self.pilots = np.asarray(pilots);
         # calculate PG & CE area
         self.calcAreaPGCE();
         # insert
-        self.insertDA(np.asarray(symbols));
+        self.insertDA(symbols);
         self.insertP(pilots_pow);
         
     '''
     set the channel estimate area (CE area is set in `map`, if you want to use your own area, call this)
     @ce_l_beg: CE delay beginning
     @ce_l_end: CE delay ending
     @ce_k_beg: CE Doppler beginning
@@ -221,28 +221,37 @@
         self.ce_doppl_beg = ce_doppl_beg;
         self.ce_doppl_end = ce_doppl_end;
         self.ce_num = (ce_delay_end - ce_delay_beg + 1)*(ce_doppl_end - ce_doppl_beg + 1);
     
     '''
     demap
     @isData:        whether give the data
+    @isDataVec:     whether the data is vectorized (default: true)
     @isCE:          whether give the channel estimation result
     @threshold:     the threshold to estimate the channel
     '''
-    def demap(self, *, isData=True, isCE=True, threshold=0):
+    def demap(self, *, isData=True, isDataVec=True, isCE=True, threshold=0):
         # input check          
         # input check - threshold
         if threshold < 0:
             raise Exception("The threshould must be non-negative.");
         # input check - pulse_type
         if self.pulse_type == self.PULSE_NO:
             raise Exception("The pulse type has to be set before demapping.");
 
         # y
-        y = self.getContentNoCE() if isData else None;
+        y = None;
+        if isData:
+            if self.pilot_type == self.PILOT_TYPE_EM:
+                if isDataVec:
+                    y = self.getContentNoCE();
+                else:
+                    y = self.getContentZeroCE();
+            elif self.pilot_type == self.PILOT_TYPE_SP:
+                    y = self.getContent(isVector=isDataVec);
         his = None;
         lis = None;
         kis = None;
         # need to estimate the channel & have pilots
         if isCE and self.isPG():
             if self.p_len == 1:
                 his, lis, kis = self.estimateChannel4SingPilot(threshold);
@@ -450,41 +459,43 @@
             if (self.pl1+self.pl_len-1) + self.gl_len_pos >= self.nSubcarNum:
                 raise Exception("The guard (pos) on delay axis overflows.");
             if self.pk1 - self.gk_len_neg < 0:
                 raise Exception("The guard (neg) on Doppler axis overflows.");
             if (self.pk1+self.pk_len-1) + self.gk_len_pos >= self.nTimeslotNum:
                 raise Exception("The guard (pos) on Doppler axis overflows.");
             # calculate PG area
-            if self.pilot_type == self.PILOT_TYPE_EM:
+            if self.pilot_type == self.PILOT_TYPE_EM or self.pilot_type == self.PILOT_TYPE_SP:
                 # PG area only exist when using embedded pilots
                 self.pg_num = ((self.pl_len+self.gl_len_neg+self.gl_len_pos)*(self.pk_len+self.gk_len_neg+self.gk_len_pos)).astype(int);
                 self.pg_delay_beg = (self.pl1 - self.gl_len_neg).astype(int);
                 self.pg_delay_end = (self.pl1 + self.pl_len - 1 + self.gl_len_pos).astype(int);
                 self.pg_doppl_beg = (self.pk1 - self.gk_len_neg).astype(int);
                 self.pg_doppl_end = (self.pk1 + self.pk_len - 1 + self.gk_len_pos).astype(int);
             # calulate channel estimate area
-            if self.gl_len_ful:
-                self.ce_delay_beg = 0;
-                self.ce_delay_end = (self.nSubcarNum - 1).astype(int);
-            else:
-                self.ce_delay_beg = (self.pg_delay_beg + self.gl_len_neg).astype(int);
-                self.ce_delay_end = (self.pg_delay_end).astype(int);
-            if self.gk_len_ful:
-                self.ce_doppl_beg = 0;
-                self.ce_doppl_end = (self.nTimeslotNum - 1).astype(int);
-            else:
-                self.ce_doppl_beg = (self.pg_doppl_beg + floor(self.gk_len_neg/2)).astype(int);
-                self.ce_doppl_end = (self.pg_doppl_end - floor(self.gk_len_pos/2)).astype(int);
-            self.ce_num = ((self.ce_delay_end - self.ce_delay_beg + 1)*(self.ce_doppl_end - self.ce_doppl_beg + 1)).astype(int);
+            if self.pilot_type == self.PILOT_TYPE_EM or self.pilot_type == self.PILOT_TYPE_SP:
+                if self.gl_len_ful:
+                    self.ce_delay_beg = 0;
+                    self.ce_delay_end = (self.nSubcarNum - 1).astype(int);
+                else:
+                    self.ce_delay_beg = (self.pg_delay_beg + self.gl_len_neg).astype(int);
+                    self.ce_delay_end = (self.pg_delay_end).astype(int);
+                if self.gk_len_ful:
+                    self.ce_doppl_beg = 0;
+                    self.ce_doppl_end = (self.nTimeslotNum - 1).astype(int);
+                else:
+                    self.ce_doppl_beg = (self.pg_doppl_beg + floor(self.gk_len_neg/2)).astype(int);
+                    self.ce_doppl_end = (self.pg_doppl_end - floor(self.gk_len_pos/2)).astype(int);
+                self.ce_num = ((self.ce_delay_end - self.ce_delay_beg + 1)*(self.ce_doppl_end - self.ce_doppl_beg + 1)).astype(int);
 
     '''
     insert data
     @symbols: symbols to map a vector
     '''
     def insertDA(self, symbols):
+        symbols = self.squeeze(symbols).copy();
         # input check
         if self.pilot_type == self.PILOT_TYPE_SP:
             data_num = self.nTimeslotNum*self.nSubcarNum - self.zp_len*self.nTimeslotNum;
         else:
             data_num = self.nTimeslotNum*self.nSubcarNum - self.pg_num - self.zp_len*self.nTimeslotNum;
         # input check - symbols
         if not self.isvector(symbols):
@@ -498,15 +509,15 @@
         elif data_num == self.nSubcarNum*self.nTimeslotNum - self.zp_len*self.nTimeslotNum:
             self.content = np.append(self.reshape(symbols, self.nTimeslotNum, (self.nSubcarNum - self.zp_len)), self.zeros(self.zp_len, self.nTimeslotNum));
         else:
             symbols_id = 0;
             for doppl_id in range(self.nTimeslotNum):
                 for delay_id in range(self.nSubcarNum):
                     if self.isInAreaDA(doppl_id, delay_id):
-                        if self.isInAreaPG(doppl_id, delay_id):
+                        if self.batch_size == self.BATCH_SIZE_NO:
                             self.content[doppl_id, delay_id] = symbols[symbols_id];
                         else:
                             self.content[..., doppl_id, delay_id] = symbols[..., symbols_id];
                         symbols_id = symbols_id + 1;
             assert(symbols_id == data_num);
 
     '''
```

### Comparing `whatshow_phy_mod_otfs-2.1.1/whatshow_phy_mod_otfs.egg-info/PKG-INFO` & `whatshow_phy_mod_otfs-2.1.2/whatshow_phy_mod_otfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatshow-phy-mod-otfs
-Version: 2.1.1
+Version: 2.1.2
 Description-Content-Type: text/markdown
 
 # OTFS Modulation
-[![PyPi](https://img.shields.io/badge/PyPi-2.1.1-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.1-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
+[![PyPi](https://img.shields.io/badge/PyPi-2.1.2-blue)](https://pypi.org/project/whatshow-phy-mod-otfs/) [![MathWorks](https://img.shields.io/badge/MathWorks-2.1.2-red)](https://mathworks.com/matlabcentral/fileexchange/161136-whatshow_phy_mod_otfs)
 
 This repository is a fundamental toolbox of OTFS modulation crossing `matlab` and `python`. This repositiory is based on papers below:
 > Raviteja, P., Phan, K. T., Hong, Y., & Viterbo, E. (2018). Interference cancellation and iterative detection for orthogonal time frequency space modulation. *IEEE transactions on wireless communications, 17(10)*, 6501-6515.
 
 > Raviteja, P., Phan, K. T., & Hong, Y. (2019). Embedded pilot-aided channel estimation for OTFS in delayâ€“Doppler channels. *IEEE transactions on vehicular technology, 68(5)*, 4906-4917.
 
 ## How to use
```

