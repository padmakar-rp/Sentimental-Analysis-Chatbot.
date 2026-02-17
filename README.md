# Sentimental-Analysis-Chatbot.
This is a simple Sentiment Analysis Chatbot built using Google Colab. This repository contains the complete project code along with images of the chatbot’s output.

[ CREATED USING GOOGLE COLAB ]

# Sentiment Analysis Chatbot

A simple Machine Learning–based sentiment chatbot built using Python, NLTK, and Scikit-learn.  
The chatbot analyzes user input and predicts whether the sentiment is **Positive** or **Negative**.

The application runs in the terminal and continues interacting with the user until `exit` is typed.

---

## Table of Contents

- Overview
- Features
- Technologies Used
- Project Structure
- Installation
- Usage
- How It Works
- Model Details
- Limitations
- Future Improvements
- License

---

## Overview

This project demonstrates a basic Natural Language Processing (NLP) pipeline using:

- Text preprocessing
- TF-IDF vectorization
- Logistic Regression classification

It is designed as a beginner-friendly machine learning project that introduces text classification concepts in a simple and practical way.

---

## Features

- Text preprocessing (lowercasing, punctuation removal, stopword filtering)
- Tokenization using NLTK
- TF-IDF feature extraction
- Logistic Regression classifier
- Interactive command-line chatbot
- Clean and readable implementation

---

## Technologies Used

- Python 3.x
- NLTK
- Scikit-learn
- Regular Expressions (re module)
- String processing

---

## Project Structure

```
sentiment-chatbot/
│
├── chatbot.py        # Main chatbot script
├── README.md         # Project documentation
```

---

## Installation

### 1. Clone the Repository

```
git clone https://github.com/your-username/sentiment-chatbot.git
cd sentiment-chatbot
```

### 2. Install Dependencies

```
pip install nltk scikit-learn
```

### 3. Run the Application

```
python chatbot.py
```

---

## Usage

After running the script, the chatbot will prompt for user input:

```
Chatbot Ready! Type 'exit' to stop.
```

Type any sentence to analyze sentiment.  
Type `exit` to end the conversation.

---

## Example

```
Chatbot Ready! Type 'exit' to stop.

You: I feel amazing today
Chatbot: You sound positive!

You: This is the worst experience ever
Chatbot: You seem upset.

You: exit
Chatbot: Goodbye!
```

---

## How It Works

1. A small labeled dataset is manually created.
2. Text preprocessing includes:
   - Converting text to lowercase
   - Removing numbers
   - Removing punctuation
   - Tokenizing text
   - Removing stopwords
3. The cleaned text is transformed using TF-IDF vectorization.
4. A Logistic Regression model is trained on the processed dataset.
5. User input is preprocessed and classified as:
   - `1` → Positive
   - `0` → Negative
6. The chatbot runs in a loop until `exit` is entered.

---

## Model Details

- Vectorizer: TF-IDF (Term Frequency – Inverse Document Frequency)
- Classifier: Logistic Regression
- Training Samples: 20 manually created examples
- Classification Type: Binary (Positive / Negative)

---

## Limitations

- Small training dataset limits generalization
- Does not handle sarcasm or complex linguistic patterns
- Binary sentiment classification only
- No model evaluation metrics included

---

## Future Improvements

- Add Neutral sentiment classification
- Expand dataset with real-world data
- Include model evaluation metrics (Accuracy, Precision, Recall, F1-Score)
- Save and load trained model
- Build a graphical user interface (GUI)
- Deploy as a web application
- Implement advanced NLP models (LSTM, BERT)

---

