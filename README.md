# Machine-Learning
Folder containing my Machine Learning Projects


For this final project, i decided to use a spam database, to create a model that detects spams. Everyone encounters spam way too much in their mail inboxes and i thought it would be interesting to try. You can access the dataset here : https://archive.ics.uci.edu/ml/machine-learning-databases/spambase/

Overview of the dataset
This dataset is composed of 58 columns and 4601 rows. Most column are corresponding to the frequece of the word into the email. We also have 3 columns concerning the capital run. The dataset is really clean, and all the values are numerical, so we dont't have to process them that much. Out of 4601 emails, 1813 of them are spams in this dataset.

I used multiple algorithms like Linear Regression, Random Forest, Naive Bayes, KNN, Decision Tree and a Deep Learning Algorithm.
After running all those algorithm we obtained those results:
*Here is a summary of the advantages and disadvantages of each algorithm, along with possible explanations for the differences in accuracy and a recommendation for what may work best for this particular problem:*


## Random Forest with 58 columns (Accuracy: 0.956)

Advantages: Random Forest is an ensemble method for improving predictive performance and reducing overfitting by combining multiple decision trees. It handles both categorical and continuous variables and works well with high-dimensional datasets. It can also provide feature importance rankings to identify the model's most important variables.

Disadvantages: Random Forest is a computationally intensive algorithm that may require hyperparameter tuning to achieve optimal performance. The model results can also be difficult to interpret.

Explanation for high accuracy: The high accuracy could be attributed to Random Forest's ability to handle high-dimensional data, which could be the case with the Spambase dataset. Furthermore, the method's ensemble nature can reduce overfitting and improve generalization to new data.


## Random Forest with 56 columns (Accuracy: 0.954)

Advantages: Same as above.

Disadvantages: Same as above.

Explanation for slightly lower accuracy: The removal of two columns may explain the difference in accuracy between this model and the previous one. It's possible that these two columns were crucial for prediction and that their removal resulted in a slight decrease in accuracy.

## Deep Learning Model (Accuracy: 0.940)

Advantages: Can learn complex patterns, extract features automatically, and handle high-dimensional and large-scale data.

Disadvantages: Requires large amounts of labeled data and computational resources to train, and can be challenging to interpret and explain.

Explanation for lower accuracy: I think that we don't have enough data to classify them. We only have 4500 emails, which is nothing. We could use a larger database with 100000+ emails inside.

## Linear Regression (Accuracy: 0.921)

Advantages: Linear Regression is a straightforward and understandable method for dealing with both continuous and categorical variables. It can also reveal relationships between the input variables and the target variable.

Disadvantages: Linear regression assumes a linear relationship between the input variables and the target variable, which is not always true in real-world data. It also does not handle variable interactions very well.

Explanation for lower accuracy: Linear Regression may be unable to capture the Spambase dataset's complex nonlinear relationships between input variables and target variables.

Recommendation: Because it achieves lower accuracy than Random Forest models, Linear Regression may not be the best choice for this problem.

## Decision Tree (Accuracy: 0.897)

Advantages: Decision Trees are basic and interpretable models that can handle both continuous and categorical inputs. They can also handle relationships between variables and can provide insights into the significant elements in the data.

Disadvantages: Decision Trees can easily overfit the training data and may not generalize well to new data. They are also sensitive to small changes in the data and can produce different results if the data is perturbed slightly.

Explanation for lower accuracy: The Decision Tree model may be overfitting the training data, leading to lower accuracy on the test data.

Recommendation: Decision Trees may not be the best choice for this problem, as they achieve lower accuracy than the Random Forest models and are more prone to overfitting.


## Naive Bayes (Accuracy: 0.829)

Advantages: Naive Bayes is a simple and fast method that can handle both continuous and categorical variables. It can also handle high-dimensional data well and can provide probabilistic predictions.

Disadvantages: Naive Bayes assumes that the input variables are independent, which may not be the case in real-world data. It can also suffer from the problem of overfitting
