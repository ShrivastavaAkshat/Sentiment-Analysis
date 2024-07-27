# Sentiment-Analysis
Using a dummy data of top 25 News of the day from financial market to train and predict a Model for overall Sentiment analysis

##Explaination
This Code performs sentiment analysis on financial market news. Here is a step-by-step explanation:

1 Import Libraries:

pandas is used for data manipulation and analysis.
numpy is used for numerical operations.
sklearn provides machine learning tools.

2 Import Dataset:

The financial market news dataset is read from a CSV file hosted on GitHub.

3 Explore Dataset:

df.head() displays the first few rows of the dataset.
df.info() provides information about the dataset, including column names, data types, and non-null values.
df.shape shows the number of rows and columns in the dataset.
df.columns lists the column names.

4 Feature Selection:

The code extracts the news text from the dataset and combines the text from columns 2 to 27 into a single string for each row.

5 Feature Text to Bag of Words:

CountVectorizer converts the news text into a numerical representation (bag of words) for machine learning.
fit_transform learns the vocabulary from the text and transforms the text into a matrix of word counts.

6 Target Variable:

The target variable y is extracted from the 'Label' column, representing the sentiment of the news.

7 Train Test Split:

train_test_split divides the dataset into training and testing sets to evaluate the model's performance.

8 Modeling:

RandomForestClassifier is a machine learning algorithm used for classification tasks.
The model is trained on the training data using rf.fit.

9 Prediction:

The trained model is used to predict the sentiment on the testing data using rf.predict.


10 Model Evaluation:

confusion_matrix and classification_report are used to assess the performance of the model.
accuracy_score calculates the overall accuracy of the model.

###In summary, the code trains a Random Forest Classifier to predict the sentiment of financial market news based on the text content. 
