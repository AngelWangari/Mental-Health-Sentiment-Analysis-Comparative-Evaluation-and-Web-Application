# 🧠 Mental Health Sentiment Analysis

## Project Overview

This project evaluates and compares multiple machine learning models to identify the most robust approach for **neutral sentiment detection** in mental health-related customer reviews. The study also includes a web-based application for real-time sentiment prediction.

## Project Title

**Evaluation and Comparative Analysis of Sentiment Analysis Models to Identify the Most Robust Approach for Neutral Sentiment Detection in Mental Health–Related Customer Reviews with Web Application Integration**

## Features

* Text preprocessing and data cleaning
* TF-IDF feature extraction
* Hyperparameter tuning using GridSearchCV
* Comparative evaluation of:

  * Logistic Regression
  * Naive Bayes
  * Linear SVM
* Hybrid LR + SVM Ensemble model
* Exploratory Data Analysis (EDA) and visualizations
* Interactive Gradio web application for real-time sentiment prediction
* Streamlit dashboard for model performance visualization

## Dataset

The project uses a mental health text dataset containing reviews categorized into three sentiment classes:

* Very Negative
* Negative
* Neutral

## Technologies Used

* Python
* Scikit-learn
* Pandas
* NumPy
* Matplotlib & Seaborn
* Plotly
* Streamlit
* Gradio
* Joblib

## Model Performance

| Model                        | Accuracy   |
| ---------------------------- | ---------- |
| Logistic Regression          | 88.49%     |
| Linear SVM                   | 88.46%     |
| Naive Bayes                  | 79.03%     |
| **Hybrid LR + SVM Ensemble** | **89.60%** |

The Hybrid LR + SVM Ensemble achieved the highest performance and was selected for deployment in the web application.

## Project Structure

```text
project-dsa/
│── models/
│── app.py
│── predict.py
│── trainmodel.py
│── trainensemble.py
│── sentiment_dashboard.py
│── edavisuals.py
│── requirements.txt
│── README.md
```

## Running the Project

1. Clone the repository.
2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. Train the models:

```bash
python trainmodel.py
python trainensemble.py
```

4. Launch the Gradio application:

```bash
python app.py
```

5. Launch the Streamlit dashboard:

```bash
streamlit run sentiment_dashboard.py
```

## Author

Developed as a Data Science research project focusing on robust sentiment analysis techniques for mental health-related text classification.
Limitations

While the project achieved strong performance in neutral sentiment detection, it has several limitations:

The dataset is limited to mental health–related customer reviews, which may reduce the model's ability to generalize to other domains.
Class imbalance within the dataset can influence model performance despite the use of stratified sampling and Macro F1-score evaluation.
TF-IDF captures word frequency but has limited understanding of context and semantic relationships between words.
Traditional machine learning models may struggle with sarcasm, irony, implicit emotions, and complex sentence structures.

# 🧠 Mental Health Sentiment Analysis

## Project Overview

This project evaluates and compares multiple machine learning models to identify the most robust approach for **neutral sentiment detection** in mental health-related customer reviews. The study also includes a web-based application for real-time sentiment prediction.

## Project Title

**Evaluation and Comparative Analysis of Sentiment Analysis Models to Identify the Most Robust Approach for Neutral Sentiment Detection in Mental Health–Related Customer Reviews with Web Application Integration**

## Features

* Text preprocessing and data cleaning
* TF-IDF feature extraction
* Hyperparameter tuning using GridSearchCV
* Comparative evaluation of:

  * Logistic Regression
  * Naive Bayes
  * Linear SVM
* Hybrid LR + SVM Ensemble model
* Exploratory Data Analysis (EDA) and visualizations
* Interactive Gradio web application for real-time sentiment prediction
* Streamlit dashboard for model performance visualization

## Dataset

The project uses a mental health text dataset containing reviews categorized into three sentiment classes:

* Very Negative
* Negative
* Neutral

## Technologies Used
Add the fact that limitations;dataset constraints, semantic similarity and future work was to icotporate transformed bert models deeplearning and database 

You can update your project README by adding the following sections after Technologies Used.

Technologies Used
Python

Pandas

NumPy

Scikit-learn

NLTK

Matplotlib

Seaborn

Plotly

Gradio

Streamlit

Joblib

Limitations
While the project achieved strong performance in neutral sentiment detection, it has several limitations:

The dataset is limited to mental health–related customer reviews, which may reduce the model's ability to generalize to other domains.

Class imbalance within the dataset can influence model performance despite the use of stratified sampling and Macro F1-score evaluation.

TF-IDF captures word frequency but has limited understanding of context and semantic relationships between words.

Traditional machine learning models may struggle with sarcasm, irony, implicit emotions, and complex sentence structures.

Dataset Constraints
The dataset contains only three sentiment classes: Very Negative, Negative, and Neutral.

Reviews vary in length and writing style, introducing inconsistencies during preprocessing.

Neutral reviews often share vocabulary with negative reviews, making them difficult to distinguish accurately.

The dataset may not fully represent diverse populations, cultures, or mental health discussions found in real-world applications.

Semantic Similarity Challenge
One of the primary challenges encountered was the high semantic similarity between Neutral and Negative reviews. Many reviews use similar words while expressing different sentiment intensities, making classification difficult for traditional TF-IDF-based machine learning models. This overlap increases the likelihood of misclassification and highlights the need for models capable of understanding contextual meaning.

Future Work
Future improvements to this project include:

Incorporating transformer-based deep learning models such as BERT, RoBERTa, and DistilBERT to improve contextual understanding and semantic representation.

Evaluating advanced deep learning architectures for improved sentiment classification performance.

Integrating a relational or NoSQL database (e.g., MongoDB or PostgreSQL) to store user predictions, historical sentiment data, and application logs.

Expanding the dataset with more diverse mental health reviews and additional sentiment categories.

Deploying the web application on a cloud platform for scalable real-world use.

Exploring explainable AI techniques to provide interpretable predictions and improve user trust.
