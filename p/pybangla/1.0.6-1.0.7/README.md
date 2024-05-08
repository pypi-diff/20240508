# Comparing `tmp/pybangla-1.0.6.tar.gz` & `tmp/pybangla-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-1.0.6.tar", last modified: Tue May  7 16:45:20 2024, max compression
+gzip compressed data, was "pybangla-1.0.7.tar", last modified: Wed May  8 20:31:56 2024, max compression
```

## Comparing `pybangla-1.0.6.tar` & `pybangla-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:20.975363 pybangla-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:17.000000 pybangla-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-07 16:45:20.975363 pybangla-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-05-07 16:45:17.000000 pybangla-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:20.971363 pybangla-1.0.6/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 16:45:17.000000 pybangla-1.0.6/pybangla/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:20.975363 pybangla-1.0.6/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:17.000000 pybangla-1.0.6/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-05-07 16:45:17.000000 pybangla-1.0.6/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-07 16:45:17.000000 pybangla-1.0.6/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-07 16:45:17.000000 pybangla-1.0.6/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-07 16:45:17.000000 pybangla-1.0.6/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    19396 2024-05-07 16:45:17.000000 pybangla-1.0.6/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-07 16:45:17.000000 pybangla-1.0.6/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-07 16:45:17.000000 pybangla-1.0.6/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:20.975363 pybangla-1.0.6/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-07 16:45:20.000000 pybangla-1.0.6/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-07 16:45:20.000000 pybangla-1.0.6/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:45:20.000000 pybangla-1.0.6/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 16:45:20.000000 pybangla-1.0.6/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 16:45:20.000000 pybangla-1.0.6/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:45:20.975363 pybangla-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-07 16:45:17.000000 pybangla-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:20.975363 pybangla-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-07 16:45:17.000000 pybangla-1.0.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:56.322170 pybangla-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:52.000000 pybangla-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-08 20:31:56.322170 pybangla-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-05-08 20:31:52.000000 pybangla-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:56.322170 pybangla-1.0.7/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:56.322170 pybangla-1.0.7/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20038 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-05-08 20:31:52.000000 pybangla-1.0.7/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:56.322170 pybangla-1.0.7/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-05-08 20:31:56.000000 pybangla-1.0.7/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 20:31:56.000000 pybangla-1.0.7/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:31:56.000000 pybangla-1.0.7/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 20:31:56.000000 pybangla-1.0.7/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 20:31:56.000000 pybangla-1.0.7/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:31:56.322170 pybangla-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-08 20:31:52.000000 pybangla-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:31:56.322170 pybangla-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-08 20:31:52.000000 pybangla-1.0.7/tests/test.py
```

### Comparing `pybangla-1.0.6/PKG-INFO` & `pybangla-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.6
+Version: 1.0.7
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.0.6/README.md` & `pybangla-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.6/pybangla/module/config.py` & `pybangla-1.0.7/pybangla/module/config.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.6/pybangla/module/date_extractor.py` & `pybangla-1.0.7/pybangla/module/date_extractor.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.6/pybangla/module/main.py` & `pybangla-1.0.7/pybangla/module/main.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.6/pybangla/module/number_parser.py` & `pybangla-1.0.7/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.6/pybangla/module/parser.py` & `pybangla-1.0.7/pybangla/module/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,35 +226,44 @@
             else:
                 n_n+=i
                 
         s_m = n_n.split(".")
         before_dot_word, after_dot_word = self.number_to_words(s_m[0]), self.digit_number_to_digit_word(s_m[1], language=language)
         word =  before_dot_word+" দশমিক "+after_dot_word
         return word
+    def check_comma_dot_dari(self,  p):
+        l_p = [",", ".", "।"]
+        if p in l_p:
+            return True
+        return False
     
     def number_processing(self, text):
         pattern = r'[\d,\.]+'
         matches = re.findall(pattern, text)
         for n in matches:
