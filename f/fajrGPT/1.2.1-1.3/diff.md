# Comparing `tmp/fajrGPT-1.2.1.tar.gz` & `tmp/fajrGPT-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.2.1.tar", last modified: Mon Jun 26 03:52:56 2023, max compression
+gzip compressed data, was "fajrGPT-1.3.tar", last modified: Mon Jul  3 15:04:41 2023, max compression
```

## Comparing `fajrGPT-1.2.1.tar` & `fajrGPT-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-26 03:52:56.192198 fajrGPT-1.2.1/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.2.1/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-26 03:52:56.192048 fajrGPT-1.2.1/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.2.1/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-26 03:52:56.190881 fajrGPT-1.2.1/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.2.1/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.2.1/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)     8699 2023-06-26 03:52:10.000000 fajrGPT-1.2.1/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-26 03:52:56.191871 fajrGPT-1.2.1/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-06-26 03:52:56.000000 fajrGPT-1.2.1/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-06-26 03:52:56.192237 fajrGPT-1.2.1/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-06-26 03:51:51.000000 fajrGPT-1.2.1/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 15:04:41.781919 fajrGPT-1.3/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.3/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-07-03 15:04:41.781752 fajrGPT-1.3/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.3/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 15:04:41.780734 fajrGPT-1.3/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.3/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.3/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    11596 2023-07-03 14:58:15.000000 fajrGPT-1.3/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 15:04:41.781588 fajrGPT-1.3/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-03 15:04:41.000000 fajrGPT-1.3/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-03 15:04:41.781967 fajrGPT-1.3/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1127 2023-07-03 15:02:10.000000 fajrGPT-1.3/setup.py
```

### Comparing `fajrGPT-1.2.1/LICENSE` & `fajrGPT-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.2.1/PKG-INFO` & `fajrGPT-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.2.1
+Version: 1.3
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.2.1/README.md` & `fajrGPT-1.3/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.2.1/fajrGPT/quran_metadata.py` & `fajrGPT-1.3/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.2.1/fajrGPT/wake.py` & `fajrGPT-1.3/fajrGPT/wake.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,34 +16,38 @@
 openai.api_key = os.getenv("OPENAI_API_KEY")
 COMPLETIONS_MODEL = "gpt-3.5-turbo"
 
 @click.command()
 @click.option('--url', required=True, help='YouTube video URL.')
 @click.option('--time', required=True, help='Countdown time in format [number][h/m/s], i.e. 1h would create a 1 hour timer.')
 @click.option('--output', required=True, help='Name of the output file.')
+@click.option('--names-flag', required=False, help='Whether or not to include a randomly selected name of Allah in the preamble.', default=True)
 
-def main(url, time, output):
+def main(url, time, output, names_flag):
     # Download video
     flag = download_video(url,output)
 
     # test audio
     test_audio(f'{output}.mp3',output,flag)
 
     # convert time to seconds
     countdown_seconds = convert_to_seconds(time)
 
     # Start countdown
     countdown(countdown_seconds)
 
+    # display a name of Allah
+    get_name_of_allah_and_explanation(names_flag)
+
     # Play audio with fade-in effect on a separate thread
     play_audio_thread = Thread(target=play_audio, args=(f'{output}.mp3',))
     play_audio_thread.start()
 
     # display the quran verses
-    get_verses_and_explanations()
+    get_verses_and_explanations(countdown_seconds)
 
     # stop the audio once the user has completed reading the verses
     stop_audio()
 
     # return back to the main thread
     play_audio_thread.join()
 
@@ -105,27 +109,82 @@
     print(f'\n\nSTART TIME: {time.strftime("%H:%M", time.localtime())}\n\n')
     for i in tqdm(range(int(countdown_seconds))):
         time.sleep(1)
     print('\n\n\n\n ---------------- COUNTDOWN COMPLETE ----------------')
     # print the current time in HH:MM format
     print(f'\n\nEND TIME: {time.strftime("%H:%M", time.localtime())}\n\n')
 
