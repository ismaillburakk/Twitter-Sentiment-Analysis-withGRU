# Intorduction
This report examines a Python code performing Twitter sentiment analysis using a GRU 
(Gated Recurrent Unit) neural network and K-Means Clustering method. Utilizing text 
data gathered from Kaggle Tweet Sentiment Analysis dataset( https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis ), this code trains and tests 
a model to determine the sentiment labels of the text data.

# Data Loading and Preprocessing
- Loading of training and testing data.
- Addition of column headers for the datasets.
- Removal of unnecessary columns.
- Cleaning of missing and duplicate data.
- Text data preprocessing: Removal of URLs, usernames, emoticons, special 
characters, and repeated letters. Additionally, text is converted to lowercase and 
lemmatized.

# Data Preparation
- Segregation of text data and labels.
- Conversion of text data to numerical format using Tokenizer and Pad Sequences, 
followed by splitting into training and testing sets.

# GRU Model
- Creation of a model incorporating Embedding, Bidirectional GRU, and Dense 
layers.
- Compilation of the model using Categorical Crossentropy.
- Label Encoder and One-Hot Encoding utilized for fitting the data.
- Training of the model and evaluation on the validation set.
- Training accuracy of the model 0.9684
- Validation accuracy of the model 0.9043
![image](https://github.com/ismaillburakk/Twitter-Sentiment-Analysis-withGRU/assets/75124682/f56948de-a741-4b53-8033-3a7d0e322aa6)

# Results
- Visualization of accuracy and loss values during training and validation 
processes.
![image](https://github.com/ismaillburakk/Twitter-Sentiment-Analysis-withGRU/assets/75124682/7dc8e7bb-a3f4-4c22-9dfd-e732ac08c0f3)
- Display of loss and accuracy values of the model on the test data.
- Confusion matrix showcasing how the model predicts different sentiment 
classes.
![image](https://github.com/ismaillburakk/Twitter-Sentiment-Analysis-withGRU/assets/75124682/a5ad19b4-8a6b-430a-b06e-41f4ac957ef7)

# K-Means Clustering
- Conversion of text data to numerical representation using TF-IDF.
- Application of K-Means clustering with a specified number of clusters.
- Assignment of cluster labels to each data point.
- Addition of cluster labels to the sentiment dataframe.
- Display of the count of data points in each cluster.
- Exploration of the characteristics of each cluster, showcasing a sample of text 
data in each cluster.
- SSE = 67268

# Conclusion
This Python code provides an effective means to perform sentiment analysis on Twitter 
texts. The model has successfully determined the sentiment labels of the texts in the 
dataset. However, further steps such as gathering more data or tuning the model's 
hyperparameters could be considered to enhance the model's performance.




