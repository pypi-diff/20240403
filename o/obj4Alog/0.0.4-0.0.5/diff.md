# Comparing `tmp/obj4Alog-0.0.4.tar.gz` & `tmp/obj4Alog-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obj4Alog-0.0.4.tar", last modified: Wed Mar 27 18:53:13 2024, max compression
+gzip compressed data, was "dist\obj4Alog-0.0.5.tar", last modified: Wed Apr  3 10:40:49 2024, max compression
```

## Comparing `obj4Alog-0.0.4.tar` & `obj4Alog-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 18:53:13.674460 obj4Alog-0.0.4/
--rw-rw-rw-   0        0        0      277 2024-03-27 18:53:13.666459 obj4Alog-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-27 18:53:13.624610 obj4Alog-0.0.4/obj4Alog/
--rw-rw-rw-   0        0        0       54 2024-03-27 18:45:04.000000 obj4Alog-0.0.4/obj4Alog/__init__.py
--rw-rw-rw-   0        0        0    16484 2024-03-27 18:19:12.000000 obj4Alog-0.0.4/obj4Alog/functions.py
-drwxrwxrwx   0        0        0        0 2024-03-27 18:53:13.666459 obj4Alog-0.0.4/obj4Alog.egg-info/
--rw-rw-rw-   0        0        0      277 2024-03-27 18:53:13.000000 obj4Alog-0.0.4/obj4Alog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-03-27 18:53:13.000000 obj4Alog-0.0.4/obj4Alog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 18:53:13.000000 obj4Alog-0.0.4/obj4Alog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-03-27 18:53:13.000000 obj4Alog-0.0.4/obj4Alog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-27 18:53:13.000000 obj4Alog-0.0.4/obj4Alog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 18:53:13.674460 obj4Alog-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      577 2024-03-27 18:17:53.000000 obj4Alog-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:40:49.424388 obj4Alog-0.0.5/
+-rw-rw-rw-   0        0        0      277 2024-04-03 10:40:49.423385 obj4Alog-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 10:40:49.368042 obj4Alog-0.0.5/obj4Alog/
+-rw-rw-rw-   0        0        0       54 2024-03-27 18:45:04.000000 obj4Alog-0.0.5/obj4Alog/__init__.py
+-rw-rw-rw-   0        0        0    27905 2024-04-03 09:56:19.000000 obj4Alog-0.0.5/obj4Alog/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:40:49.419386 obj4Alog-0.0.5/obj4Alog.egg-info/
+-rw-rw-rw-   0        0        0      277 2024-04-03 10:40:48.000000 obj4Alog-0.0.5/obj4Alog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-03 10:40:49.000000 obj4Alog-0.0.5/obj4Alog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 10:40:48.000000 obj4Alog-0.0.5/obj4Alog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-03 10:40:49.000000 obj4Alog-0.0.5/obj4Alog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-03 10:40:49.000000 obj4Alog-0.0.5/obj4Alog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 10:40:49.425384 obj4Alog-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      577 2024-04-03 10:40:12.000000 obj4Alog-0.0.5/setup.py
```

### Comparing `obj4Alog-0.0.4/obj4Alog/functions.py` & `obj4Alog-0.0.5/obj4Alog/functions.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 # ## import libraries
 
 # In[1]:
 
 
 import os
 import time
+import math
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from datetime import datetime
 import matplotlib.pyplot as plt
+from matplotlib.colors import LogNorm
+from datetime import datetime, timedelta
 
-from sklearn.cluster import DBSCAN
+from sklearn.cluster import DBSCAN, KMeans
 from sklearn.metrics import silhouette_score
+from sklearn.neighbors import NearestNeighbors, BallTree
 from sklearn.preprocessing import StandardScaler
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import pairwise_distances_argmin_min
 
 import pm4py
 from pm4py import read_xes
 from pm4py.algo.evaluation import algorithm
@@ -44,66 +47,84 @@
 
 # ## read dataset
 
 # In[3]:
 
 def hello():
     print('hello')
+
+
 def get_log_stats(log):
     # event log columns
-    all_columns = log.columns
     print("\nEvent log have total {} columns and {} log activities".format(log.shape[1], log.shape[0]))
     print("======================================================")
     
     print("\nEvent Log have the follwing columns:")
     print("====================================")
     print(list(log.columns))
     
