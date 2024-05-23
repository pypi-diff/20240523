# Comparing `tmp/typing_test_sdd-1.0.3.tar.gz` & `tmp/typing_test_sdd-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_test_sdd-1.0.3.tar", last modified: Tue May 21 12:29:49 2024, max compression
+gzip compressed data, was "typing_test_sdd-1.0.4.tar", last modified: Thu May 23 14:05:42 2024, max compression
```

## Comparing `typing_test_sdd-1.0.3.tar` & `typing_test_sdd-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:29:49.317398 typing_test_sdd-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 12:29:43.000000 typing_test_sdd-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-21 12:29:49.317398 typing_test_sdd-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-21 12:29:43.000000 typing_test_sdd-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:29:49.317398 typing_test_sdd-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 12:29:43.000000 typing_test_sdd-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:29:49.317398 typing_test_sdd-1.0.3/typing_test_sdd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:29:49.317398 typing_test_sdd-1.0.3/typing_test_sdd/Assets/
--rw-r--r--   0 runner    (1001) docker     (127)    78455 2024-05-21 12:29:43.000000 typing_test_sdd-1.0.3/typing_test_sdd/Assets/main_image.png
--rw-r--r--   0 runner    (1001) docker     (127)    41028 2024-05-21 12:29:43.000000 typing_test_sdd-1.0.3/typing_test_sdd/Assets/polka.png
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 12:29:43.000000 typing_test_sdd-1.0.3/typing_test_sdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-05-21 12:29:43.000000 typing_test_sdd-1.0.3/typing_test_sdd/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    21222 2024-05-21 12:29:43.000000 typing_test_sdd-1.0.3/typing_test_sdd/words.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:29:49.317398 typing_test_sdd-1.0.3/typing_test_sdd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-21 12:29:49.000000 typing_test_sdd-1.0.3/typing_test_sdd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-21 12:29:49.000000 typing_test_sdd-1.0.3/typing_test_sdd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:29:49.000000 typing_test_sdd-1.0.3/typing_test_sdd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 12:29:49.000000 typing_test_sdd-1.0.3/typing_test_sdd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 12:29:49.000000 typing_test_sdd-1.0.3/typing_test_sdd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 12:29:49.000000 typing_test_sdd-1.0.3/typing_test_sdd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:05:42.067608 typing_test_sdd-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-23 14:05:42.067608 typing_test_sdd-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:05:42.067608 typing_test_sdd-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:05:42.063609 typing_test_sdd-1.0.4/typing_test_sdd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:05:42.067608 typing_test_sdd-1.0.4/typing_test_sdd/Assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    78455 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/typing_test_sdd/Assets/main_image.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41028 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/typing_test_sdd/Assets/polka.png
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/typing_test_sdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/typing_test_sdd/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21222 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/typing_test_sdd/words.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:05:42.067608 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/top_level.txt
```

### Comparing `typing_test_sdd-1.0.3/PKG-INFO` & `typing_test_sdd-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_test_sdd
-Version: 1.0.3
+Version: 1.0.4
 Summary: TKinter GUI Typing Test - Gaurav Surve 122SDD2
 Home-page: https://github.com/GauravS2507/Gaurav-Surve-SDD2-Project---Typing-Test
 Author: Gaurav Surve
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Education
@@ -39,14 +39,16 @@
     https://www.youtube.com/c/Codemycom
 - W3 Schools (JSON FILES, but also other things)
     https://www.w3schools.com/python/python_json.asp
 - Stack Overflow --> Helped to get general assistance for any bugs or issues I encountered. 
     https://stackoverflow.com/
 - Github --> Repository
     https://github.com/
-- CHATGPT was used to source words for my words.json list. This was the fastest way to source words for this project, and the only time any AI was used in the making of this task. 
+- CHATGPT was used to source words for my words.json list. This was the fastest way to source words for this project, and the only time any AI was used in the making of this task.
+
+SEE WIKI FOR ADDITIONAL INFORMATION/ASSISTANCE: https://github.com/GauravS2507/typing_test_sdd.wiki.git
 
 
 
 
 Thanks, 
 - Gaurav
