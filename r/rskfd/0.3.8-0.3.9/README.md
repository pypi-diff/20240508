# Comparing `tmp/rskfd-0.3.8.tar.gz` & `tmp/rskfd-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rskfd-0.3.8.tar", last modified: Tue Apr 16 13:27:37 2024, max compression
+gzip compressed data, was "rskfd-0.3.9.tar", last modified: Wed May  8 16:08:20 2024, max compression
```

## Comparing `rskfd-0.3.8.tar` & `rskfd-0.3.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.792232 rskfd-0.3.8/
--rw-rw-rw-   0        0        0     2248 2024-04-16 13:27:37.792232 rskfd-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     1386 2020-07-13 06:29:17.000000 rskfd-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.760985 rskfd-0.3.8/examples/
--rw-rw-rw-   0        0        0     3705 2023-02-16 10:45:21.000000 rskfd-0.3.8/examples/Wv2BinStream.py
--rw-rw-rw-   0        0        0      984 2023-11-21 08:38:13.000000 rskfd-0.3.8/examples/fileopening.py
--rw-rw-rw-   0        0        0     6637 2020-10-13 07:00:50.000000 rskfd-0.3.8/examples/instrumentexamples.py
--rw-rw-rw-   0        0        0     1082 2020-07-08 13:59:40.000000 rskfd-0.3.8/license.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.760985 rskfd-0.3.8/rskfd/
--rw-rw-rw-   0        0        0     1299 2023-03-15 14:55:14.000000 rskfd-0.3.8/rskfd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.776609 rskfd-0.3.8/rskfd/helper/
--rw-rw-rw-   0        0        0     4389 2024-04-15 19:01:01.000000 rskfd-0.3.8/rskfd/helper/helper.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.776609 rskfd-0.3.8/rskfd/iq_data_handling/
--rw-rw-rw-   0        0        0    21129 2024-04-16 13:07:29.000000 rskfd-0.3.8/rskfd/iq_data_handling/iqdata.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.792232 rskfd-0.3.8/rskfd/remote_control/
--rw-rw-rw-   0        0        0    14935 2024-04-16 04:51:55.000000 rskfd-0.3.8/rskfd/remote_control/instrument.py
--rw-rw-rw-   0        0        0     1352 2022-06-15 06:04:19.000000 rskfd-0.3.8/rskfd/remote_control/instrumentRS.py
--rw-rw-rw-   0        0        0      675 2019-12-09 13:08:45.000000 rskfd-0.3.8/rskfd/remote_control/instrumentRSExceptions.py
--rw-rw-rw-   0        0        0     8562 2024-04-15 13:54:25.000000 rskfd-0.3.8/rskfd/remote_control/instrumentRS_FSW.py
--rw-rw-rw-   0        0        0     1905 2019-12-09 13:10:19.000000 rskfd-0.3.8/rskfd/remote_control/instrumentRS_VSE.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.792232 rskfd-0.3.8/rskfd/signal_generation/
--rw-rw-rw-   0        0        0     2290 2020-12-11 07:28:48.000000 rskfd-0.3.8/rskfd/signal_generation/signal_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.792232 rskfd-0.3.8/rskfd/snp_handling/
--rw-rw-rw-   0        0        0     9605 2021-03-16 15:49:04.000000 rskfd-0.3.8/rskfd/snp_handling/snpfiles.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:27:37.792232 rskfd-0.3.8/rskfd.egg-info/
--rw-rw-rw-   0        0        0     2248 2024-04-16 13:27:37.000000 rskfd-0.3.8/rskfd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2024-04-16 13:27:37.000000 rskfd-0.3.8/rskfd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 13:27:37.000000 rskfd-0.3.8/rskfd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 13:27:37.000000 rskfd-0.3.8/rskfd.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2024-04-16 13:27:37.000000 rskfd-0.3.8/rskfd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-16 13:27:37.792232 rskfd-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1439 2024-04-16 13:27:01.000000 rskfd-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.600732 rskfd-0.3.9/
+-rw-rw-rw-   0        0        0     2248 2024-05-08 16:08:20.600732 rskfd-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1386 2020-07-13 06:29:17.000000 rskfd-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.540302 rskfd-0.3.9/examples/
+-rw-rw-rw-   0        0        0     3705 2023-02-16 10:45:21.000000 rskfd-0.3.9/examples/Wv2BinStream.py
+-rw-rw-rw-   0        0        0     1322 2024-05-08 14:30:04.000000 rskfd-0.3.9/examples/fileopening.py
+-rw-rw-rw-   0        0        0     6637 2020-10-13 07:00:50.000000 rskfd-0.3.9/examples/instrumentexamples.py
+-rw-rw-rw-   0        0        0     1082 2020-07-08 13:59:40.000000 rskfd-0.3.9/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.548354 rskfd-0.3.9/rskfd/
+-rw-rw-rw-   0        0        0     1299 2023-03-15 14:55:14.000000 rskfd-0.3.9/rskfd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.568528 rskfd-0.3.9/rskfd/helper/
+-rw-rw-rw-   0        0        0     4389 2024-04-15 19:01:01.000000 rskfd-0.3.9/rskfd/helper/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.570543 rskfd-0.3.9/rskfd/iq_data_handling/
+-rw-rw-rw-   0        0        0    21282 2024-05-08 14:18:43.000000 rskfd-0.3.9/rskfd/iq_data_handling/iqdata.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.590685 rskfd-0.3.9/rskfd/remote_control/
+-rw-rw-rw-   0        0        0    14935 2024-04-16 04:51:55.000000 rskfd-0.3.9/rskfd/remote_control/instrument.py
+-rw-rw-rw-   0        0        0     1352 2022-06-15 06:04:19.000000 rskfd-0.3.9/rskfd/remote_control/instrumentRS.py
+-rw-rw-rw-   0        0        0      675 2019-12-09 13:08:45.000000 rskfd-0.3.9/rskfd/remote_control/instrumentRSExceptions.py
+-rw-rw-rw-   0        0        0     8562 2024-04-15 13:54:25.000000 rskfd-0.3.9/rskfd/remote_control/instrumentRS_FSW.py
+-rw-rw-rw-   0        0        0     1905 2019-12-09 13:10:19.000000 rskfd-0.3.9/rskfd/remote_control/instrumentRS_VSE.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.590685 rskfd-0.3.9/rskfd/signal_generation/
+-rw-rw-rw-   0        0        0     2290 2020-12-11 07:28:48.000000 rskfd-0.3.9/rskfd/signal_generation/signal_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.590685 rskfd-0.3.9/rskfd/snp_handling/
+-rw-rw-rw-   0        0        0     9605 2021-03-16 15:49:04.000000 rskfd-0.3.9/rskfd/snp_handling/snpfiles.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:08:20.600732 rskfd-0.3.9/rskfd.egg-info/
+-rw-rw-rw-   0        0        0     2248 2024-05-08 16:08:20.000000 rskfd-0.3.9/rskfd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-05-08 16:08:20.000000 rskfd-0.3.9/rskfd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 16:08:20.000000 rskfd-0.3.9/rskfd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-08 16:08:20.000000 rskfd-0.3.9/rskfd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-05-08 16:08:20.000000 rskfd-0.3.9/rskfd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-08 16:08:20.608781 rskfd-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1439 2024-05-08 16:06:54.000000 rskfd-0.3.9/setup.py
```

### Comparing `rskfd-0.3.8/PKG-INFO` & `rskfd-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rskfd
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python Package for Instrument Control and Data Handling
 Home-page: https://gitlab.com/ramian/rskfd
 Download-URL: https://gitlab.com/ramian/rskfd/
 Author: Florian Ramian
 Author-email: gitlab@ramian.eu
 License: MIT
 Keywords: INSTRUMENT CONTROL,I/Q DATA,WV,IQ.TAR
