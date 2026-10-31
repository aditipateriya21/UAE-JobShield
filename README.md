# UAE JobShield – Recruitment Scam Detection System

## Project Overview

UAE JobShield is an NLP-based recruitment scam detection and risk screening system designed for the UAE job market.

The system analyses job descriptions and recruitment messages and classifies them into three categories:

- **Fraudulent:** Content displaying strong indicators of recruitment fraud.
- **Suspicious:** Content containing potentially risky or unusual recruitment patterns.
- **Legitimate:** Content that does not exhibit the identified scam indicators.

It combines a machine learning classifier with rule-based warning detection to help users identify potentially unsafe recruitment communications.

## Objectives

- Develop an NLP-based system for recruitment scam screening.
- Classify job-related text into three risk categories.
- Identify warning signs such as recruitment fees and requests for sensitive personal information.
- Provide an interactive interface for testing job descriptions and messages.
- Explore the application of NLP to recruitment safety in the UAE context.

## Technologies Used

- Python
- Pandas and NumPy
- Scikit-learn
- TF-IDF Vectorization (word and character features)
- Logistic Regression
- Matplotlib and Seaborn
- Gradio
- Joblib

## Methodology

The project follows these main steps:

1. **Data Collection:** Uses the `agnialf/Internship-Job-Scam-Dataset` dataset from Hugging Face.
2. **Data Preprocessing:** Cleans text, handles missing values, and removes duplicate records.
3. **Exploratory Data Analysis:** Examines class distribution and dataset characteristics.
4. **Feature Extraction:** Converts text into numerical features using word-level and character-level TF-IDF.
5. **Model Training:** Trains Logistic Regression classifiers for three-class classification.
6. **Model Evaluation:** Evaluates performance using accuracy, precision, recall, F1-score, and confusion matrices.
7. **Risk Detection:** Applies rule-based checks to identify warning patterns in recruitment messages.
8. **Prototype:** Provides an interactive Gradio interface for testing user-provided text.

## Model Performance

The improved model uses combined word-level and character-level TF-IDF features with Logistic Regression.

| Evaluation Metric | Result |
|---|---:|
| Accuracy | 83.24% |
| Macro Precision | 83.19% |
| Macro Recall | 83.20% |
| Macro F1-score | 83.15% |

The improved model was compared against a baseline word-level TF-IDF model, which achieved 80.45% accuracy.

## Project Structure

```text
UAE-JobShield/
