# Comparing `tmp/PULSEY-0.0.3.tar.gz` & `tmp/PULSEY-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PULSEY-0.0.3.tar", last modified: Wed Jan 24 18:56:19 2024, max compression
+gzip compressed data, was "PULSEY-0.0.4.tar", last modified: Fri Feb 16 20:15:41 2024, max compression
```

## Comparing `PULSEY-0.0.3.tar` & `PULSEY-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-01-24 18:56:19.048641 PULSEY-0.0.3/
--rw-r--r--   0 aayala     (501) staff       (20)      490 2024-01-24 18:56:19.048389 PULSEY-0.0.3/PKG-INFO
-drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-01-24 18:56:19.047336 PULSEY-0.0.3/PULSEY/
--rw-r--r--   0 aayala     (501) staff       (20)    16928 2024-01-24 17:22:26.000000 PULSEY-0.0.3/PULSEY/PULSEY.py
--rw-r--r--   0 aayala     (501) staff       (20)       21 2024-01-24 17:51:01.000000 PULSEY-0.0.3/PULSEY/__init__.py
-drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-01-24 18:56:19.048164 PULSEY-0.0.3/PULSEY.egg-info/
--rw-r--r--   0 aayala     (501) staff       (20)      490 2024-01-24 18:56:19.000000 PULSEY-0.0.3/PULSEY.egg-info/PKG-INFO
--rw-r--r--   0 aayala     (501) staff       (20)      180 2024-01-24 18:56:19.000000 PULSEY-0.0.3/PULSEY.egg-info/SOURCES.txt
--rw-r--r--   0 aayala     (501) staff       (20)        1 2024-01-24 18:56:19.000000 PULSEY-0.0.3/PULSEY.egg-info/dependency_links.txt
--rw-r--r--   0 aayala     (501) staff       (20)        7 2024-01-24 18:56:19.000000 PULSEY-0.0.3/PULSEY.egg-info/top_level.txt
--rw-r--r--   0 aayala     (501) staff       (20)        9 2023-06-21 18:06:32.000000 PULSEY-0.0.3/README.md
--rw-r--r--   0 aayala     (501) staff       (20)      572 2024-01-24 18:08:39.000000 PULSEY-0.0.3/pyproject.toml
--rw-r--r--   0 aayala     (501) staff       (20)       38 2024-01-24 18:56:19.048688 PULSEY-0.0.3/setup.cfg
+drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-02-16 20:15:41.007382 PULSEY-0.0.4/
+-rw-r--r--   0 aayala     (501) staff       (20)      490 2024-02-16 20:15:41.007135 PULSEY-0.0.4/PKG-INFO
+drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-02-16 20:15:41.005896 PULSEY-0.0.4/PULSEY/
+-rw-r--r--   0 aayala     (501) staff       (20)    15452 2024-02-16 20:06:45.000000 PULSEY-0.0.4/PULSEY/PULSEY.py
+-rw-r--r--   0 aayala     (501) staff       (20)       21 2024-01-24 17:51:01.000000 PULSEY-0.0.4/PULSEY/__init__.py
+drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-02-16 20:15:41.006927 PULSEY-0.0.4/PULSEY.egg-info/
+-rw-r--r--   0 aayala     (501) staff       (20)      490 2024-02-16 20:15:41.000000 PULSEY-0.0.4/PULSEY.egg-info/PKG-INFO
+-rw-r--r--   0 aayala     (501) staff       (20)      180 2024-02-16 20:15:41.000000 PULSEY-0.0.4/PULSEY.egg-info/SOURCES.txt
+-rw-r--r--   0 aayala     (501) staff       (20)        1 2024-02-16 20:15:41.000000 PULSEY-0.0.4/PULSEY.egg-info/dependency_links.txt
+-rw-r--r--   0 aayala     (501) staff       (20)        7 2024-02-16 20:15:41.000000 PULSEY-0.0.4/PULSEY.egg-info/top_level.txt
+-rw-r--r--   0 aayala     (501) staff       (20)        9 2023-06-21 18:06:32.000000 PULSEY-0.0.4/README.md
+-rw-r--r--   0 aayala     (501) staff       (20)      572 2024-02-16 20:15:26.000000 PULSEY-0.0.4/pyproject.toml
+-rw-r--r--   0 aayala     (501) staff       (20)       38 2024-02-16 20:15:41.007433 PULSEY-0.0.4/setup.cfg
```

### Comparing `PULSEY-0.0.3/PULSEY/PULSEY.py` & `PULSEY-0.0.4/PULSEY/PULSEY.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,47 +101,44 @@
         Star object with pulsation modes, frequencies, and amplitudes as indicated by user
 
     ### Example
     
     """
 
     #Init function taking freq, amp, etc. to initialize star with features
-    def __init__(self, lmMode, freq, amp, phase, time = np.zeros(1), inc=90, lMax = None, fcn = None, osParam = 2, observed = True, binaryDictionary = None):
+    def __init__(self, lmMode, freq, amp, phase, inc=90, lMax = None, fcn = None, osParam = 2, observed = True):
         #Insert warning if fcn given and no lMax provided (make sure its large enough)
         #See if we can change complexity (lMax) of map after initialization
         self.lmMode = lmMode
         self.freq = freq
         self.amp = amp
         self.phase = phase
         self.inc = inc
         self.fcn = fcn
         self.observed = observed
-        self.time = time
 
         #Save Y2P from pixel transform as feature of star
         
         #Provided lMax means we will transform surface output values SH-maps.  Need to carry along larger transform array.
         if(lMax is None):
             if(len(lmMode) > 0):
                 self.lMax = np.max(self.lmMode)
             else:
                 self.lMax = 0
         else:
             self.lMax = lMax
 
 
         self.nSignals = len(self.lmMode)
-        self._map = starry.Map(ydeg=self.lMax, amp=1.0, inc = self.inc + 90)
+        self._map = starry.Map(ydeg=self.lMax, amp=1.0, inc = self.inc - 90)
         #Look into creating inclination function
 
-        self._computeAmpCoeffs()
-        self.computeMapCoeffs()
-        self._computeFlux()
-
-        self.lat, self.lon, self.Y2P, self.P2Y, self.Dx, self.Dy = self._map.get_pixel_transforms(oversample=osParam)
+        self._computeAmpCoeffs() #Think about renaming
+        #self.computeMapCoeffs()
+        #self._computeFlux()
 
         if self.fcn is not None:
             self.setTransFcn(self.fcn, osParam)
             self.lat, self.lon, self.Y2P, self.P2Y, self.Dx, self.Dy = self._map.get_pixel_transforms(oversample=osParam)
 
     #Transform constructed stellar surface map to new values in accordance with input transform function
     def setTransFcn(self, fcn):
@@ -168,19 +165,19 @@
         """Compute the amplitude coefficients for converting map values to desired observables
 
         ### Parameters
 
         ### Example
         Add example
         """
-        # DESIRED amplitudes set to ampCoeffArray, transform if observed flag is true
-        self.ampCoeffArray = np.ones(self.nSignals)
+        # DESIRED amplitudes set to ampScaleFactor, transform if observed flag is true
+        self.ampScaleFactor = np.ones(self.nSignals)
         self.phaseOffsetArray = np.zeros(self.nSignals)
 
-        #Sample map over arbitrary time to retrieve necessarry amplitudes and phase to combine for constructing desired surfacd map
+        #Sample map over arbitrary time to retrieve necessary amplitudes and phase to combine for constructing desired surfacd map
         for i in range(len(self.lmMode)):
             timeSample = np.arange(0,1,0.25)
             testFluxArray = np.zeros(len(timeSample))
             for j, t in enumerate(timeSample):
                 self._map.y[1:] = 0.0
                 l = self.lmMode[i][0]
                 m = self.lmMode[i][1]
@@ -191,113 +188,63 @@
 
                 testFluxArray[j] = self._map.flux()
 
             #Save amp and phase coefficients for use in map construction
             maxAmp = np.nanmax(testFluxArray)
             maxAmp = maxAmp-1.0
             if self.observed:
-                self.ampCoeffArray[i] = 1.0/maxAmp
-                if(self.ampCoeffArray[i] > 1.0):
+                self.ampScaleFactor[i] = 1.0/maxAmp
+                if(self.ampScaleFactor[i] > 1.0):
                     warnings.warn("WARNING: Producing unphysical amplitude values!")
                     
             self.phaseOffsetArray[i] = (timeSample[np.argmax(testFluxArray)]-0.25)
 
     #Compute coefficients necessary to construct surface maps for pulsation over given time sample
-    def computeMapCoeffs(self):
-        """Construct surface maps for every timestamp in the given time period
-
-        ### Parameters
-
-        timeArray : array_like (float, 1D)
-            Time values over which to construct surface maps
-
-        ### Example
-        
-        """
-
-
-        #Remove saving pos/neg Coeffs to self._map.  Store directly in self.coeffArray
-        self.coeffArray = np.zeros((len(self.time), len(self._map.y)))
-        for i,t in enumerate(self.time):
-            self.coeffArray[i,:] = self.getMapCoeffs([t])
-            ###Insert function transform
-            if self.fcn is not None:
-                p = self.Y2P.dot(self._map.y)
-                newP = self.fcn(p)
-                self.coeffArray[i,:] = self.P2Y.dot(newP)
-                #print(p, newP, self.coeffArray[i])
-
-
     #Compute coefficients necessary to construct surface maps for pulsation over given time sample
-    def getMapCoeffs(self, time):
+    def computePulsation(self, time):
         """Construct surface maps for every timestamp in the given time period
 
         ### Parameters
 
         timeArray : array_like (float, 1D)
             Time values over which to construct surface maps
 
         ### Example
         
         """
 
-
         #Remove saving pos/neg Coeffs to self._map.  Store directly in self.coeffArray
 
         if not hasattr(time, '__iter__'):
             time = [time]
         
         coeffArray = np.zeros((len(time),len(self._map.y)))
         coeffArray[:,0] = 1.0
         for i,t in enumerate(time):
             for j in range(self.nSignals):
                     l = self.lmMode[j][0]
                     m = self.lmMode[j][1]
-                    posC,negC = _LxMx(t, m, frequency=self.freq[j],amp=self.amp[j]*self.ampCoeffArray[j], 
+                    posC,negC = _LxMx(t, m, frequency=self.freq[j],amp=self.amp[j]*self.ampScaleFactor[j], 
                                         phase0=self.phase[j]+self.phaseOffsetArray[j])
                     
                     #print(posC)
 
                     coeffArray[i,lmIndex(l, np.abs(m))] += posC
                     if m != 0:
                         coeffArray[i,lmIndex(l,-np.abs(m))] += negC
 
+            if self.fcn is not None:
+                p = self.Y2P.dot(coeffArray[i,:])
+                newP = self.fcn(p)
+                coeffArray[i,:] = self.P2Y.dot(newP)
+
         return coeffArray
 
     #Calculate flux of surface map pulsation over given time sample (time Array given HERE)
-    def _computeFlux(self, binaryIndicator=False):
-        """Compute output flux of star object over input time array and save as feature of star
-
-        ### Parameters
-
-        timeArray : array_like (float, 1D)
-            Time values over which to construct surface maps
-
-        binaryIndicator : boolean (deafault = False)
-            Flag indicating whether star is in binary system
-        
-        
-        ### Returns
-
-        fluxArray : array_like (float, 1D)
-            Integrated disc flux values of star at each value of timeArray 
-
-        ### Example
-        
-        """
-        
-        
-        self.flux = self.getFlux(self.time, binaryIndicator)
-
-    
-    #Internal starry dummy object
-
-    
-
-    def getFlux(self, time, binaryIndicator=False):
+    def computeFlux(self, time, binaryIndicator=False):
         """Compute output flux of star object over input time array and save as feature of star
 
         ### Parameters
 
         timeArray : array_like (float, 1D)
             Time values over which to construct surface maps
 
