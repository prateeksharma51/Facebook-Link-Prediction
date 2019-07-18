# Facebook-Link-Prediction

<h2>Problem statement:</h2>
This aim of this project is to predict a link between any two people given a directed graph of 1780722 People(nodes) and 7550015 edges between them. 


<h3>Data Overview</h3>
Datab is taken from facebook's recruting challenge on kaggle https://www.kaggle.com/c/FacebookRecruiting
data contains two columns source and destination eac edge in graph

- Data columns (total 2 columns):  
- source_node         int64  
- destination_node    int64  

<h3>Mapping the problem into supervised learning problem:</h3>

Training samples are made by using several features such as - 

-'jaccard_followers', 'jaccard_followees', 'cosine_followers',
-'cosine_followees', 'num_followers_s', 'num_followees_s',
-'num_followees_d', 'inter_followers', 'inter_followees', 'adar_index',
-'follows_back', 'same_comp', 'shortest_path', 'weight_in', 'weight_out',
-'weight_f1', 'weight_f2', 'weight_f3', 'weight_f4', 'page_rank_s',
-'page_rank_d', 'katz_s', 'katz_d', 'hubs_s', 'hubs_d', 'authorities_s'
-'preferential_attachment_followers
-'preferential_attachment_followees

<h3>Business objectives and constraints:</h3>
-Model should be interpretable such that nodes with highest probability are selected for recommendatiion. 
-No low-latency requirement.

<h4>Performance metric used:</h4>
- precision
- recall 