+
 def read_log(xes_file_path):
     # Import the XES file as an event log
     event_log = read_xes(xes_file_path)
     return event_log
 
 
 # ## split log
 
 # In[4]:
 
 
 def split_log(log, test_size=0.30, shuffle=False):
     train_log, test_log = train_test_split(log, test_size=test_size, random_state=42, shuffle=shuffle)
+    # train_log = pm4py.objects.conversion.log.variants.df_to_event_log_1v.apply(train_log)
+    # test_log = pm4py.objects.conversion.log.variants.df_to_event_log_1v.apply(test_log)
     return train_log, test_log
 
 
 # ## train and evaluate Petri Net
 
 # In[5]:
 
 
 def train_evaluate_petri_net(training_log, testing_log):
     net, im, fm = pm4py.discover_petri_net_inductive(training_log, noise_threshold=0.2)
 
-    q_o = algorithm.apply(test_log, net, im, fm)
+    q_o = algorithm.apply(testing_log, net, im, fm)
 
     fitness = round(q_o['fitness']['average_trace_fitness'],3)
+
+    # log = pd.concat([training_log, testing_log])
+    q_o = algorithm.apply(training_log, net, im, fm)
     prec = round(q_o['precision'],3)
     gen = round(q_o['generalization'],3)
     simp = round(q_o['simplicity'],3)
     
     # fitness = pm4py.fitness_token_based_replay(testing_log, net, im, fm)
     # prec = pm4py.precision_token_based_replay(testing_log, net, im, fm)
     # gen = generalization_evaluator.apply(testing_log, net, im, fm)
     # simp = simplicity_evaluator.apply(net)
-    
+
+   
     print("\n========================")
     print("Fitness: ", fitness)
     print("Precision: ", prec)
     print("Generalization: ", gen)
     print("Simplicity: ", simp)
-    print("========================\n")
+    print("========================\n\n")
+
+    # fitness_alignments = pm4py.fitness_alignments(log, net, im, fm, activity_key='concept:name', case_id_key='case:concept:name', timestamp_key='time:timestamp')
+    # precision_alignments = pm4py.precision_alignments(log, net, im, fm, activity_key='concept:name', case_id_key='case:concept:name', timestamp_key='time:timestamp')
+  
+    # print("\n========================")
+    # print("Alignment Fitness: ", fitness_alignments)
+    # print("Alignment Precision: ", precision_alignments)
+    # print("Generalization: ", gen)
+    # print("Simplicity: ", simp)
+    # print("========================\n")
 
     return net, im, fm
 
 
 # ## save and plot models
 
 # In[6]:
@@ -165,18 +186,21 @@
 
     format_string = '%Y-%m-%d %H:%M:%S'
     event_log['time:timestamp'] = event_log['time:timestamp'].apply(lambda x : datetime.strptime(x, format_string))
 
     return event_log
     
 def create_session(log, session_duration):
-    log = log_preprocessing(log)
+    event_log = log_preprocessing(log)
     
     customers = list(event_log['case:concept:name'].unique())
-    session_df = pd.DataFrame(columns=['case:concept:name', 'lifecycle:transition','concept:name', 'time:timestamp',  'Session'])
+    if 'lifecycle:transition' in event_log.columns:
+        session_df = pd.DataFrame(columns=['case:concept:name', 'lifecycle:transition','concept:name', 'time:timestamp',  'Session'])
+    else:
+        session_df = pd.DataFrame(columns=['case:concept:name','concept:name', 'time:timestamp',  'Session'])
 
     for customer in customers:
         customer_trace = event_log[event_log['case:concept:name'] == customer]
         customer_trace = customer_trace.sort_values('time:timestamp')
         customer_trace['Session'] = (customer_trace['time:timestamp'] - 
                                      customer_trace['time:timestamp'].shift(1)).gt(pd.Timedelta(minutes=session_duration)).cumsum() + 1
         session_df = pd.concat([session_df, customer_trace], ignore_index=True)
@@ -192,49 +216,130 @@
 def freq_encoding(session_log):
     # Perform one-hot encoding
     one_hot_encoded = pd.get_dummies(session_log['concept:name'], prefix='activity')
     
     # Replace frequency with 1 where frequency is not 0
     one_hot_encoded = one_hot_encoded.applymap(lambda x: 1 if x > 0 else 0)
     
