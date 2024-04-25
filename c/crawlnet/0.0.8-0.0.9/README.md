# Comparing `tmp/crawlnet-0.0.8.tar.gz` & `tmp/crawlnet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlnet-0.0.8.tar", last modified: Thu Apr 25 16:30:21 2024, max compression
+gzip compressed data, was "crawlnet-0.0.9.tar", last modified: Thu Apr 25 18:36:48 2024, max compression
```

## Comparing `crawlnet-0.0.8.tar` & `crawlnet-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 16:30:21.435632 crawlnet-0.0.8/
--rw-rw-rw-   0        0        0     1005 2024-04-25 16:30:21.435632 crawlnet-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-04-25 16:29:54.000000 crawlnet-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 16:30:21.417296 crawlnet-0.0.8/crawlnet/
--rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.8/crawlnet/__init__.py
--rw-rw-rw-   0        0        0    24418 2024-04-25 15:37:33.000000 crawlnet-0.0.8/crawlnet/cl3.py
--rw-rw-rw-   0        0        0    31728 2024-04-25 16:27:31.000000 crawlnet-0.0.8/crawlnet/cl4.py
-drwxrwxrwx   0        0        0        0 2024-04-25 16:30:21.435632 crawlnet-0.0.8/crawlnet.egg-info/
--rw-rw-rw-   0        0        0     1005 2024-04-25 16:30:21.000000 crawlnet-0.0.8/crawlnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-25 16:30:21.000000 crawlnet-0.0.8/crawlnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 16:30:21.000000 crawlnet-0.0.8/crawlnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-25 16:30:21.000000 crawlnet-0.0.8/crawlnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 16:30:21.000000 crawlnet-0.0.8/crawlnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 16:30:21.435632 crawlnet-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-04-25 16:29:58.000000 crawlnet-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:36:48.686302 crawlnet-0.0.9/
+-rw-rw-rw-   0        0        0     1005 2024-04-25 18:36:48.662370 crawlnet-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-04-25 16:29:54.000000 crawlnet-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 18:36:48.633694 crawlnet-0.0.9/crawlnet/
+-rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.9/crawlnet/__init__.py
+-rw-rw-rw-   0        0        0    24418 2024-04-25 15:37:33.000000 crawlnet-0.0.9/crawlnet/cl3.py
+-rw-rw-rw-   0        0        0    29780 2024-04-25 18:36:14.000000 crawlnet-0.0.9/crawlnet/cl4.py
+drwxrwxrwx   0        0        0        0 2024-04-25 18:36:48.662370 crawlnet-0.0.9/crawlnet.egg-info/
+-rw-rw-rw-   0        0        0     1005 2024-04-25 18:36:48.000000 crawlnet-0.0.9/crawlnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-25 18:36:48.000000 crawlnet-0.0.9/crawlnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 18:36:48.000000 crawlnet-0.0.9/crawlnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-25 18:36:48.000000 crawlnet-0.0.9/crawlnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 18:36:48.000000 crawlnet-0.0.9/crawlnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 18:36:48.686749 crawlnet-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-04-25 18:35:08.000000 crawlnet-0.0.9/setup.py
```

### Comparing `crawlnet-0.0.8/PKG-INFO` & `crawlnet-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlnet
-Version: 0.0.8
+Version: 0.0.9
 Summary: CrawlNet
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: `!pip install crawlnet`
```

### Comparing `crawlnet-0.0.8/crawlnet/cl3.py` & `crawlnet-0.0.9/crawlnet/cl3.py`

 * *Files identical despite different names*

### Comparing `crawlnet-0.0.8/crawlnet/cl4.py` & `crawlnet-0.0.9/crawlnet/cl4.py`

 * *Files 9% similar despite different names*

```diff
@@ -336,120 +336,42 @@
 writer.append_data(image)
 display.Image(filename = anim_file)
 """
 
 sentiment_analysis = """
 !pip install tensorflow
 
-from tensorflow.keras.layers import SimpleRNN, LSTM, GRU, Bidirectional, Dense, Embedding
+import tensorflow as tf
 from tensorflow.keras.datasets import imdb
+from tensorflow.keras.preprocessing.sequence import pad_sequences
 from tensorflow.keras.models import Sequential
-import numpy as np
+from tensorflow.keras.layers import Embedding, SimpleRNN, Dense
+
+vocab_size = 10000  # Size of the vocabulary
+max_len = 500       # Maximum length of the review sequences
 
-# Getting reviews with words that come under 5000
-# most occurring words in the entire
-# corpus of textual review data
-vocab_size = 5000
+# Load the IMDB dataset
 (x_train, y_train), (x_test, y_test) = imdb.load_data(num_words=vocab_size)
 
-print(x_train[0])
-#These are the index values of the words and hence we done see any reviews 
+# Pad sequences to ensure uniform input size
+x_train = pad_sequences(x_train, maxlen=max_len)
+x_test = pad_sequences(x_test, maxlen=max_len)
+
+model = Sequential()
+model.add(Embedding(vocab_size, 32, input_length=max_len))
+model.add(SimpleRNN(32))  # Simple RNN layer with 32 units
+model.add(Dense(1, activation='sigmoid'))  # Output layer with sigmoid activation for binary classification
 