```

### Comparing `typing_test_sdd-1.0.3/README.md` & `typing_test_sdd-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     https://www.youtube.com/c/Codemycom
 - W3 Schools (JSON FILES, but also other things)
     https://www.w3schools.com/python/python_json.asp
 - Stack Overflow --> Helped to get general assistance for any bugs or issues I encountered. 
     https://stackoverflow.com/
 - Github --> Repository
     https://github.com/
-- CHATGPT was used to source words for my words.json list. This was the fastest way to source words for this project, and the only time any AI was used in the making of this task. 
+- CHATGPT was used to source words for my words.json list. This was the fastest way to source words for this project, and the only time any AI was used in the making of this task.
+
+SEE WIKI FOR ADDITIONAL INFORMATION/ASSISTANCE: https://github.com/GauravS2507/typing_test_sdd.wiki.git
 
 
 
 
 Thanks, 
-- Gaurav
+- Gaurav
```

### Comparing `typing_test_sdd-1.0.3/setup.py` & `typing_test_sdd-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="typing_test_sdd",
-    version="1.0.3",
+    version="1.0.4",
     author="Gaurav Surve",
     url="https://github.com/GauravS2507/Gaurav-Surve-SDD2-Project---Typing-Test",
     description="TKinter GUI Typing Test - Gaurav Surve 122SDD2",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     platforms="any",
```

### Comparing `typing_test_sdd-1.0.3/typing_test_sdd/Assets/main_image.png` & `typing_test_sdd-1.0.4/typing_test_sdd/Assets/main_image.png`

 * *Files identical despite different names*

### Comparing `typing_test_sdd-1.0.3/typing_test_sdd/Assets/polka.png` & `typing_test_sdd-1.0.4/typing_test_sdd/Assets/polka.png`

 * *Files identical despite different names*

### Comparing `typing_test_sdd-1.0.3/typing_test_sdd/main.py` & `typing_test_sdd-1.0.4/typing_test_sdd/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,99 +5,99 @@
 import random
 from pathlib import Path
 import json
 from os import path
 
 
 # Initialize a variable to store the ID of the scheduled update
-timer_update_id = None
+timer_update_id = None #Boolean Variable to set whether the timer is meant to update or not
 
 
 # Defining Commands - Making Main Frame, All Widgets in 2nd Window, Each widget placed here will be represened in the main window
 def create_typing():
-    global current_word_label, container, typing_container, text_container, current_text, typing_box, container, timer_label, test_time, len_time, wpm_label, Textspeech, check_var, Back, Restart_button, timer_label, is_on_main_window, is_on_typing_window, scale
-    is_on_main_window = False
-    is_on_typing_window = True
+    global current_word_label, container, typing_container, text_container, current_text, typing_box, container, timer_label, test_time, len_time, wpm_label, Textspeech, check_var, Back, Restart_button, timer_label, is_on_main_window, is_on_typing_window, scale, modes
+    is_on_main_window = False #Boolean variable to show main window is not on, and now typing window keybinds wont work
+    is_on_typing_window = True #Boolean variable to show that typing window is on, and now Main window keybinds wont work
     
     # Clearing Frame
     for widget in main_window.winfo_children():  # Emptying out frame
         widget.place_forget()
     main_window.pack_forget()
 
-    root.geometry("1400x700")
+    root.geometry("1400x700") #Creating Typing window frame
     container = ctk.CTkFrame(root)
     container.pack(expand=True, fill="both")
     
-    typing_container = ctk.CTkFrame(container)
+    typing_container = ctk.CTkFrame(container) #First container that wholes everything else
     typing_container.place(
         relx=0.5, rely=0.5, relwidth=0.9, relheight=0.9, anchor="c"
     )
-    main_image = PIL.Image.open(Path(__file__).resolve().parents[0] / path.join("Assets", "main_image.png"))
+    main_image = PIL.Image.open(Path(__file__).resolve().parents[0] / path.join("Assets", "main_image.png")) #Image holder
     dummy_widget1 = ctk.CTkLabel(
         typing_container,
         text="",
         image=ctk.CTkImage(main_image, size=(1400, 700)),
     )
