# Detect All Abuse! Toward Universal Abusive Language Detection Models
This repository contains code for paper [Detect All Abuse! Toward Universal Abusive Language Detection Models](https://www.aclweb.org/anthology/2020.coling-main.560/)

<h3 align="center">
  <b>Wang, K., Lu, D., Han, S. C., Long, S., & Poon, J. (2020) <br/><a href="https://www.aclweb.org/anthology/2020.coling-main.560/">Detect All Abuse! Toward Universal Abusive Language Detection Models</a><br/>In Proceedings of the 28th International Conference on Computational Linguistics 2020 (pp. 6366-6376)</b></span>
</h3>


<img src="https://usydnlpgroup.files.wordpress.com/2020/12/macas.png">


## Embeddings
### 1. Direct Abuse Embedding
The code is mainly from https://github.com/kamalkraj/Named-Entity-Recognition-with-Bidirectional-LSTM-CNNs
#### 1.1 Download Dataset For NER Model
Download 3 files from https://github.com/kamalkraj/Named-Entity-Recognition-with-Bidirectional-LSTM-CNNs/tree/master/data
>train.txt  
>test.txt  
>val.txt
#### 1.2 Download Glove embeddings
Download glove embeddings and unzip it: http://nlp.stanford.edu/data/glove.6B.zip
>glove.6B.100d.txt
#### 1.3 Train the Model and Make Prediction on the target Dataset
Please Note:
- Use [Direct Abuse Embedding](https://github.com/usydnlp/MACAS/blob/main/Directed%20Abuse%20Embedding.ipynb) to generate D embedding
- Change the MAX_LEN to the max length of your target dataset
- "sent_text" variable should be a list of original sentences
### 2. Generalized Abuse Embedding
Download the file from https://drive.google.com/file/d/152264axxTfmuYfb_7oWYQJFCggt06CEC/view?usp=sharing
### 3. Explicit Abuse Embedding
Download the file from https://drive.google.com/file/d/1059cRocqijTNzrl0UOXkFnngqpEZ54c1/view?usp=sharing
### 4. Implicit Abuse Embedding
#### 4.1 Generate Implicit Input
Use [Sarcasm Embedding Input](https://github.com/usydnlp/MACAS/blob/main/Generate%20Input%20for%20Sarcasm%20Model.ipynb) to generate Implicit Input
#### 4.2 Generate Implicit Embedding
After running [Sarcasm Embedding](https://github.com/usydnlp/MACAS/blob/main/Sarcasm_embedding.ipynb), copy and paste the embedding into a text file "sarcasm_embedding.txt"
### 5. User Linguistic Behavior Embedding
- Use [Linguistic Behavior](https://github.com/usydnlp/MACAS/blob/main/User%20Linguistic%20Behavior%20Embedding.ipynb) to get User Linguistic Behavior Embedding
- Change the sentences and raw labels 
## Final Model
- Use [Final Model](https://github.com/usydnlp/MACAS/blob/main/Final%20Model.ipynb) to do the final model training and prediction
- Use the target dataset to fill in the "sentence_list" and "label_list"
- Change the "seq_length" based on your choice
- Change the "use_gcn" based on whether you want to use User Linguistic Behavior Embedding 