-# Getting all the words from word_index dictionary
-word_idx = imdb.get_word_index()
+model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])
+model.summary()
 
-# Originally the index number of a value and not a key,
-# hence converting the index as key and the words as values
-word_idx = {i: word for word, i in word_idx.items()}
-
-# again printing the review
-print([word_idx[i] for i in x_train[0]])
-
-# Get the minimum and the maximum length of reviews
-print("Max length of a review:: ", len(max((x_train+x_test), key=len)))
-print("Min length of a review:: ", len(min((x_train+x_test), key=len)))
-
-from tensorflow.keras.preprocessing import sequence
-
-# Keeping a fixed length of all reviews to max 400 words
-max_words = 400
-
-x_train = sequence.pad_sequences(x_train, maxlen=max_words)
-x_test = sequence.pad_sequences(x_test, maxlen=max_words)
-
-x_valid, y_valid = x_train[:64], y_train[:64]
-x_train_, y_train_ = x_train[64:], y_train[64:]
-
-# fixing every word's embedding size to be 32
-embd_len = 32
-
-# Creating a RNN model
-RNN_model = Sequential(name="Simple_RNN")
-RNN_model.add(Embedding(vocab_size,
-						embd_len,
-						input_length=max_words))
-
-# In case of a stacked(more than one layer of RNN)
-# use return_sequences=True
-RNN_model.add(SimpleRNN(128,
-						activation='tanh',
-						return_sequences=False))
-RNN_model.add(Dense(1, activation='sigmoid'))
-
-# printing model summary
-print(RNN_model.summary())
-
-# Compiling model
-RNN_model.compile(
-	loss="binary_crossentropy",
-	optimizer='adam',
-	metrics=['accuracy']
-)
-
-# Training the model
-history = RNN_model.fit(x_train_, y_train_,
-						batch_size=64,
-						epochs=5,
-						verbose=1,
-						validation_data=(x_valid, y_valid))
-
-# Printing model score on test data
-print()
-print("Simple_RNN Score---> ", RNN_model.evaluate(x_test, y_test, verbose=0))
-
-# Defining LSTM model
-lstm_model = Sequential(name="LSTM_Model")
-lstm_model.add(Embedding(vocab_size,
-						embd_len,
-						input_length=max_words))
-lstm_model.add(LSTM(128,
-					activation='relu',
-					return_sequences=False))
-lstm_model.add(Dense(1, activation='sigmoid'))
-
-# Printing Model Summary
-print(lstm_model.summary())
-
-# Compiling the model
-lstm_model.compile(
-	loss="binary_crossentropy",
-	optimizer='adam',
-	metrics=['accuracy']
-)
-
-# Training the model
-history3 = lstm_model.fit(x_train_, y_train_,
-						batch_size=64,
-						epochs=5,
-						verbose=2,
-						validation_data=(x_valid, y_valid))
-
-# Displaying the model accuracy on test data
-print()
-print("LSTM model Score---> ", lstm_model.evaluate(x_test, y_test, verbose=0))
+history = model.fit(x_train, y_train, epochs=5, batch_size=64, validation_split=0.2)
+
+test_loss, test_acc = model.evaluate(x_test, y_test)
+print(f'Test Accuracy: {test_acc}')
 """
 
 data_classification_algorithm = """
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from sklearn.linear_model import LogisticRegression
 from sklearn.datasets import load_iris
@@ -950,16 +872,15 @@
     "data_classification_algorithm": data_classification_algorithm,
     "data_clustering_algorithm": data_clustering_algorithm,
     "data_visualization_and_ETL": data_visualization_and_ETL,
     "import_data_and_load_in_target_system": import_data_and_load_in_target_system,
     "etl_in_sql_server":etl_in_sql_server,
     "map_reduce_to_generate_grades_of_students": map_reduce_to_generate_grades_of_students,
     "mapreduce_to_calculate_freq_of_given_word_in_file": mapreduce_to_calculate_freq_of_given_word_in_file,
-    "mapreduce_for_mat_multiplication":mapreduce_for_mat_multiplication
-    
+    "mapreduce_for_mat_multiplication": mapreduce_for_mat_multiplication
 }
 
 
 class Writer:
     def __init__(self, filename):
         self.filename = os.path.join(os.getcwd(), filename)
         self.masterDict = masterDict
```

### Comparing `crawlnet-0.0.8/crawlnet.egg-info/PKG-INFO` & `crawlnet-0.0.9/crawlnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlnet
-Version: 0.0.8
+Version: 0.0.9
 Summary: CrawlNet
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: `!pip install crawlnet`
```

### Comparing `crawlnet-0.0.8/setup.py` & `crawlnet-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "CrawlNet"
 
 # Setting up
 setup(
     name="crawlnet",
     version=VERSION,
     author="Hrushikesh Kachgunde",
```