@@ -309,15 +256,15 @@
 
         fluxArray : array_like (float, 1D)
             Integrated disc flux values of star at each value of timeArray 
 
         ### Example
         
         """
-        coeffArray = self.getMapCoeffs(time)
+        coeffArray = self.computePulsation(time)
         fluxArray = np.zeros(len(time))
 
 
         if binaryIndicator == True:
             for i,t in enumerate(time):
                 self.sys.primary.map.y[1:] = coeffArray[i][1:]
                 fluxArray[i] = self.sys.flux(t)
@@ -364,34 +311,34 @@
         sec = starry.Secondary(starry.Map(ydeg=0, inc=0, amp=sbRatio), r=r2, m=m2, porb=period, prot=np.inf, t0=t0, inc=90)
 
         self.sys = starry.System(pri, sec)
 
 
 
     #Function for computing flux map for SPECIFIC time instance and outputs map
-    def setTime(self, time, binaryFlag):
-        """Construct surface map at specific time isntance and associate time value as a feature of star
+    # def setTime(self, time, binaryFlag):
+    #     """Construct surface map at specific time isntance and associate time value as a feature of star
 
-        ### Parameters
+    #     ### Parameters
 
-        time : float
-            Time value last associated with given star object
+    #     time : float
+    #         Time value last associated with given star object
 
