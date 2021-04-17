# WorldNews-UpVotes-Anomaly-Detection-LSTM
1. Dataset
  A large dataset (72.7 MB) of time-series news information published on Worldnews between 1/25/2008 and 11/22/2016, a peek on this dataset is shown below: ![data](Peek_on_data.jpg).
 There are 509236 rows and 8 columns which are "time_created", "date_created", "up_votes", "down_votes", "title", "over_18", "author", and "category". Note that in  "down_votes" column, the numbers are all zero and there is only one category which is Worldnews.
 
2. Motivation 
Given such dataset, an overall goal is to find any association between the large number of up votes and the types of news. Such information can serve as a guidence for inserting appropriate adds on the news pages. To do this, we can perform the following tasks step by step. 
* Exploring the yearly, monthly, and daily trends of the number of news and their corresponding up votes. 
* Using Machine Learning (ML) techniques to identify anomalies in the time-series up votes. 
* Perform Natural Language Processing (NLP) techniques on the "anomaly" news to extract the most frequent words in such news  
  
3. Technologies Used

 * Python
    - numpy
    - pandas
    - matplotlib
 * TensorFlow
 * Keras
 * Sklearn
 * NLTK

4. How to run the scripts
* Files
  -  `Eluvio_DS_Challenge.csv`
  -  `WorldNews_Anomaly_Detection_LSTM.ipynb`.
* Make sure the data file and the jupyter notebook in the same folder
* Open `WorldNews_Anomaly_Detection_LSTM.ipynb` and run it 