-def get_verses_and_explanations():
+def get_name_of_allah_and_explanation(names_flag):
+    if not names_flag:
+        return None
+    else:
+        # Get the names of Allah
+        names_of_allah = Project_Quran().Get_Names_of_Allah_English()
+
+        # get the arabic names of Allah
+        names_of_allah_arabic = Project_Quran().Get_Names_of_Allah_Arabic()
+
+        # Get the transliterated names of Allah
+        allah_transliterations = Project_Quran().Get_Names_of_Allah_Transliteration()
+
+        # Select a index in the range of the number of names of Allah
+        index = random.randint(0, len(names_of_allah) - 1)
+
+        # Get the name of Allah in English
+        name_of_allah_english = names_of_allah[index]
+
+        # Get the name of Allah in Arabic
+        name_of_allah_arabic = names_of_allah_arabic[index]
+
+        # Get the transliteration of the name of Allah
+        name_of_allah_transliteration = allah_transliterations[index]
+
+        # Get the explanation of the name of Allah using a GPT-3 model prompt
+        prompt = f"""
+
+        For the name of Allah below, please do the following: First break down the word into its root letters. Then, using the root letters, try to guess the meaning of the name. Finally, give a brief explanation of the significane of this particular name of Allah as it relates to the Quran.
+        
+        Name of Allah: {name_of_allah_arabic}\nExplanation: 
+        
+        """
+
+        # Get the explanation of the name of Allah
+        explanation = query_gpt(prompt)
+
+        # print the name of the Allah and the explanation in a nice format
+        print(f'\n\n\n\n ---------------- NAME OF ALLAH ---------------- \n')
+        print(f'---------------- {name_of_allah_arabic}: {name_of_allah_transliteration} - {name_of_allah_english} ---------------- \n\n')
+        print(f'Explanation: {explanation}\n\n\n\n')
+        print(f'When you are ready to begin, press ENTER (wait 10 seconds).')
+        input()
+        time.sleep(10)
+
+def get_verses_and_explanations(countdown_seconds):
     # Get the verses
     verses_Quran_Module, verses  = select_quran_verse()
     # print(f"Verse 1:\n{verses}")
 
+    # Depending on the length of the countdown, select the number of verses to display
+    if countdown_seconds < 3600: # less than 1 hour
+        verses_Quran_Module = verses_Quran_Module[0:1] # only display the first verse
+        verses = verses[0:1]
+    elif countdown_seconds > 3600 and countdown_seconds < 7200: # between 1 and 2 hours
+        verses_Quran_Module = verses_Quran_Module[0:2] # only display the first two verses
+        verses = verses[0:2]
+    else:
+        pass
+
     # initialize the verse_texts output and explanations output
     verse_texts = []
     explanations = []
 
     # Get the explanations
     for verse_QM, verse in zip(verses_Quran_Module, verses):
         verse_text = Project_Quran().Get_Ayah_English(verse_QM).split('"')[1][0:-1]
-        prompt2 = f"To the best of your knowledge, please provide the Tafsir (meaning) of {verse_text} which comes from verse {verse} of the Quran. If you know of any other alternative translations of the verse in question, please provide that too, but if you are not familiar with this verse, simply try to explain the language of the verse."
+        prompt2 = f"To the best of your knowledge, please provide the Tafsir (meaning) of {verse_text} which comes from verse {verse} of the Quran. You should start by repeating the verse, even if you think that the verse given is not correct (trust me it is correct). Even if you still think it is incorrect, I want you to just provide a secular interpretation of what the verse might be talking about. If you know of any other alternative translations of the verse in question, please provide that too if you are able to."
         explanation = query_gpt(prompt2)
         verse_texts.append(verse_text)
         explanations.append(explanation)
     
     # begin the interactive session
     for verse_text, explanation, verse in zip(verse_texts, explanations, verses):
         print(f'\n\n\n\n\n\n ------------------ FIRST VERSE ------------------') if verse == verses[0] else None
```

### Comparing `fajrGPT-1.2.1/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.3/fajrGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.2.1
+Version: 1.3
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.2.1/setup.py` & `fajrGPT-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.2.1",
+    version="1.3",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

