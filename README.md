## Movie Genre Classification

This Python script performs movie genre classification using machine learning techniques. The dataset used for training and testing contains movie entries with titles, genres, and plots.

### Data Preparation

- The dataset is loaded from a text document file, where each line represents a movie entry with columns separated by ':::'.
- Data cleaning is performed to handle missing values, if any.

### Feature Extraction

- Plot summaries are tokenized and vectorized using the CountVectorizer from scikit-learn.
- Genre labels are encoded into numerical representations using LabelEncoder from scikit-learn.

### Model Training

- Data is split into training and testing sets.
- A pipeline for model training is defined, consisting of a VotingClassifier ensemble with Multinomial Naive Bayes and Decision Tree classifiers.
- Grid search cross-validation is performed to tune hyperparameters and optimize model performance.

### Model Evaluation

- The trained model is evaluated on the testing set using metrics such as accuracy, precision, recall, F1 score, and confusion matrix.

### Usage

1. Run the Python script `movie_genre_classification.py`.
2. The script will load the dataset, preprocess the data, train the model, and evaluate its performance.
3. Review the evaluation metrics printed to the console to assess the model's accuracy and effectiveness in classifying movie genres.

### Requirements

- Python 3.x
- pandas
- scikit-learn

### About

This project demonstrates the application of machine learning for movie genre classification. It can be extended and customized with additional preprocessing steps, feature engineering techniques, or different classification algorithms. Contributions and feedback are welcome.

Enjoy exploring movie genre classification with machine learning!
