# Movie Reviews Text Classification Project

## Overview

This project implements a machine learning pipeline to classify movie reviews as either **positive** or **negative** sentiments using Natural Language Processing (NLP) techniques and Support Vector Machines (SVM).

## Project Description

The goal of this project is to build an automated sentiment classifier that can accurately predict whether a movie review expresses positive or negative sentiment. This is a classic binary text classification problem solved using TF-IDF vectorization and LinearSVC.

## Dataset

**File:** `moviereviews.csv`

- **Format:** CSV with review text and sentiment labels
- **Features:**
  - `review`: Text content of the movie review
  - `label`: Sentiment label ('pos' for positive, 'neg' for negative)
- **Data Preprocessing:**
  - Removed missing values
  - Removed empty/whitespace-only reviews
  - Balanced sentiment distribution

## Project Workflow

### 1. **Data Loading & Exploration**
   - Load movie reviews from CSV file
   - Examine data structure and info
   - Check for missing values and empty reviews
   - Visualize label distribution using seaborn

### 2. **Exploratory Data Analysis (EDA)**
   - Analyzed most frequent words in positive reviews
   - Analyzed most frequent words in negative reviews
   - Used CountVectorizer for word frequency analysis
   - Identified key sentiment indicators

### 3. **Data Preparation**
   - Split data into 80% training and 20% testing sets
   - Maintained class balance across splits
   - Used `random_state=42` for reproducibility

### 4. **Model Development**
   - **Vectorizer:** TF-IDF (Term Frequency-Inverse Document Frequency)
   - **Classifier:** LinearSVC (Linear Support Vector Machine)
   - **Pipeline:** Combined vectorizer and classifier for seamless preprocessing and prediction

### 6. **Model Evaluation**
   - Classification report with precision, recall, and F1-score
   - Confusion matrix visualization


## Project Structure

```
Text_Classification_Project/
├── main.ipynb              # Main Jupyter notebook with full pipeline
├── moviereviews.csv        # Dataset with movie reviews and labels
└── README.md              # This file
```

## Key Features

- **Complete ML Pipeline:** Data loading → EDA → Preprocessing → Training → Evaluation
- **Well-Documented Code:** Every cell has comments explaining its purpose
- **Model Optimization:** Tuned parameters to balance accuracy and generalization
- **Performance Metrics:** Comprehensive evaluation with multiple metrics
- **Real-world Testing:** Example predictions with interpretation
- **Reproducible Results:** Fixed random seed for consistency

## Model Parameters

**TF-IDF Vectorizer:**
- `stop_words="english"`: Remove common English words

## Files Included

- `main.ipynb` - Complete Jupyter notebook with all code and analysis
- `moviereviews.csv` - Dataset containing movie reviews and sentiment labels
- `README.md` - This documentation file

## Author

Anish Kumar

## License

Educational purpose - Free to use and modify

