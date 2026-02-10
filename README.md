# NLU.Assignment01
Text classification of Indian news articles into Sports and Politics using traditional machine learning techniques and TF-IDF based features.
🔹 Problem Overview

The goal of this task is to build a machine learning based system that can automatically classify Indian news articles into two categories: Sports and Politics. The project focuses on understanding how traditional machine learning models work for text classification problems.

🔹 Data Collection

The dataset is collected from Kaggle, which is a reliable and widely used platform for public datasets. The data consists of Indian news articles from multiple domains. From this dataset, only Sports and Politics related articles are selected to keep the task simple and focused.

🔹 Dataset Description

Each data sample contains:

A label (SPORTS or POLITICS)

The corresponding news article text

The dataset is split into 80% training data and 20% testing data using stratified sampling to maintain class balance. The final test set contains 160 articles, equally divided between both classes.

🔹 Feature Representation

Different text feature extraction techniques are used:

Bag of Words (BoW): Counts word frequencies.

TF-IDF: Assigns higher weight to important words and lower weight to common words.

TF-IDF with n-grams: Uses unigrams and bigrams to capture small word phrases.

These features convert raw text into numerical form so that machine learning models can process it.

🔹 Machine Learning Models Used

Three traditional machine learning models are implemented:

Naive Bayes: A probabilistic model based on word probabilities.

Logistic Regression: A linear classifier that learns feature weights.

Linear Support Vector Machine (SVM): Finds an optimal separating boundary between classes.

🔹 Experimental Results

The models are evaluated using accuracy, precision, recall, and F1-score.

Model	Accuracy
Naive Bayes	78.75%
Logistic Regression	88.12%
Linear SVM	88.12%

Logistic Regression and Linear SVM improve accuracy by nearly 10% compared to Naive Bayes and show more balanced performance across both classes.

🔹 Limitations

The system works only on word-level features and does not understand deep context.

Sarcasm and mixed-topic articles are not handled well.

Classification is limited to only two categories.

Using n-grams increases computation and memory usage.

🔹 Conclusion

This project shows that traditional machine learning models combined with proper feature representation techniques can perform well for text classification tasks. Logistic Regression and Linear SVM achieved the best results with around 88% accuracy. The project highlights the importance of data preparation, feature selection, and proper evaluation in building effective NLP systems.
