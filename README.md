# SMS-Spam-Classifier

The Problem of Spam

Unwanted email, commonly referred to as spam, disrupts daily communication and introduces security threats. Spam emails can contain malware designed to steal sensitive information, phishing attempts to trick users into revealing credentials, or fraudulent schemes.
Developing an automated system to identify and filter spam emails is crucial for improving user experience and protecting against these security risks.

Objective

This project's primary objective is to build a reliable spam detection model. By analyzing email content and metadata, the model will classify emails as either spam or legitimate ("ham").

Data Description

The system will utilize a dataset containing a collection of emails pre-labeled as spam or ham. Each email sample will be represented by features such as sender address, subject line, email body content, and potentially attachments. A balanced distribution of spam and ham emails ensures the model effectively learns to differentiate between the two classes.

Data Set: https://www.kaggle.com/datasets/jackksoncsie/spam-email-dataset

Data Wrangling:

Load the dataset containing the "text" and "label" columns.
Understanding the data
Handle any missing values or duplicates if present.

Exploratory Data Analysis (EDA):

Perform basic exploratory analysis to understand the characteristics of the email text data.
Visualize the distribution of spam and ham emails using histograms or pie charts.
Explore the length of emails (number of characters or words) in each category.
Identify common keywords or phrases in spam and ham emails through word frequency analysis.

Data Preprocessing:

Convert text data to lowercase to ensure uniformity.
Remove any special characters, punctuation, and digits from the text.
Tokenize the text data into individual words or tokens.
Remove stop words (commonly occurring words like "and", "the", "is") to reduce noise.
Perform stemming or lemmatization to reduce words to their base or root form.

Feature Engineering:

Convert the preprocessed text data into numerical features that can be used by machine learning algorithms
Explore feature representation techniques such as bag-of-words, TF-IDF (Term Frequency-Inverse Document Frequency).
Vectorize the text data using the chosen feature representation technique.

Splitting the Data:

Split the dataset into training, and test sets. Typically, you might use a 70-30 or 80-20 split.
Ensure that the distribution of spam and ham emails is consistent across the splits.

Model Building:

Choose appropriate machine learning algorithms for classification, such as:
Naive Bayes (e.g., Multinomial Naive Bayes)
Support Vector Machines (SVM)
Decision Trees
Random Forests

Model Evaluation:

Evaluate the final model on the test set to obtain unbiased performance metrics.

Result:

This analysis evaluated four classification models (Naive Bayes, Decision Tree, SVM, and Random Forest) for their performance on a binary classification task. All models achieved high Recall, with SVM achieving the highest (0.992) followed by Random Forest (0.946), Naive Bayes and Decision Tree (both at 0.926).

In terms of AUC (Area Under the ROC Curve), SVM again emerged as the leader (0.994), followed by Random Forest (0.973 ) and lastly, Decision Tree and lastly Naive Bayes (both at 0.949)

Conclusion:

Based on the evaluation results, SVM classification model appears to be the best performing model overall, achieving the highest accuracy and AUC. However, the differences in performance between the models are relatively small
