# Quora_text_classification

## Quora Insincere Questions Classification

### Project Overview
This project aims to classify questions from the Quora platform as either sincere or insincere. The objective is to develop a model that can detect toxic or insincere questions, which can then be flagged and appropriately handled to maintain a healthy and constructive online community.

### Dataset
The dataset used in this project is provided by the Quora Insincere Questions Classification competition on Kaggle. It includes a large collection of questions labeled as either sincere (target=0) or insincere (target=1). The training set comprises over a million labeled questions, while the test set includes around 375,000 questions.

### Data Exploration and Preprocessing
- **Exploratory Data Analysis (EDA)**: Initial data exploration revealed that the dataset is highly imbalanced, with about 94% sincere questions and 6% insincere questions.
- **Text Preprocessing**: Various text preprocessing techniques were applied to clean and prepare the text data for modeling. This included:
  - **Tokenization**: Splitting text into individual words.
  - **Stop Word Removal**: Removing common words that do not contribute significantly to the model's performance (e.g., 'the', 'is').
  - **Stemming**: Reducing words to their root forms (e.g., 'going' to 'go').
  - **Vectorization**: Converting text into numerical vectors using the Bag of Words model. A CountVectorizer was used to create a vocabulary of the most frequent words and transform the questions into vectors based on word counts.

### Model Training
A sample of 100,000 questions was used for initial model development to reduce computational complexity. The data was transformed into vectors, which served as inputs for machine learning algorithms to classify the questions.

### Tools and Libraries
- **Pandas**: For data manipulation and analysis.
- **NLTK**: For natural language processing tasks like tokenization, stop word removal, and stemming.
- **Scikit-learn**: For vectorization and machine learning model implementation.

### Goals and Next Steps
- **Model Evaluation**: Train and evaluate different machine learning models to find the most effective one for this classification task.
- **Optimization**: Fine-tune the model parameters to improve performance.
- **Deployment**: Implement the final model into a system that can automatically flag insincere questions on Quora.

This project provides a structured approach to handling text data and building a machine learning model for binary classification. It leverages various preprocessing techniques to prepare the data and uses CountVectorizer to transform text into a format suitable for machine learning algorithms.