+    if 'lifecycle:transition' in session_log.columns:
+        df_encoded = pd.concat([session_log[['case:concept:name', 'lifecycle:transition', 'Session']], one_hot_encoded], axis=1)
+        df_grouped = df_encoded.groupby(['case:concept:name', 'lifecycle:transition', 'Session']).sum().reset_index()
+    else:
+        df_encoded = pd.concat([session_log[['case:concept:name', 'Session']], one_hot_encoded], axis=1)
+        df_grouped = df_encoded.groupby(['case:concept:name', 'Session']).sum().reset_index()
+
+    return df_grouped
+
+
+def calculate_time_spent(records):
+    time_spent_list = []
+    for i in range(len(records)-1):
+        current_record = records.iloc[i]
+        next_record = records.iloc[i+1]
+
+        current_time = current_record['time:timestamp']
+        next_time = next_record['time:timestamp']
+
+        if current_record['case:concept:name'] == next_record['case:concept:name'] and current_record['Session'] == next_record['Session']:
+            time_spent = next_time - current_time
+        else:
+            time_spent = timedelta(minutes=15)
+
+        time_spent_list.append(round(time_spent.total_seconds() / 60, 2))  # Convert to minutes
+
+    # Adding time spent for the last record (assuming the last record is not considered in the loop)
+    time_spent_list.append(15)
+
+    return time_spent_list
+
+def duration_encoding(session_log):
+    time_spent = calculate_time_spent(session_log)
+    session_log['duration'] = time_spent
+    
+    # Perform one-hot encoding
+    one_hot_encoded = pd.get_dummies(session_log['concept:name'], prefix='activity')
+    one_hot_encoded = one_hot_encoded.astype(float)
+    
     # Concatenate one-hot encoded columns with original DataFrame
-    df_encoded = pd.concat([session_log[['case:concept:name', 'lifecycle:transition', 'Session']], one_hot_encoded], axis=1)
+    if 'lifecycle:transition' in session_log.columns:
+        df_encoded = pd.concat([session_log[['case:concept:name', 'lifecycle:transition', 'Session']], one_hot_encoded], axis=1)
+    else:
+        df_encoded = pd.concat([session_log[['case:concept:name', 'Session']], one_hot_encoded], axis=1)
+
+    # Initialize new columns for each page name with default value 0
+    for page_name in df_encoded['concept:name'].unique():
+        df_encoded[page_name] = 0.0
+
+    # Fill the one-hot encoded columns with the corresponding duration values
+    for index, row in df_encoded.iterrows():
+        page_name_col = row["concept:name"]
+        df_encoded.at[index, page_name_col] = round(row['duration'], 2)
+
+    # Drop unnecessary columns
+    df_encoded = df_encoded.drop(['concept:name', 'duration'], axis=1)
     
     # Group by customer_id and session
     # df_encoded['time:timestamp'] = df_encoded['time:timestamp'].astype(str)
-    df_grouped = df_encoded.groupby(['case:concept:name', 'lifecycle:transition', 'Session']).sum().reset_index()
+    if 'lifecycle:transition' in session_log.columns:
+        df_grouped = df_encoded.groupby(['case:concept:name', 'lifecycle:transition', 'Session']).sum().reset_index()
+    else:
+        df_grouped = df_encoded.groupby(['case:concept:name', 'Session']).sum().reset_index()
 
     return df_grouped
 
-
 # ## Clustering
 
 # In[9]:
 
 
-def __clustering_preprocessing(endoded_log):
+def clustering_preprocessing(encoded_log):
     # Filter columns
-    activity_columns = [col for col in endoded_log.columns if col.startswith('activity_')]
+    activity_columns = [col for col in encoded_log.columns if col.startswith('activity_')]
     
     # Select only the columns that start with 'activity_'
     features = encoded_log[activity_columns]
 
     # Standardize features
     X = StandardScaler().fit_transform(features)
 
     # Convert the transformed ndarray back to a DataFrame
     # You need to retain the column names and index of your original DataFrame
     transformed_df = pd.DataFrame(X, columns=features.columns, index=features.index)
 
     return transformed_df
-    
+
 
 def elbow_clustering(encoded_log):
