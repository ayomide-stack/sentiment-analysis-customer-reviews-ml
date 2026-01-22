
# Sentiment Analysis of Customer Reviews
**Sentiment analysis using TF–IDF + Naive Bayes, Logistic Regression, and SVM on UCI dataset.**

In this project, I worked with short customer review texts collected from multiple online
platforms and applied supervised machine learning techniques to automatically classify
opinions as positive or negative. The focus was not only on model performance, but also on
building a clear, reproducible natural language processing (NLP) workflow and interpreting
how different models learn sentiment patterns from text.

## Project Aims

The main aim of this project was to design and implement a complete sentiment analysis
pipeline using real-world textual data. Specifically, I aimed to:

1. Explore and understand the structure of short customer reviews through EDA
2. Apply NLP preprocessing techniques to clean and normalise text
3. Convert text into numerical features using TF–IDF vectorisation
4. Train and evaluate multiple supervised classification models
5. Compare model performance and analyse their strengths and limitations
6. Interpret learned feature weights to understand influential sentiment terms
7. Reflect on ethical and social considerations of automated text analysis

## Prediction Task

The dataset was formulated as a binary sentiment classification problem:

**1. Sentiment Classification**
Predicting whether a customer review expresses:

a. Positive sentiment (1)

b. Negative sentiment (0)

This task reflects real-world business applications such as:

a. Monitoring customer satisfaction

b. Detecting negative feedback early

c. Supporting service improvement and product evaluation

## Dataset

**1. Source**: UCI Sentiment Labelled Sentences Dataset

**2. Link**: https://archive.ics.uci.edu/dataset/331/sentiment+labelled+sentences

**3. Size**: 3,000 sentences

**4. Sources**: Amazon product reviews, Yelp business reviews, IMDb movie reviews

## Features:

**1. text** – review sentence (independent variable)

**2. label** – sentiment class (dependent variable)

The dataset combines multiple review domains, allowing the models to learn sentiment
patterns across different writing styles and contextual expressions.

## Methods and Tools
Models Used

**Multinomial Naive Bayes**
Used as a probabilistic baseline model that performs well with sparse text features.

**Logistic Regression**
Used as an interpretable linear classifier that assigns weighted importance to words.

**Linear Support Vector Machine (SVM)**
Used as a high-performance linear classifier that maximises separation between sentiment
classes in high-dimensional feature space.

## Libraries

1. Python
2. pandas and numpy for data handling
3. matplotlib for visualisation
4. scikit-learn for vectorisation, modelling, and evaluation
5. nltk for tokenisation, stopword removal, and lemmatisation

## Workflow Overview
The project follows a structured and reproducible NLP and machine learning workflow:

1. Loading and combining datasets from multiple sources
2. Performing exploratory data analysis (EDA) on text length and class distribution
3. Preprocessing text using tokenisation, stopword removal, and lemmatisation
4. Converting text into numerical features using TF–IDF with unigrams and bigrams
5. Splitting data into training and test sets using stratification
6. Training three supervised classification models
7. Evaluating performance using standard classification metrics
8. Exporting model coefficients for interpretability analysis
9. Saving all outputs to organised results folders

## Model Evaluation
To evaluate model performance, I used:

1. Accuracy
2. Precision
3. Recall
4. F1-score
5. Confusion matrices for error analysis
   
These metrics provide a balanced assessment of classification performance and allow
direct comparison between different models. Linear SVM achieved the highest overall
accuracy, followed closely by Logistic Regression, while Naive Bayes provided a strong and
efficient baseline.

## Ethical Considerations

Although the dataset is anonymised and publicly available, sentiment analysis systems can
still reflect biases present in user-generated language. Expressions of emotion, sarcasm,
and cultural differences may be misinterpreted by automated systems.

In real-world applications, such models should be used to support and not replace no human
judgement, particularly when monitoring customer feedback or moderating online content.
Responsible use requires transparency, regular evaluation, and awareness of potential
misclassification risks.

Ayomide Ogunmakinwa

DATA SCIENTIST