```

### Comparing `rskfd-0.3.8/README.md` & `rskfd-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/examples/Wv2BinStream.py` & `rskfd-0.3.9/examples/Wv2BinStream.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/examples/fileopening.py` & `rskfd-0.3.9/examples/fileopening.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,11 +33,21 @@
 def ReadWvTest():
     '''
     Test the wv reading routine (tags!!)
     '''
     iq, fs = rskfd.ReadWv(r'\\myserver\signal\higher_qams.wv')
 
 
+def ReadIqTar64bitTest():
+    '''
+    Test the wv reading routine (tags!!)
+    '''
+    iq,fs = rskfd.ReadIqTar(r'C:\Users\ramian\Documents\k18\testing\AmptoolsMeas.iq.tar')
+    #iq = rskfd.ReadIqw(r'C:\Users\ramian\Downloads\iq_data.complex.float64', BytesPerValue=8)
+    rskfd.ShowLogFFT(iq)
+    pass
+
+
 if __name__ == "__main__":
-	pass
-    ReadWvTest()
-    
+	#pass
+    #ReadWvTest()
+    ReadIqTar64bitTest()
```

### Comparing `rskfd-0.3.8/examples/instrumentexamples.py` & `rskfd-0.3.9/examples/instrumentexamples.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/license.txt` & `rskfd-0.3.9/license.txt`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/rskfd/__init__.py` & `rskfd-0.3.9/rskfd/__init__.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/rskfd/helper/helper.py` & `rskfd-0.3.9/rskfd/helper/helper.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/rskfd/iq_data_handling/iqdata.py` & `rskfd-0.3.9/rskfd/iq_data_handling/iqdata.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,40 +88,45 @@
     except:
         logging.error("File (" + FileName +") write error!" )
     
     return NumberOfSamples
 
 
 
-def ReadIqw( FileName, iqiq = True):
+def ReadIqw( FileName, iqiq=True, BytesPerValue=4):
     """Reads an IQW (can be iiqq or iqiq) file. Returns complex samples.
     If iqiq is True, samples are read pairwise (IQIQIQ),
     otherwise in blocks, i first then q (IIIQQQ)
     Note: IIIQQQ is a deprecated format, don't use it for new files.
-    iqList = ReadIqw("MyFile.iqw", iqiq = True)"""
-    
+    iqList = ReadIqw("MyFile.iqw", iqiq = True)
+    BytesPerValue specifies the word length per I/Q sample in the file"""
+
     import struct
     import logging
-        
-    BytesPerValue = 4
-    
+
     try:
         file = open( FileName, "rb")
         data = file.read()
         file.close
     except:
-        logging.error( "File open error ("+ FileName+")!")    
-        
+        logging.error("File open error (" + FileName+")!")
+
     ReadSamples = len(data) // BytesPerValue
-    data = list(struct.unpack("f"*ReadSamples, data))
+    if BytesPerValue == 4:
+        data = list(struct.unpack("f"*ReadSamples, data))
+    elif BytesPerValue == 8:
+        data = list(struct.unpack("d"*ReadSamples, data))
+    else:
+        logging.error("Unsupported word length!")
+
     if iqiq:
-        data = Iqiq2Complex( data) 
+        data = Iqiq2Complex(data)
     else:
-        data = Iiqq2Complex( data)
-    
+        data = Iiqq2Complex(data)
+
     return data
 
 
 
 def WriteBin( iqData, fSamplingRate, FileName):
     """Writes a bin file, e.g. for use on KS generators
     iqData can be a list of complex or list of floats (iqiqiq format mandatory).
@@ -135,41 +140,41 @@
     import logging
 
     #check if iqData is complex
     if isinstance( iqData[0], complex):
         iqData = Complex2Iqiq( iqData)
 
     NumberOfSamples = len(iqData) // 2
-  
+
     #Find maximum magnitude and scale for max to be FullScale (1.0)
     power = []
     for n in range(NumberOfSamples):
         power.append(abs(iqData[2*n]**2 + iqData[2*n+1]**2))
     scaling = math.sqrt( max(power))
 
     # normalize to magnitude 1
     iqData = [ iq / scaling for iq in iqData]
 
     #calculate rms in dB (below full scale)
     rms = math.sqrt(sum(power)/NumberOfSamples)/scaling
     rms = abs(20*math.log10( rms))
     # Convert to int16, use floor function, otherwise distribution is not correct
     iqData = [ math.floor(iq * 32767 +.5) for iq in iqData]
-        
+
     try:
         file = open( FileName, "wb")
 
         # binary block, big endian
         for nIdx in range(len(iqData)):
             file.write( struct.pack(">h",iqData[nIdx]))
 
         file.close()
     except:
         logging.error("File (" + FileName +") write error!" )
-        
+
     return NumberOfSamples
 
 
 
 def WriteWv( iqData, fSamplingRate, FileName):
     """Writes a WV file.
     iqData can be a list of complex or list of floats (iqiqiq format mandatory).
@@ -300,23 +305,22 @@
 
     if ReadData:
         return data, SamplingRate
     else:
         return SamplingRate, NumberOfSamples, RmsLevelOffset, RfRmsLevel
 
 
-
-def __WriteXml( fs, NumberOfSamples, filenameiqw, filenamexml, fCenterFrequency = 0):
+def __WriteXml(fs, NumberOfSamples, filenameiqw, filenamexml, fCenterFrequency=0):
     """Function to write the xml part of the iq.tar
     __WriteXml( samplingrate, numberofsamples, filenameiqw, filenamexml)"""
-    
+
     from datetime import datetime
-    
-    xmlfile = open ( filenamexml, "w")
-    
+
+    xmlfile = open(filenamexml, "w")
+
     xmlfile.write("<?xml version=\"1.0\" encoding=\"UTF-8\"?>\n")
     xmlfile.write("<?xml-stylesheet type=\"text/xsl\" href=\"open_IqTar_xml_file_in_web_browser.xslt\"?>\n")
     xmlfile.write("<RS_IQ_TAR_FileFormat fileFormatVersion=\"2\" xsi:noNamespaceSchemaLocation=\"http://www.rohde-schwarz.com/file/RsIqTar.xsd\" xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\">\n")
     #Optional
     xmlfile.write("<Name>Python iq.tar Writer (iqdata.py)</Name>\n")
     #Optional
     xmlfile.write("<Comment>RS WaveForm, TheAE-RA</Comment>\n")
@@ -329,140 +333,140 @@
     xmlfile.write("<ScalingFactor unit=\"V\">1</ScalingFactor>\n")
     #Optional
     #xmlfile.write("<NumberOfChannels>1</NumberOfChannels>\n")
     xmlfile.write("<DataFilename>" + filenameiqw+ "</DataFilename>\n")
     #Optional
     if fCenterFrequency != 0:
         xmlfile.write( f'<UserData><RohdeSchwarz><SpectrumAnalyzer><CenterFrequency unit="Hz">{fCenterFrequency}</CenterFrequency></SpectrumAnalyzer></RohdeSchwarz></UserData>\n')
-    
+
     xmlfile.write("</RS_IQ_TAR_FileFormat>\n")
     xmlfile.close()
-    
+
     return
 
 
 
 def WriteIqTar( iqData, fs, FileName, fCenterFrequency = 0):
     """Writes an iq.tar file. Complex iqData values are interpreted as Volts.
     iqData can be a list of complex or list of floats (iqiqiq format).
     writtenSamples = WriteIqTar(iqList,fs,"MyFile.iq.tar")"""
-    
+
     import tarfile
     import os
     import re
     import logging
-    
+
     path,filename = os.path.split(FileName)
-       
+
     #Create binary file
     binaryfile = re.sub( "iq.tar", "complex.1ch.float32", filename, flags=re.IGNORECASE)
     NumberOfSamples = WriteIqw( iqData, os.path.join(path, binaryfile))
     if NumberOfSamples == 0:
         return 0
-    
+
     #xsltfilename = "open_IqTar_xml_file_in_web_browser.xslt"
-    
+
     xmlfilename = re.sub( "iq.tar", "xml", filename, flags=re.IGNORECASE)
     __WriteXml( fs, NumberOfSamples, binaryfile, os.path.join(path, xmlfilename), fCenterFrequency=fCenterFrequency)
-    
+
     try:
         tar = tarfile.open( FileName, "w")
         tar.add( os.path.join(path, binaryfile), arcname=binaryfile)
         #xslt is optional
         #tar.add( os.path.join(path, xsltfilename), arcname=xsltfilename)
         tar.add( os.path.join(path, xmlfilename), arcname=xmlfilename)
         tar.close()
         os.remove( os.path.join(path, binaryfile))
         os.remove( os.path.join(path, xmlfilename))
     except:
         logging.error("IqTar (" + FileName +") write error!" )
-    
+
     return NumberOfSamples
 
 
 
-def ReadIqTar( FileName, ChannelToRead = 1):
+def ReadIqTar( FileName, ChannelToRead = 1, BytesPerValue = 4):
     """Reads an iq.tar file. 
     data,fs = ReadIqTar("MyFile.iq.tar", ChannelToRead = 1)
-    ChannelToRead specifies the channel to be read. "0" reads all channels and returns a matrix."""
-    
+    ChannelToRead specifies the channel to be read. "0" reads all channels and returns a matrix.
+    BytesPerValue specifies the word length per I/Q sample in the file"""
+
     import tarfile
     import os
     import xml.etree.ElementTree as ET
     import logging
-    
-    filename = os.path.split(FileName)[1]
-    data=[]
+
+    data = []
     fs = 0
-        
+
     try:
-        tar = tarfile.open( FileName, "r:")
-        a=tar.getnames()
+        tar = tarfile.open(FileName, "r:")
+        a = tar.getnames()
         xmlfile = [filename for filename in a if ".xml" in filename.lower()]
         xmlfile = xmlfile[0]
         tar.extract(xmlfile)
         tree = ET.parse(xmlfile)
         root = tree.getroot()
         binaryfilename = root.find("DataFilename").text
         fs = float(root.find("Clock").text)
 
         helper = root.find("Samples")
         NumberOfSamples = 1
         if helper.text:
             NumberOfSamples = int(root.find("Samples").text)
-        
+
         helper = root.find("ScalingFactor")
         ScalingFactor = 1
         if helper.text:
             if helper.get("unit")!="V":
                 logging.warn("Only (V)olts scaling factor supported - assuming 1V!")
             else:
                 ScalingFactor = float(root.find("ScalingFactor").text)
 
         helper = root.find("NumberOfChannels")
         NumberOfChannels = 1
-        if helper != None:
+        if helper is not None:
             if helper.text:
                 NumberOfChannels = int(root.find("NumberOfChannels").text)
-                    
-        os.remove( xmlfile)
+
+        os.remove(xmlfile)
         del root
         tar.extract(binaryfilename)
         tar.close()
-        data = ReadIqw( binaryfilename)
-        os.remove( binaryfilename)
-        
+        data = ReadIqw(binaryfilename, BytesPerValue=BytesPerValue)
+        os.remove(binaryfilename)
+
     except:
-        logging.error("IqTar (" + FileName + ") read error!" )
-    
-    #Apply scaling factor
+        logging.error("IqTar (" + FileName + ") read error!")
+
+    # Apply scaling factor
     if ScalingFactor != 1:
         data = [sample * ScalingFactor for sample in data]
 
-    #separate channels
+    # separate channels
     if NumberOfChannels > 1:
-        
+
         if (ChannelToRead > NumberOfChannels):
             logging.warn("File " + FileName + " only contains " + str(NumberOfChannels) + " channels, using channel 1!")
             ChannelToRead = 1
         if ChannelToRead > 0:
             data1 = []
-            #for n in range(NumberOfSamples):
-                #data1.append( data[n*NumberOfChannels+ChannelToRead-1])
+            # for n in range(NumberOfSamples):
+            # data1.append( data[n*NumberOfChannels+ChannelToRead-1])
             data1 = data[ChannelToRead-1::NumberOfChannels]
         else:
             import numpy
-            data1 = numpy.empty((NumberOfSamples,NumberOfChannels),dtype = complex)
+            data1 = numpy.empty((NumberOfSamples, NumberOfChannels), dtype=complex)
             for n in range(NumberOfSamples):
                 for m in range(NumberOfChannels):
                     if m==0:
                         data1[n][m] = data[n*NumberOfChannels+m]
         data = data1
 
-    return data,fs
+    return data, fs
 
 
 
 def Iqw2Iqtar( FileName, fs, keepIqw = False, fCenterFrequency = 0):
     """Converts an iqw file into iq.tar. Suggested to use after directly reading
     binary data from instrument into file (iqw).
     Note: iqw must be in iqiqiq format
```

