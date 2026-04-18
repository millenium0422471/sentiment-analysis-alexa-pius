# Sentiment Analysis - Amazon Alexa Reviews

## Author
Pius Nnaji

## Project Overview
This project performs sentiment analysis on Amazon Alexa customer reviews using Natural Language Processing (NLP) and Machine Learning. The objective is to classify customer feedback as either positive or negative based on review text and product variation.

---

## Dataset
The dataset used is the Amazon Alexa Reviews dataset, which contains approximately 3000 customer reviews.

### Features:
- **rating**: Customer rating (1–5)
- **date**: Date of review
- **variation**: Product type (Echo, Echo Dot, etc.)
- **verified_reviews**: Customer review text
- **feedback**: Sentiment label (1 = Positive, 0 = Negative)

---

## Methodology

### 1. Data Preprocessing
- Removed irrelevant columns (`date`, `rating`)
- Handled missing values
- Cleaned and prepared text data

### 2. Feature Engineering
- One-hot encoding applied to product variation
- Text converted into numerical features using **CountVectorizer (Bag of Words)**

### 3. Model Building
- Used **Random Forest Classifier**
- Trained model on 80% of data and tested on 20%

---

## Model Evaluation

The model performance was evaluated using:

- **Accuracy**
- **Confusion Matrix**
- **Precision, Recall, F1-score**

### Results:
The model achieved strong performance in classifying positive and negative reviews, with high accuracy and balanced precision/recall scores.

---

## Visualizations
- Feedback distribution (positive vs negative)
- Product variation vs rating
- Confusion matrix heatmap
- Feature importance chart

---

## How to Run

1. Open the notebook in Google Colab
2. Mount Google Drive
3. Upload or place `amazon_alexa.tsv` in your Drive
4. Update the dataset path if needed
5. Run all cells in order

---

## Files in this Repository

- `Lesson_10_assignment.ipynb` → Main notebook
- `README.md` → Project documentation

---

## Conclusion

The Random Forest model successfully captures sentiment patterns in customer reviews. This project demonstrates how NLP techniques and machine learning can be applied to real-world text classification problems.

---

## Future Improvements
- Use TF-IDF instead of CountVectorizer
- Try advanced models like SVM or Logistic Regression
- Implement deep learning models such as LSTM or BERT