-            status = self.contains_only_english(n)
-            m_re = n.replace(",", "")
-            if status:
-                if "." in m_re:
-                    bn_m= self.fraction_number_conversion(m_re)
-                else:
-                    bn_m= self.number_to_words(self._digit_converter(m_re))
-                
-                text = text.replace(n, bn_m)
+            p_status = self.check_comma_dot_dari(n)
+
+            if p_status:
+                text = text.replace(n, n+" ")
             else:
-                if "." in m_re:
-                    bn_m= self.fraction_number_conversion(m_re, language="bn")
+                status = self.contains_only_english(n)
+                m_re = n.replace(",", "")
+                if status:
+                    if "." in m_re:
+                        bn_m= self.fraction_number_conversion(m_re)
+                    else:
+                        bn_m= self.number_to_words(self._digit_converter(m_re))
+                    
+                    text = text.replace(n, bn_m)
                 else:
-                    bn_m= self.number_to_words(m_re)
-                # print(n, m_re, bn_m)
-                text = text.replace(n, bn_m)
+                    if "." in m_re:
+                        bn_m= self.fraction_number_conversion(m_re, language="bn")
+                    else:
+                        bn_m= self.number_to_words(m_re)
+                    text = text.replace(n, bn_m)
 
         return text
 
 class DateParser:
     def __init__(self):
         self.samples = cfg.samples
 
@@ -394,14 +403,21 @@
         self.currency_pattern = r'(?:\$|£|৳|€|¥|₹|₽|₺)?(?:\d+(?:,\d{3})*(?:\.\d+)?|\d+(?:\.\d+)?)'
         self.npr = NumberParser()
         self.dp = DateParser() 
 
     def collapse_whitespace(self, text):
         return re.sub(_whitespace_re, " ", text)
     
+    def unwanted_puntuation_removing(self, text):
+        unwanted_symbols = ["-", "_", ":", "[", "]", "(", ")", "{", "}", "^", "~"]
+        pattern = "[" + re.escape("".join(unwanted_symbols)) + "]"
+        text = re.sub(pattern, " ", text)
+        return text
+
+    
     def expand_symbols(self, text, lang="bn"):
         for regex, replacement in _symbols[lang]:
             # print("regex : ", regex)
             text = re.sub(regex, replacement, text)
             text = text.replace("  ", " ")  # Ensure there are no double spaces
         return text.strip()
 
@@ -484,35 +500,37 @@
                 return True
         return False
 
 
     
     def replance_date_processing(self, text):
         dates = dt.get_dates(text)
+        # print()
         for date in dates:
             status = True
             if " " in date:
                 status = self.date_formate_validation(date)
             if status:
                 position = self.npr.find_word_index(text, date)
                 formated_date = self.dp.date_processing(date)
                 f_d_string = formated_date["txt_date"]+" "+formated_date["month"]+" "+formated_date["txt_year"]
                 text = self.npr.replace_text_at_position(text, f_d_string, position[0], position[1])
         return text
 
     
 
     def processing(self, text):
-        text = self.collapse_whitespace(text)
+        text = self.unwanted_puntuation_removing(text)
         text = self.expand_symbols(text)
         text = self.expand_abbreviations(text)
         text = self.expand_position(text)
         text = self.extract_currency_amounts(text)
         text = self.replance_date_processing(text)
         text = self.npr.number_processing(text)
+        text = self.collapse_whitespace(text)
         return text
     
 if __name__ =="__main__":
 
     text = "রাহিম ক্লাস ওয়ান এ ১ম, ১১তম ২২ তম ৩৩ তম, ১২৩৪ শতাব্দীতে ¥২০৩০.১২৩৪ বিবিধ  বাকেরগঞ্জ উপজেলার প্রায় 40 ভাগের পেশাই চাষাবাদ 80 and 40 ২২"
     tp = TextParser()
     text = tp.processing(text)
