# Email Security & Phishing Detection

## Project Overview

This project explores the application of Machine Learning and Deep Learning techniques to identify phishing emails and distinguish them from legitimate emails.

The project implements and compares two classification approaches:

- **Logistic Regression** – A traditional machine learning approach using TF-IDF feature extraction.
- **Long Short-Term Memory (LSTM)** – A deep learning approach designed to learn sequential patterns in email text.

The objective is to evaluate both approaches using standard classification metrics and understand their effectiveness in detecting phishing emails.

## Technologies Used

- Python
- Pandas & NumPy
- Scikit-learn
- TensorFlow / Keras
- NLTK
- Matplotlib & Seaborn
- Hugging Face Datasets

## Dataset

The project uses the [Phishing Email Dataset](https://huggingface.co/datasets/zefang-liu/phishing-email-dataset), hosted on Hugging Face.

The dataset contains email text labelled as:
- Phishing Email
- Safe Email

The notebook automatically downloads the dataset, so manual dataset uploads are not required.

## Project Workflow

### 1. Data Collection & Preparation
- Download the dataset from Hugging Face.
- Inspect the dataset and class distribution.
- Handle missing values.
- Convert email labels into binary classification values.

### 2. Text Preprocessing
- Convert text to lowercase.
- Remove URLs, email addresses and HTML tags.
- Remove non-alphabetic characters.
- Remove English stop words.
- Apply lemmatization.

### 3. Logistic Regression
- Extract text features using TF-IDF.
- Use unigrams and bigrams.
- Train a Logistic Regression classifier.
- Evaluate classification performance.

### 4. LSTM Deep Learning Model
- Tokenize email content.
- Convert text into numerical sequences.
- Apply sequence padding.
- Build and train an LSTM neural network.
- Use early stopping to help prevent overfitting.

### 5. Model Evaluation & Comparison

Both models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve and AUC

The notebook also provides visual comparisons of model performance.

## How to Run

The project is designed to run in **Google Colab**.

1. Open the `.ipynb` notebook in Google Colab.
2. Select Runtime → Change runtime type.
3. GPU is optional but can help accelerate LSTM training.
4. Run all cells from top to bottom.

The required Python libraries are installed within the notebook, and the dataset is downloaded automatically.

## Repository Structure

```text
Email-Security-and-Phishing-Detection/
│
├── 1_Email_Security_&_Phishing_Detection.ipynb
└── README.md
```

## Learning Objectives

This project demonstrates practical implementation of:

- Email security and phishing detection concepts.
- Natural Language Processing (NLP).
- Text preprocessing and feature extraction.
- Traditional Machine Learning classification.
- Deep Learning using LSTM networks.
- Model evaluation and performance comparison.

## Disclaimer

This is an educational machine learning project developed to explore phishing email classification. The models are experimental and should not be considered standalone solutions for production email security systems.

---

**Project Area:** Cybersecurity | Machine Learning | Deep Learning | NLP# Email-Security-and-Phishing-Detection
