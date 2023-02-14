### Persian Sentiment Analysis using XGBoost

![Farsi svg](https://user-images.githubusercontent.com/75095471/218720442-7f60dee8-5a9b-47fb-bb3e-58c81aa62d47.png)

70,000 comments with two labe

### About this Dataset
Snappfood (an online food delivery company) user comments containing 70,000 comments with two labels (i.e. polarity classification):Happy , Sad
Label	Number

<table>
<thead>
<tr>
<th>Label</th>
<th>Number</th>
</tr>
</thead>
<tbody>
<tr>
<td>Negative</td>
<td>35000</td>
</tr>
<tr>
<td>Positive</td>
<td>35000</td>
</tr>
</tbody>
</table>

This code provides a solution for sentiment analysis of comments from the online food delivery company Snappfood. The dataset contains 70,000 comments with two labels: positive and negative.

### Data Preprocessing

Read the dataset into a pandas dataframe.
Remove any English alphabet letters from the comments using the function "remove_fingilish".
Check that there are no mistakes in the labels.
Split the data into features (comments) and target (labels) for model training.

### Text Vectorization

Use the TfidfVectorizer from scikit-learn to convert the comments into a matrix of TF-IDF features.

### Resampling

Use the ClusterCentroids from the imblearn library to balance the class distribution in the training data.

### Model Training and Evaluation

Train an XGBoost classifier on the preprocessed and resampled data.
Evaluate the performance of the model using the classification report.
The code outputs the precision, recall, and f1-score for both the positive and negative classes.