-        binaryFlag : boolean (deafault = False)
-            Flag indicating whether star is in binary system
+    #     binaryFlag : boolean (deafault = False)
+    #         Flag indicating whether star is in binary system
         
         
-        ### Returns
+    #     ### Returns
 
-        ### Example
-        Returns the desired output
-        """
+    #     ### Example
+    #     Returns the desired output
+    #     """
 
-        _ = self.getFlux([time], binaryIndicator=binaryFlag)
-        #self.time = time
+    #     _ = self.getFlux([time], binaryIndicator=binaryFlag)
+    #     #self.time = time
 
     #Visualize should take a time parameter
     def visualizeStar(self):
         """Construct animated gif visualizing star's pulsation over specific time period
 
         ### Parameters
         
@@ -477,15 +424,15 @@
 
 # Loop to create true flux array using newly determined phase offset values
 for i,time in enumerate(timeArray):
     map.y[1:] = 0
     for j in range(len(freq)):
             l = lmMode[j][0]
             m = lmMode[j][1]
-            posC,negC = _LxMx(time, m, frequency=freq[j],amp=amp[j]*ampCoeffArray[j], phase0=phase[j]+phaseOffsetArray[j])
+            posC,negC = _LxMx(time, m, frequency=freq[j],amp=amp[j]*ampScaleFactor[j], phase0=phase[j]+phaseOffsetArray[j])
 
             map[l,np.abs(m)]  += posC
             if m != 0:
                 map[l,-np.abs(m)] += negC
             
     fluxArray[i] = map.flux()
     mapArray[i] = map.render()
```

### Comparing `PULSEY-0.0.3/pyproject.toml` & `PULSEY-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PULSEY"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Andrew Ayala", email="andrew.ayala.2018@gmail.com" },
 ]
 description = "Stellar Pulsation Package"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

