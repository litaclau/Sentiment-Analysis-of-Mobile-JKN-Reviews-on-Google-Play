# Sentiment Analysis of Mobile JKN Google Play Reviews

This project analyzes **12,105 Mobile JKN reviews from Google Play Store collected between June and August 2026** using Natural Language Processing (NLP) and Machine Learning.

The reviews are classified into three sentiment categories:

- Negative
- Neutral
- Positive

The workflow includes **data scraping, manual labeling, text preprocessing, TF-IDF feature extraction, model comparison, sentiment prediction, and visualization**.

## Model Performance

Three models were compared:

- Logistic Regression
- Linear SVM
- Multinomial Naive Bayes

**Linear SVM** achieved the best performance.

| Metric | Score |
|---|---:|
| Accuracy | **90.35%** |
| Precision Macro | **88.32%** |
| Recall Macro | **87.92%** |
| F1 Macro | **88.04%** |

---

## Analysis Results

### 1. Final Sentiment Distribution

![Final Sentiment Distribution](Output%20Hasil%20Analisis/Grafik%20%26%20Wordcloud/distribusi_sentimen.png)

From 12,105 reviews:

- **Negative:** 5,809 (48.0%)
- **Neutral:** 930 (7.7%)
- **Positive:** 5,366 (44.3%)

Negative sentiment is the largest category, although positive sentiment also represents a substantial proportion of reviews.

---

### 2. Main User Complaints

![Negative Review WordCloud](Output%20Hasil%20Analisis/Grafik%20%26%20Wordcloud/wordcloud_keluhan_negatif.png)

Common complaint topics include **login, registration, phone number, verification, OTP, and application errors**.

---

### 3. Peak Review Hour

![Peak Review Hour](Output%20Hasil%20Analisis/Grafik%20%26%20Wordcloud/jam_puncak_ulasan.png)

The highest review activity occurred at **09:00 WIB**, with **959 reviews**.

---

### 4. Confusion Matrix

![Confusion Matrix](Output%20Hasil%20Analisis/Grafik%20%26%20Wordcloud/confusion_matrix.png)

The final Linear SVM model correctly classified most Negative and Positive reviews, while Neutral sentiment was relatively more difficult to distinguish.

---

### 5. Main Positive Feedback

![Positive Review WordCloud](Output%20Hasil%20Analisis/Grafik%20%26%20Wordcloud/wordcloud_pujian_positif.png)

Positive feedback commonly highlights that Mobile JKN is **helpful, easy to use, fast, convenient, and useful for accessing healthcare services**.

---

### 6. Sentiment by Rating

![Sentiment by Rating](Output%20Hasil%20Analisis/Grafik%20%26%20Wordcloud/sentimen_berdasarkan_rating.png)

Low ratings are strongly associated with Negative sentiment, while higher ratings, especially Rating 5, are dominated by Positive sentiment.

---

## Technologies Used

`Python` · `Pandas` · `Scikit-learn` · `TF-IDF` · `Sastrawi` · `Matplotlib` · `WordCloud` · `Google Play Scraper` · `Gradio`

## Conclusion

The analysis shows that Mobile JKN receives both significant criticism and positive feedback. The main complaints are related to **login, OTP, verification, registration, and application errors**, while positive reviews emphasize **ease of use, usefulness, and convenience**.

## Disclaimer

This project was created for **educational and portfolio purposes** and is not an official analysis by BPJS Kesehatan.