```

### Comparing `pybangla-1.0.6/pybangla/module/word_to_number.py` & `pybangla-1.0.7/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.6/pybangla/test.py` & `pybangla-1.0.7/pybangla/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import time
 from module.main import Normalizer
 
 if __name__ == "__main__":
 
 
     # # Testing Date format
-    date_list = [
-        "সেপ্টেম্বর ০৫ ২০২৩",
-        "এপ্রিল ২০২৩" 
-        "2023-04-05",  
-        "06-04-2023", 
-        "04/01/2023",  
-        "07 April, 2023", 
-        "Apr 1, 2023",  
-        "2023/04/01", 
-        "01-Apr-2023", 
-        "01-Apr/2023",  
-        "20230401",  
-        "20042024",
-        ["1", "4", "2025"]
-    ]
-    # # # number = "123456" or "২০২৩"
-    # number = "২০২৩"
+    # date_list = [
+    #     "সেপ্টেম্বর ০৫ ২০২৩",
+    #     "এপ্রিল ২০২৩" 
+    #     "2023-04-05",  
+    #     "06-04-2023", 
+    #     "04/01/2023",  
+    #     "07 April, 2023", 
+    #     "Apr 1, 2023",  
+    #     "2023/04/01", 
+    #     "01-Apr-2023", 
+    #     "01-Apr/2023",  
+    #     "20230401",  
+    #     "20042024",
+    #     ["1", "4", "2025"]
+    # ]
+    # # # # number = "123456" or "২০২৩"
+    # # number = "২০২৩"
     nrml = Normalizer()
-    # # print("++++++++++++++++++++ Date testing ++++++++++++++++++++++")
-    # print("Date format Testing : ", end ="", flush=True)
-    for date_ in date_list:
-        start_time = time.time()
-        formated_date = nrml.date_format(date_, language="bn")
-        print(formated_date)
-    print("++++++++++++++++++++ end of Date testing ++++++++++++++++++++++")
+    # # # print("++++++++++++++++++++ Date testing ++++++++++++++++++++++")
+    # # print("Date format Testing : ", end ="", flush=True)
+    # for date_ in date_list:
+    #     start_time = time.time()
+    #     formated_date = nrml.date_format(date_, language="bn")
+    #     print(formated_date)
+    # print("++++++++++++++++++++ end of Date testing ++++++++++++++++++++++")
 
     # print("++++++++++++++++++++ en number to bn number convert ++++++++++++++++++++++")
     # number = nrml.number_convert(number, language="bn")
     
     
     # number = nrml.number_convert(number, language="bn")
 
@@ -74,104 +74,108 @@
 
     # text = "রাহিম ক্লাস ওয়ান এ ১ম, ১১তম ২২ তম ৩৩ তম, ১২৩৪ শতাব্দীতে ¥২০৩০.১২৩৪ বিবিধ  বাকেরগঞ্জ উপজেলার প্রায় 40 ভাগের পেশাই চাষাবাদ 80 and 40 ২২"
     
     # text = nrml.text_normalizer(text)
 
     # print(text)
 