-    dummy_widget1.pack()
+    dummy_widget1.pack() #Frame that holds the words to type, and time left
     text_container = ctk.CTkFrame(
         typing_container, border_width=5, border_color="#767272"
     )
     text_container.place(
         relx=0.5, rely=0.05, relwidth=0.9, relheight=0.45, anchor="n"
     )
-    settings_container = ctk.CTkFrame(    
+    settings_container = ctk.CTkFrame(    #Container that holds settings functions + accesibility features
         typing_container, border_width=5, border_color="#767272", height=280
     )
     settings_container.place(relx=0.87, rely=0.75, anchor="c")
     # Label for the WPM counter
-    wpm_label = ctk.CTkLabel(
+    wpm_label = ctk.CTkLabel( #Label that displays the WPM of the user
         typing_container,
         text="WPM: ",
         corner_radius=100,
         fg_color="grey",
         text_color="black",
     )
     wpm_label.place(in_=typing_container, relx=0.1, rely=0.07)
 
-    Back = ctk.CTkButton(
+    Back = ctk.CTkButton( #Button to go back to Main window from the typing window
         container,
         text="← Go Back (Esc)",
         command=go_back,
         corner_radius=100,
         fg_color="white",
         text_color="black",
     )
     Back.place(relx=0.1)
 
-    current_word_label = ctk.CTkLabel(
+    current_word_label = ctk.CTkLabel( #Current word that the user has to type
         text_container,
         text=" ".join(sampled_words[0:3]),
         font=ctk.CTkFont(size=40),
     )
     current_word_label.place(relx=0.5, rely=0.5, anchor="c")
 
-    timer_label = ctk.CTkLabel(
+    timer_label = ctk.CTkLabel( #Timer label
         text_container, text=f"Time left: {timer_seconds} seconds"
     )
     timer_label.place(relx=0.5, rely=0.7, anchor="c")
 
-    current_text = ""
-    typing_box = ctk.CTkEntry(
+    current_text = "" #This variable stores what the user has typed into the entrybox and then later on checks whether the word is spelt correctly
+    typing_box = ctk.CTkEntry( #entrybox for the user to type in
         typing_container,
         placeholder_text="   Click Box To Begin",
         font=ctk.CTkFont(size=20),
     )
     typing_box.bind("<KeyRelease>", on_key_press)
     typing_box.place(
         relx=0.5, rely=0.91, anchor="c", relheigh=0.1, relwidth=0.3
     )
-    typing_box.focus()
+    typing_box.focus() #Focus ensures that the entrybox is already highlighted, and that the user does not need to click it
 
     # Options for Length of Time the Test is for
-    len_time = ctk.CTkOptionMenu(
+    len_time = ctk.CTkOptionMenu( 
         settings_container,
         values=["10", "30", "60"],
         command=test_time,
         button_color="black",
         fg_color="grey",
     )
     len_time.grid(column=0, row=1, pady=6, padx=10)
@@ -107,18 +107,18 @@
         text="Seconds",
         corner_radius=100,
         fg_color="grey",
         text_color="black",
     )
     len_time_label.grid(column=0, row=0, pady=8, padx=10)
 
-    modes = ctk.CTkOptionMenu(
+    modes = ctk.CTkOptionMenu( #Options for mode the user wants, system, dark or light
         settings_container,
         values=["dark", "light", "system"],
-        command=ctk.set_appearance_mode,
+        command= ctk.set_appearance_mode,
         button_color="black",
         fg_color="grey",
     )
     modes.grid(column=0, row=3, pady=6, padx=10)
     modes_label = ctk.CTkLabel(
         settings_container,
         text="Modes",
@@ -126,15 +126,15 @@
         fg_color="grey",
         text_color="black",
     )
     modes_label.grid(column=0, row=2, pady=6, padx=10)
     modes.set("system")
     modes.set(ctk.get_appearance_mode())
 
-    scale = ctk.CTkOptionMenu(
+    scale = ctk.CTkOptionMenu( #Options for the scale the user wants to use
         settings_container,
         values=["0.75", "1.0", "1.25"],
         command=scaling,
         button_color="black",
         fg_color="grey",
     )
     scale.grid(column=0, row=5, pady=8, padx=10)
@@ -143,44 +143,53 @@
         text="UI Scale",
         corner_radius=100,
         fg_color="grey",
         text_color="black",
     )
     scale_label.grid(column=0, row=4, pady=6, padx=10)
     scale.set(current_scaling)
-    
-
   
-    Restart_button = ctk.CTkButton(
+    Restart_button = ctk.CTkButton( #To restart the test
         typing_container,
         text="Restart (Enter)",
         command=restart,
         fg_color="grey",
         text_color="black",
     )
     Restart_button.place(relx=0.5, rely=0.80, anchor="c")
 
 
-def test_time(value):
+def test_time(value): #Function that updates the time left in the timer label
     global timer_seconds
     timer_label.configure(text=f"Time left: {str(value)} seconds")
     timer_seconds = int(value)
 
 
-def scaling(value):
+def scaling(value): #Function that sets the scale to what the user selects, Customtkinter function
     global current_scaling
     current_scaling = value
     ctk.set_widget_scaling(float(value))
 
 
 # Function that commands the Go Back Button
 def go_back():
+    global is_on_main_window, is_on_typing_window, timer_update_id, timer_seconds
+
+    # If leaving the typing window, stop the timer
+    if is_on_typing_window:
+        if timer_update_id:
+            root.after_cancel(timer_update_id)
+            timer_seconds = int(len_time.get())
+    
+    # Set window flags accordingly
+    is_on_main_window = True
+    is_on_typing_window = False
     container.pack_forget()  # Forget the current window
     root.geometry("1400x700")  # Adjust window size
-    make_main_window()  # Have to remake content who knows why!!!
+    make_main_window()  
     place_main_window_content()
 
 
 # Function that commands when the first word is written right
 def on_key_press(e):
     global score, sampled_words
     current_text = typing_box.get()
@@ -232,15 +241,15 @@
             root.after_cancel(timer_update_id)
         # Schedule the next update
         timer_update_id = root.after(1000, update_timer)
     else:
         timer_label.configure(text="Time's up!")
         value = int(len_time.get())
         if value == 10:
-            wpm_label.configure(text=f"WPM: {score * 6} ")
+            wpm_label.configure(text=f"WPM: {score * 6} ") #formula depending on the length of the test the user wants to run. 
 
         elif value == 30:
             wpm_label.configure(text=f"WPM: {score * 2} ")
         else:
             wpm_label.configure(text=f"WPM: {score} ")
         typing_box.configure(state="disable")
```

### Comparing `typing_test_sdd-1.0.3/typing_test_sdd/words.json` & `typing_test_sdd-1.0.4/typing_test_sdd/words.json`

 * *Files identical despite different names*

### Comparing `typing_test_sdd-1.0.3/typing_test_sdd.egg-info/PKG-INFO` & `typing_test_sdd-1.0.4/typing_test_sdd.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_test_sdd
-Version: 1.0.3
+Version: 1.0.4
 Summary: TKinter GUI Typing Test - Gaurav Surve 122SDD2
 Home-page: https://github.com/GauravS2507/Gaurav-Surve-SDD2-Project---Typing-Test
 Author: Gaurav Surve
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Education
@@ -39,14 +39,16 @@
     https://www.youtube.com/c/Codemycom
 - W3 Schools (JSON FILES, but also other things)
     https://www.w3schools.com/python/python_json.asp
 - Stack Overflow --> Helped to get general assistance for any bugs or issues I encountered. 
     https://stackoverflow.com/
 - Github --> Repository
     https://github.com/
-- CHATGPT was used to source words for my words.json list. This was the fastest way to source words for this project, and the only time any AI was used in the making of this task. 
+- CHATGPT was used to source words for my words.json list. This was the fastest way to source words for this project, and the only time any AI was used in the making of this task.
+
+SEE WIKI FOR ADDITIONAL INFORMATION/ASSISTANCE: https://github.com/GauravS2507/typing_test_sdd.wiki.git
 
 
 
 
 Thanks, 
 - Gaurav
```