### Comparing `rskfd-0.3.8/rskfd/remote_control/instrument.py` & `rskfd-0.3.9/rskfd/remote_control/instrument.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/rskfd/remote_control/instrumentRS.py` & `rskfd-0.3.9/rskfd/remote_control/instrumentRS.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/rskfd/remote_control/instrumentRSExceptions.py` & `rskfd-0.3.9/rskfd/remote_control/instrumentRSExceptions.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/rskfd/remote_control/instrumentRS_FSW.py` & `rskfd-0.3.9/rskfd/remote_control/instrumentRS_FSW.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/rskfd/remote_control/instrumentRS_VSE.py` & `rskfd-0.3.9/rskfd/remote_control/instrumentRS_VSE.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/rskfd/signal_generation/signal_generation.py` & `rskfd-0.3.9/rskfd/signal_generation/signal_generation.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/rskfd/snp_handling/snpfiles.py` & `rskfd-0.3.9/rskfd/snp_handling/snpfiles.py`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/rskfd.egg-info/PKG-INFO` & `rskfd-0.3.9/rskfd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rskfd
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python Package for Instrument Control and Data Handling
 Home-page: https://gitlab.com/ramian/rskfd
 Download-URL: https://gitlab.com/ramian/rskfd/
 Author: Florian Ramian
 Author-email: gitlab@ramian.eu
 License: MIT
 Keywords: INSTRUMENT CONTROL,I/Q DATA,WV,IQ.TAR
```

### Comparing `rskfd-0.3.8/rskfd.egg-info/SOURCES.txt` & `rskfd-0.3.9/rskfd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rskfd-0.3.8/setup.py` & `rskfd-0.3.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   long_description = filein.read()
 
 setuptools.setup(
   name = 'rskfd',
   #packages = ['rskfd','rskfd.remote_control','rskfd.iq_data_handling','rskfd.signal_generation','rskfd.helper'],
   #packages = setuptools.find_packages(),
   packages = setuptools.find_namespace_packages(),
-  version = '0.3.8',
+  version = '0.3.9',
   license='MIT',
   description = 'Python Package for Instrument Control and Data Handling',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   author = 'Florian Ramian', 
   author_email = 'gitlab@ramian.eu',
   url = 'https://gitlab.com/ramian/rskfd',   # gitlab
```