-    input_texts = [
-        "আমি এক দুই তিন চার পাঁচ টু থ্রি ফাইভ ছয় সেভেন এইট নাইন শূন্য আমার ফোন নাম্বার জিরো ওয়ান ডাবল সেভেন",
-        "ওয়ান ডাবল নাইন টু",
-        "একশ বিশ টাকা",
-        "জিরো টু ডাবল ওয়ান",
-        "জিরো ওয়ান ডাবল সেভেন থ্রি ডাবল ফাইভ নাইন থ্রি সেভেন নাইন",
-        "আমার ফোন নম্বর জিরো ওয়ান ডাবল সেভেন থ্রি ডাবল ফাইভ নাইন থ্রি সেভেন নাইন",
-        "ট্রিপল টু ওয়ান",
-        "দুই হাজার চারশো বিশ",
-        "দুই হাজার চারশ  বিশ",
-        "হাজার বিশ",
-        "ডাবল নাইন টু",
-        "এক লক্ষ চার হাজার দুইশ",
-        "এক লক্ষ চার হাজার দুইশ এক",
-        "এক লক্ষ চার হাজার দুইশ এক টাকা এক দুই",
-        "আমাকে এক লক্ষ দুই হাজার টাকা দেয়",
-        "আমাকে এক লক্ষ দুই হাজার এক টাকা দেয় এন্ড তুমি বিশ হাজার টাকা নিও এন্ড এক লক্ষ চার হাজার দুইশ এক টাকা এক ডবল দুই",
-        "ছয় হাজার বিশ",
-        "আমার সাড়ে পাঁচ হাজার",
-        "আমার সাড়ে তিনশ",
-        "আড়াই হাজার",
-        "আড়াই লক্ষ",
-        "ডেরশ",
-        "আমাকে ডেরশ টাকা দেয়",
-        "সাড়ে পাঁচ কোটি টাকা",
-        "সাড়ে 1254 টাকা",
-        "জিরো",
-        "একশ বিশ take একশ",
-        "জিরো টু ডাবল ওয়ান",
-        "জিরো টু ওয়ান ওয়ান",
-        "থ্রি ফোর ফাইভ এইট",
-        "একশ বিশ টাকা",
-        "ডাবল ওয়ান ডবল টু",
-        "জিরো ওয়ান টু",
-        "থ্রি ফোর ফাইভ সিক্স",
-        "সেভেন এইট নাইন টেন",
-        "একশ দুইশ তিনশ",
-        "চারশ পাঁচশ",
-        "ছয়শ সাতশ",
-        "আটশ নয়শ",
-        "দশ তিরানব্বই",
-        "ট্রিপল থ্রি টু",
-        "শূন্য এক দুই তিন",
-        "চার পাঁচ ছয় সাত",
-        "আট নয় দশ এগারো",
-        "বারো তেরো চৌদ্দ পনেরো",
-        "ষোল সতেরো আঠারো উনিশ",
-        "বিশ একুশ বাইশ তেইশ",
-        "চব্বিশ পঁচিশ ছাব্বিশ সাতাশ",
-        "আঠাশ ঊনত্রিশ ত্রিশ একত্রিশ",
-        "বত্রিশ তেত্রিশ চৌত্রিশ পঁয়ত্রিশ",
-        "ছত্রিশ সাঁইত্রিশ আটত্রিশ ঊনচল্লিশ",
-        "চল্লিশ একচল্লিশ বিয়াল্লিশ তেতাল্লিশ",
-        "চুয়াল্লিশ পঁয়তাল্লিশ ছেচল্লিশ সাতচল্লিশ",
-        "আটচল্লিশ ঊনপঞ্চাশ পঞ্চাশ একান্ন",
-        "বাহান্ন তিপ্পান্ন চুয়ান্ন পঞ্চান্ন",
-        "ছাপ্পান্ন সাতান্ন আটান্ন ঊনষাট",
-        "ষাট একষট্টি বাষট্টি তেষট্টি",
-        "চৌষট্টি পঁয়ষট্টি ছেষট্টি সাতষট্টি",
-        "আটষট্টি ঊনসত্তর সত্তর একাত্তর",
-        "বাহাত্তর তিয়াত্তর চুয়াত্তর পঁচাত্তর",
-        "ছিয়াত্তর সাতাত্তর আটাত্তর ঊনআশি",
-        "আশি একাশি বিরাশি তিরাশি",
-        "চুরাশি পঁচাশি ছিয়াশি সাতাশি",
-        "আটাশি ঊননব্বই নব্বই একানব্বই",
-        "বিরানব্বই তিরানব্বই চুরানব্বই পঁচানব্বই",
-        "ছিয়ানব্বই সাতানব্বই আটানব্বই নিরানব্বই",
-        "এক লক্ষ চার হাজার দুইশ এক টাকা এক দুই",
-        "তিনশ পঁচিশ পাঁচশ",
-        "তিনশ পঁচিশ পাঁচশ এক",
-        "চা-পুন",
-        "ওকে",
-        "ডের আউটস্ট্যান্ডিং কত",
-        "ডাবল",
-        "নাইন ডাবল এইট",
-        "দশ বারো এ এগুলা একশ একশ দুই",
-        "এক লক্ষ তেত্রিশ চার"
-        ]
-    for i in input_texts:
-        print("="*40)
-        print("input : ", i)
-        text = nrml.word2number(i)
-        print("output : ", text)
-        print("="*40)
-    text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২,০২৩"
-    formated_date = nrml.date_extraction(text)
+    # input_texts = [
+    #     "আমি এক দুই তিন চার পাঁচ টু থ্রি ফাইভ ছয় সেভেন এইট নাইন শূন্য আমার ফোন নাম্বার জিরো ওয়ান ডাবল সেভেন",
+    #     "ওয়ান ডাবল নাইন টু",
+    #     "একশ বিশ টাকা",
+    #     "জিরো টু ডাবল ওয়ান",
+    #     "জিরো ওয়ান ডাবল সেভেন থ্রি ডাবল ফাইভ নাইন থ্রি সেভেন নাইন",
+    #     "আমার ফোন নম্বর জিরো ওয়ান ডাবল সেভেন থ্রি ডাবল ফাইভ নাইন থ্রি সেভেন নাইন",
+    #     "ট্রিপল টু ওয়ান",
+    #     "দুই হাজার চারশো বিশ",
+    #     "দুই হাজার চারশ  বিশ",
+    #     "হাজার বিশ",
+    #     "ডাবল নাইন টু",
+    #     "এক লক্ষ চার হাজার দুইশ",
+    #     "এক লক্ষ চার হাজার দুইশ এক",
+    #     "এক লক্ষ চার হাজার দুইশ এক টাকা এক দুই",
+    #     "আমাকে এক লক্ষ দুই হাজার টাকা দেয়",
+    #     "আমাকে এক লক্ষ দুই হাজার এক টাকা দেয় এন্ড তুমি বিশ হাজার টাকা নিও এন্ড এক লক্ষ চার হাজার দুইশ এক টাকা এক ডবল দুই",
+    #     "ছয় হাজার বিশ",
+    #     "আমার সাড়ে পাঁচ হাজার",
+    #     "আমার সাড়ে তিনশ",
+    #     "আড়াই হাজার",
+    #     "আড়াই লক্ষ",
+    #     "ডেরশ",
+    #     "আমাকে ডেরশ টাকা দেয়",
+    #     "সাড়ে পাঁচ কোটি টাকা",
+    #     "সাড়ে 1254 টাকা",
+    #     "জিরো",
+    #     "একশ বিশ take একশ",
+    #     "জিরো টু ডাবল ওয়ান",
+    #     "জিরো টু ওয়ান ওয়ান",
+    #     "থ্রি ফোর ফাইভ এইট",
+    #     "একশ বিশ টাকা",
+    #     "ডাবল ওয়ান ডবল টু",
+    #     "জিরো ওয়ান টু",
+    #     "থ্রি ফোর ফাইভ সিক্স",
+    #     "সেভেন এইট নাইন টেন",
+    #     "একশ দুইশ তিনশ",
+    #     "চারশ পাঁচশ",
+    #     "ছয়শ সাতশ",
+    #     "আটশ নয়শ",
+    #     "দশ তিরানব্বই",
+    #     "ট্রিপল থ্রি টু",
+    #     "শূন্য এক দুই তিন",
+    #     "চার পাঁচ ছয় সাত",
+    #     "আট নয় দশ এগারো",
+    #     "বারো তেরো চৌদ্দ পনেরো",
+    #     "ষোল সতেরো আঠারো উনিশ",
+    #     "বিশ একুশ বাইশ তেইশ",
+    #     "চব্বিশ পঁচিশ ছাব্বিশ সাতাশ",
+    #     "আঠাশ ঊনত্রিশ ত্রিশ একত্রিশ",
+    #     "বত্রিশ তেত্রিশ চৌত্রিশ পঁয়ত্রিশ",
+    #     "ছত্রিশ সাঁইত্রিশ আটত্রিশ ঊনচল্লিশ",
+    #     "চল্লিশ একচল্লিশ বিয়াল্লিশ তেতাল্লিশ",
+    #     "চুয়াল্লিশ পঁয়তাল্লিশ ছেচল্লিশ সাতচল্লিশ",
+    #     "আটচল্লিশ ঊনপঞ্চাশ পঞ্চাশ একান্ন",
+    #     "বাহান্ন তিপ্পান্ন চুয়ান্ন পঞ্চান্ন",
+    #     "ছাপ্পান্ন সাতান্ন আটান্ন ঊনষাট",
+    #     "ষাট একষট্টি বাষট্টি তেষট্টি",
+    #     "চৌষট্টি পঁয়ষট্টি ছেষট্টি সাতষট্টি",
+    #     "আটষট্টি ঊনসত্তর সত্তর একাত্তর",
+    #     "বাহাত্তর তিয়াত্তর চুয়াত্তর পঁচাত্তর",
+    #     "ছিয়াত্তর সাতাত্তর আটাত্তর ঊনআশি",
+    #     "আশি একাশি বিরাশি তিরাশি",
+    #     "চুরাশি পঁচাশি ছিয়াশি সাতাশি",
+    #     "আটাশি ঊননব্বই নব্বই একানব্বই",
+    #     "বিরানব্বই তিরানব্বই চুরানব্বই পঁচানব্বই",
+    #     "ছিয়ানব্বই সাতানব্বই আটানব্বই নিরানব্বই",
+    #     "এক লক্ষ চার হাজার দুইশ এক টাকা এক দুই",
+    #     "তিনশ পঁচিশ পাঁচশ",
+    #     "তিনশ পঁচিশ পাঁচশ এক",
+    #     "চা-পুন",
+    #     "ওকে",
+    #     "ডের আউটস্ট্যান্ডিং কত",
+    #     "ডাবল",
+    #     "নাইন ডাবল এইট",
+    #     "দশ বারো এ এগুলা একশ একশ দুই",
+    #     "এক লক্ষ তেত্রিশ চার"
+    #     ]
+    # for i in input_texts:
+    #     print("="*40)
+    #     print("input : ", i)
+    #     text = nrml.word2number(i)
+    #     print("output : ", text)
+    #     print("="*40)
+    # text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২,০২৩"
+    # formated_date = nrml.date_extraction(text)
 
-    print(formated_date)
+    # print(formated_date)
 
     # text = "৫ বছরে নন-ক্যাডার পদে ৭,৪৪৭ জনকে নিয়োগের সুপারিশ করা হয়েছে 1,230"
     text = "৫ বছরে নন-ক্যাডার পদে ৭,৪৪৭ জনকে নিয়োগের সুপারিশ করা হয়েছে"
 
+    # text = "শীঘ্রই ভিক্টোরিয়ার এক প্রতিনিধিদল আসছেন,শিলংয়ের ব্রুকসাইড হাউসে"
+
     # text = "The numbers are 10 নন-ক্যাডার 20.5  30, and 40.75. সুপারিশ ২০৩০.৩০ 12 23 45"
+    # text = "This_is-a:test~sentence^with{some}unwanted[symbols]"
 
+    print("input : ", text)
     text = nrml.text_normalizer(text)
-    print(text)
+    print("output : ", text)
```

### Comparing `pybangla-1.0.6/pybangla.egg-info/PKG-INFO` & `pybangla-1.0.7/pybangla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.6
+Version: 1.0.7
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.0.6/setup.py` & `pybangla-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-1.0.6/tests/test.py` & `pybangla-1.0.7/tests/test.py`

 * *Files identical despite different names*