+    features_log = clustering_preprocessing(encoded_log)
+    
+    # Compute K-Means for different values of k
+    k_values = range(3, 21)  # Adjust the range of k as needed
+    silhouette_scores = []
+    
+    for k in k_values:
+        kmeans = KMeans(n_clusters=k)
+        labels = kmeans.fit_predict(features_log)
+        silhouette_scores.append(silhouette_score(features_log, labels))
+    
+    # Find the optimal k using the elbow method
+    plt.plot(k_values, silhouette_scores, 'bx-')
+    plt.xlabel('Number of Clusters (k)')
+    plt.ylabel('Silhouette Score')
+    plt.title('Elbow Method For Optimal k')
+    plt.show()
+    
+    # Choose the best k based on the elbow point
+    optimal_k = k_values[np.argmax(silhouette_scores)]
+    print("Optimal number of clusters (k) based on the elbow method:", optimal_k)   
+
+    return optimal_k
 
-    features_log = __clustering_preprocessing(encoded_log)
+def estimate_eps(encoded_log):
+
+    features_log = clustering_preprocessing(encoded_log)
     
     # Compute DBSCAN
     eps_values = np.linspace(0.1, 3.0, num=20)
     silhouette_scores = []
     
     for eps in eps_values:
         dbscan = DBSCAN(eps=eps)
@@ -246,17 +351,38 @@
     plt.xlabel('Eps')
     plt.ylabel('Silhouette Score')
     plt.title('DBSCAN Elbow Method')
     plt.grid(True)
     plt.show()
 
 
+def KMeans_Clusteirng(encoded_log, k=2):
+
+    features_log = clustering_preprocessing(encoded_log)
+
+    # Apply DBSCAN clustering
+    kmeans_model = KMeans(n_clusters=k)  
+    encoded_log['KMeans_Cluster'] = kmeans_model.fit_predict(features_log)
+
+    labels = kmeans_model.labels_
+
+    # Number of clusters in labels, ignoring noise if present.
+    n_clusters_ = len(set(labels)) - (1 if -1 in labels else 0)
+    n_noise_ = list(labels).count(-1)
+    
+    print('\nEstimated number of clusters: %d' % n_clusters_)
+    print('Estimated number of noise points: %d' % n_noise_)
+    
+    print("\n", encoded_log['KMeans_Cluster'].value_counts(), "\n")
+
+    return encoded_log
+
 def DBSACN_Clusteirng(encoded_log, epsilon_value=2, minimum_samples=12):
 
-    features_log = __clustering_preprocessing(encoded_log)
+    features_log = clustering_preprocessing(encoded_log)
 
     # Apply DBSCAN clustering
     dbscan_model = DBSCAN(eps=epsilon_value, min_samples=minimum_samples)  # Adjust eps and min_samples based on your data
     encoded_log['DBSCAN_Cluster'] = dbscan_model.fit_predict(features_log)
 
     labels = dbscan_model.labels_
 
@@ -272,77 +398,167 @@
     return encoded_log
 
 def remove_noise_samples(encoded_log):
     # Assuming features_df is a DataFrame containing the feature vectors and DBSCAN_Cluster column
     # Reset the index to ensure proper alignment of indices
     # encoded_log = encoded_log.reset_index(drop=True)
 
-    features_log = __clustering_preprocessing(encoded_log)
-    features_log['DBSCAN_Cluster'] = encoded_log['DBSCAN_Cluster']
+    features_log = clustering_preprocessing(encoded_log)
+    if 'DBSCAN_Cluster' in encoded_log.columns:
+        cluster_column = 'DBSCAN_Cluster'
+    else:
+        cluster_column = 'KMeans_Cluster'
+
+    features_log[cluster_column] = encoded_log[cluster_column]
     
     # Find noise indices
-    noise_indices = encoded_log[encoded_log['DBSCAN_Cluster'] == -1].index
+    noise_indices = encoded_log[encoded_log[cluster_column] == -1].index
+
+    if len(noise_indices) >= 1:
     
