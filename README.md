# MACAS

The code is for [Detect All Abuse! Toward Universal Abusive Language Detection Models](https://arxiv.org/abs/2010.03776)

# Embeddings
## 1. Direct Abuse Embedding
The code is mainly from https://github.com/kamalkraj/Named-Entity-Recognition-with-Bidirectional-LSTM-CNNs
### 1.1 Download Dataset For NER Model
Download 3 files from https://github.com/kamalkraj/Named-Entity-Recognition-with-Bidirectional-LSTM-CNNs/tree/master/data
>train.txt  
>test.txt  
>val.txt
### 1.2 Download Glove embeddings
Download glove embeddings and unzip it: http://nlp.stanford.edu/data/glove.6B.zip
>glove.6B.100d.txt
### 1.3 Train the Model and Make Prediction on the target Dataset
Please Note:
- Use xxxxxxxx to generate D embedding
- Change the MAX_LEN to the max length of your target dataset
- "sent_text" variable should be a list of original sentences
## 2. Generalized Abuse Embedding
Download the file from https://drive.google.com/file/d/152264axxTfmuYfb_7oWYQJFCggt06CEC/view?usp=sharing
## 3. Explicit Abuse Embedding
Download the file from https://drive.google.com/file/d/1059cRocqijTNzrl0UOXkFnngqpEZ54c1/view?usp=sharing
## 4. Implicit Abuse Embedding
### 4.1 Generate Implicit Input
Use xxx to generate Implicit Input
### 4.2 Generate Implicit Embedding
After running, copy and paste the embedding into a text file "sarcasm_embedding.txt"
## 5. User Linguistic Behavior Embedding
- Use xxxx to get User Linguistic Behavior Embedding
- Change the sentences and raw labels 
# Final Model
- Use xxx to do the final model training and prediction
- Use the target dataset to fill in the "sentence_list" and "label_list"
- Change the "seq_length" based on your choice
- Change the "use_gcn" based on whether you want to use User Linguistic Behavior Embedding