-    # Find the nearest cluster for each noise point
-    nearest_cluster_indices, _ = pairwise_distances_argmin_min(
-        features_log.iloc[noise_indices, :-1],  # Exclude the cluster label column
-        features_log[features_log['DBSCAN_Cluster'] != -1].iloc[:, :-1]  # Exclude noise points
-    )
-    
-    # Merge noise samples into the nearest cluster
-    encoded_log.loc[noise_indices, 'DBSCAN_Cluster'] = encoded_log.loc[
-        encoded_log['DBSCAN_Cluster'] != -1, 'DBSCAN_Cluster'
-    ].iloc[nearest_cluster_indices].values
-    
-    # Check if there are still noise points
-    remaining_noise_indices = encoded_log[encoded_log['DBSCAN_Cluster'] == -1].index
-    if len(remaining_noise_indices) > 0:
-        print(f"T\nhere are still {len(remaining_noise_indices)} noise points remaining.\n")
-    else:
-        print("\nAll noise points have been assigned to the nearest cluster.\n")
+        # Find the nearest cluster for each noise point
+        nearest_cluster_indices, _ = pairwise_distances_argmin_min(
+            features_log.iloc[noise_indices, :-1],  # Exclude the cluster label column
+            features_log[features_log[cluster_column] != -1].iloc[:, :-1]  # Exclude noise points
+        )
+        
+        # Merge noise samples into the nearest cluster
+        encoded_log.loc[noise_indices, cluster_column] = encoded_log.loc[
+            encoded_log[cluster_column] != -1, cluster_column
+        ].iloc[nearest_cluster_indices].values
+        
+        # Check if there are still noise points
+        remaining_noise_indices = encoded_log[encoded_log[cluster_column] == -1].index
+        if len(remaining_noise_indices) > 0:
+            print(f"T\nhere are still {len(remaining_noise_indices)} noise points remaining.\n")
+        else:
+            print("\nAll noise points have been assigned to the nearest cluster.\n")
 
-    print("\n", encoded_log['DBSCAN_Cluster'].value_counts(), "\n")
+        print("\n", encoded_log[cluster_column].value_counts(), "\n")
     return encoded_log
 
 
 # ## Plotting
 
 # In[10]:
 
 
-def plot_heatmap(encoded_log):
+def plot_heatmap2(encoded_log, largest_activities=20, mode="linear"):
+    if 'DBSCAN_Cluster' in encoded_log.columns:
+        cluster_column = 'DBSCAN_Cluster'
+    else:
+        cluster_column = 'KMeans_Cluster'
+
+    features_log = clustering_preprocessing(encoded_log)
+    features_log[cluster_column] = encoded_log[cluster_column]
+    features_df = features_log
+    
+    # Filter numeric columns for plotting
+    numeric_features = features_df.select_dtypes(include='number')
+    
+    # Calculate mean of each feature within each cluster
+    cluster_means = numeric_features.groupby(cluster_column).mean().T
+    
+    # Calculate correlation matrix
+    correlation_matrix = cluster_means.corr()
+    
+    # Filter top correlated features for each cluster from all features
+    top_correlated_columns = {}
+    for cluster_label in correlation_matrix.columns:
+        top_correlated_columns[cluster_label] = correlation_matrix[cluster_label].nlargest(largest_activities).index.tolist()
+    
+    # Create a DataFrame containing only the top correlated columns for each cluster
+    cluster_means_top_correlated = pd.DataFrame()
+    for cluster_label, columns in top_correlated_columns.items():
+        cluster_means_top_correlated[cluster_label] = cluster_means[columns].idxmax()
+    
+    # Plot heatmap
+    plt.figure(figsize=(10, 6))
+    fig, ax = plt.subplots()
+    
+    if mode == "linear":
+        sns.heatmap(cluster_means_top_correlated, cmap="YlOrRd", annot=True, fmt="", cbar=False, linewidths=.5, xticklabels=True, yticklabels=True, ax=ax)
+    else:
+        sns.heatmap(cluster_means_top_correlated, cmap="YlOrRd", annot=True, fmt="", cbar=False, linewidths=.5, norm=LogNorm(), xticklabels=True, yticklabels=True, ax=ax)
+    
+    plt.title('Heatmap of Top {} Most Correlated Columns with Each Feature'.format(largest_activities))
+    plt.xlabel('Cluster')
+    plt.ylabel('Feature')
+    plt.show()
+    
+    # Return the most correlated feature names for each cluster
+    most_correlated_features = {}
+    for cluster_label, columns in top_correlated_columns.items():
+        most_correlated_features[cluster_label] = numeric_features.columns[cluster_means[columns].idxmax()]
+    
+    return most_correlated_features
+
+
+def plot_heatmap(encoded_log, largest_activities=20, mode="linear"):
+    if 'DBSCAN_Cluster' in encoded_log.columns:
+        cluster_column = 'DBSCAN_Cluster'
+    else:
+        cluster_column = 'KMeans_Cluster'
 
-    features_log = __clustering_preprocessing(encoded_log)
-    features_log['DBSCAN_Cluster'] = encoded_log['DBSCAN_Cluster']
+    features_log = clustering_preprocessing(encoded_log)
+    features_log[cluster_column] = encoded_log[cluster_column]
     features_df = features_log
     
     # Calculate mean of each feature within each cluster
-    cluster_means = (features_df.groupby('DBSCAN_Cluster').mean()).T
+    cluster_means = (features_df.groupby(cluster_column).mean()).T
     
     # Calculate correlation matrix
     correlation_matrix = cluster_means.corr()
     
+
     # Select top 10 most correlated columns for each cluster
     top_correlated_columns = {}
     for cluster_label in correlation_matrix.columns:
-        top_correlated_columns[cluster_label] = correlation_matrix[cluster_label].nlargest(20).index.tolist()
+        top_correlated_columns[cluster_label] = correlation_matrix[cluster_label].nlargest(largest_activities).index.tolist()
     
     # Create a DataFrame containing only the top 10 most correlated columns for each cluster
     cluster_means_top_correlated = pd.DataFrame()
     for cluster_label, columns in top_correlated_columns.items():
         cluster_means_top_correlated[cluster_label] = cluster_means[cluster_label][columns]
     
     # Plot heatmap
     plt.figure(figsize=(10, 6))
-    sns.heatmap(cluster_means_top_correlated, annot=True, cmap="hot", fmt=".2f", facecolor='white')
-    plt.title('Heatmap of Top 10 Most Correlated Columns with Each Feature')
+    fig, ax = plt.subplots()
+    logmin = 0.001
+    # sns.heatmap(cluster_means_top_correlated, annot=True, cmap="hot", fmt=".2f", facecolor='white')
+    if mode == "linear":
+        sns.heatmap(cluster_means_top_correlated, cmap="YlOrRd", linewidths=.5,xticklabels=True, yticklabels= True, ax = ax)
+    else:
+        sns.heatmap(cluster_means_top_correlated, cmap="YlOrRd", linewidths=.5,norm =LogNorm(), xticklabels=True, yticklabels= True, ax= ax)
+    
+    plt.title('Heatmap of Top {} Most Correlated Columns with Each Feature')
     plt.xlabel('Cluster')
     plt.ylabel('Feature')
     plt.show()
 
+    cluster_map = {}
+    for col in cluster_means_top_correlated.columns:
+        sorted_values = cluster_means_top_correlated[col].sort_values(ascending=False)
+        highest_value = sorted_values.iloc[0]
+        highest_index = sorted_values.index[0]
+        # second_highest_value = sorted_values.iloc[1]
+        # second_highest_index = sorted_values.index[1]
+        # cluster_map[col] = {
+        #     'highest_value': highest_value,
+        #     'highest_index': highest_index,
+        #     'second_highest_value': second_highest_value,
+        #     'second_highest_index': second_highest_index
+        # }
+
+        cluster_map[col] = highest_index
+    
+    activity_dict_no_activity = {k: v.replace('activity_', '') for k, v in cluster_map.items()}
+
+    return activity_dict_no_activity
+ 
 
 # ## Abstract Model
 
 # In[11]:
 
 
 # Define a function to label the activities as 'start' and 'end'
@@ -355,21 +571,26 @@
         return pd.concat([group, pd.DataFrame([new_activity])], ignore_index=True)
     else:
         group.loc[group.index[0], 'Activity_Status'] = 'start'
         group.loc[group.index[-1], 'Activity_Status'] = 'end'
         return group
 
 def abstract_log_preprocessing(session_log, cluster_log, cluster_map):
+    if 'DBSCAN_Cluster' in cluster_log.columns:
+        cluster_column = 'DBSCAN_Cluster'
+    else:
+        cluster_column = 'KMeans_Cluster'
+
     # Perform inner join
     merged_log = pd.merge(session_log, cluster_log, on=['case:concept:name', 'Session', 'lifecycle:transition'], how='inner')
     
-    merged_log = merged_log[['case:concept:name', 'Session', 'lifecycle:transition', 'time:timestamp', 'concept:name', 'DBSCAN_Cluster']]
+    merged_log = merged_log[['case:concept:name', 'Session', 'lifecycle:transition', 'time:timestamp', 'concept:name', cluster_column]]
     
-    merged_log['DBSCAN_Cluster'] = merged_log['DBSCAN_Cluster'].replace(cluster_map)
-    merged_log.rename({'concept:name':'log_activity', 'DBSCAN_Cluster':'abstract_activity'}, axis=1, inplace=True)
+    merged_log[cluster_column] = merged_log[cluster_column].replace(cluster_map)
+    merged_log.rename({'concept:name':'log_activity', cluster_column:'abstract_activity'}, axis=1, inplace=True)
 
     merged_log = merged_log.sort_values(by=['case:concept:name', 'Session', 'time:timestamp'])
     
     # Group the DataFrame by 'CustomerID' and 'Session', then apply the function
     new_df = merged_log.groupby(['case:concept:name', 'Session']).apply(__label_activity).reset_index(drop=True)
     
     # Select only the 'start' and 'end' activities
@@ -455,7 +676,82 @@
     print("Fitness: ", fitness)
     print("Precision: ", prec)
     print("Generalization: ", gen)
     print("Simplicity: ", simp)
     print("========================\n")
 
     return a_net, a_im, a_fm
+
+
+def distance (center, enc):
+    difference = np.diff([center,enc], axis = 0)
+    return np.sqrt(np.sum(np.power(difference,2)))
+
+
+def epsEstimate (enc,imgpath=""):
+    enc = clustering_preprocessing(enc)
+
+    enc = enc.values.tolist()
+    nbrs = NearestNeighbors(n_neighbors=2, algorithm='auto').fit(enc)
+    _,indices = nbrs.kneighbors(enc)
+    eps_dist = []
+    for i,e in enumerate(enc): 
+        eps_dist.append(distance(e,enc[indices[i][-1]]))
+    eps_dist.sort()
+    
+    tot = len(eps_dist)
+    fig,ax1 = plt.subplots(figsize=(10,5))
+    hist, bins, _ = ax1.hist(eps_dist[:-math.floor(tot/5)],bins= 50)
+    perc = [0 for i in bins]
+
+    cumsum = np.cumsum(hist)
+    percent = (cumsum / tot) * 100
+    
+    # Find the knee of the curve where the percentage plateaus
+    knee_index = np.argmax(np.gradient(percent))
+    best_eps = bins[knee_index]
+
+    for i,v in enumerate(bins):
+        for e in eps_dist:
+            if e<v:
+                perc[i]+=1
+    for i,_ in enumerate(perc):
+        perc[i] = (perc[i]/tot)*100
+    ax1.set_xticks(bins)
+    ax1.xaxis.set_tick_params(rotation=90)
+    ax1.set_title("Eps Estimate ")
+    ax1.set_ylabel('n')
+    ax1.set_xlabel('Eps')
+    ax2 = ax1.twinx()
+    ax2.plot(bins,perc,color= 'red')
+    ax2.set_yticks(np.linspace(0,100,num = 11))
+    ax2.set_ylabel('percentage')
+    ax1.grid(color= 'C0',alpha = 0.5)
+    ax2.grid(color= 'red',alpha = 0.5)
+    ax2.hlines(50,xmin=min(bins),xmax = max(bins),linestyle = 'dashed',color = 'k')
+    ax2.tick_params(axis='y', colors='red')
+    ax1.tick_params(axis='y', colors='C0')
+    fig.tight_layout()
+    fig.savefig("epsEstimate.png")
+    fig.clear()
+
+    return best_eps
+
+
+def minPointsEstimate (enc, eps, imgpath=""):
+    enc = clustering_preprocessing(enc)
+    tree = BallTree(np.array(enc))
+    allNgbr = []
+    allNgbr.append(tree.query_radius(enc, eps, count_only=True))
+    _, bins, _ = plt.hist (allNgbr, bins = 45)
+    plt.grid(axis='y', alpha=0.75)
+    plt.xticks(bins, rotation = 90 )
+    plt.title("MinPts Estimate")
+    plt.ylabel('Number of sessions')
+    plt.xlabel('Number of neighbors')
+    plt.tight_layout()
+    plt.savefig("minptsEstimate.png")
+    plt.close()
+
+    # Determine the best value for min_samples
+    min_samples = int(np.ceil(np.mean(allNgbr)))
+    return min_samples
```

### Comparing `obj4Alog-0.0.4/setup.py` & `obj4Alog-0.0.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="obj4Alog",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     install_requires=[
     'matplotlib==3.6.3',
     'numpy>=1.21.1',
     'pandas>=2.0.3',
     'pm4py>=2.7.1',
     'scikit_learn==1.3.2',
```

