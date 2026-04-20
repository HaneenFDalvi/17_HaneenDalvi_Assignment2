## (1) Problem Statement
During the COVID-19 pandemic, people shared opinions, emotions, and information through Twitter. The problem is to automatically classify COVID-19 related tweets into sentiment categories (Positive, Neutral, Negative) using Machine Learning techniques.

## (2) Objective
- To perform sentiment analysis on COVID-19 tweets.
- To classify tweets into Positive, Neutral, and Negative categories.
- To train and compare multiple Machine Learning models (Naïve Bayes, SVM, Logistic Regression).
- To evaluate the models using Precision, Recall, F1-score, and Accuracy.

## (3) Dataset
- Source: Kaggle (COVID-19 Tweets Dataset)
- Features:
  - `tweets` (tweet text)
  - `sentiment` (label: positive / neutral / negative)
- Size: 100 tweets

## (4) Methodology
1. **Data Preprocessing**
   - Loaded dataset using Pandas
   - Removed missing values
   - Converted tweet text into numerical features using TF-IDF Vectorization

2. **EDA**
   - Displayed dataset samples
   - Checked sentiment distribution across classes

3. **Model Building**
   - Trained the following models:
     - Multinomial Naïve Bayes
     - Support Vector Machine (LinearSVC)
     - Logistic Regression

4. **Evaluation**
   - Evaluated models using:
     - Accuracy
     - Precision (Macro Average)
     - Recall (Macro Average)
     - F1-score (Macro Average)
   - Compared model performance using F1-score graph

## (5) Results
- All three models produced nearly similar performance.
- The F1-score for Naïve Bayes, SVM, and Logistic Regression was approximately around 0.43–0.44.
- SVM and Logistic Regression slightly performed better than Naïve Bayes, but the difference was minimal.
- The small dataset size (100 tweets) may have limited overall model performance.

## (6) How to Run
```bash
pip install -r requirements.txt
python main.py
```

## (7) Conclusion
This project successfully implemented sentiment analysis on COVID-19 tweets using Machine Learning models. Tweets were processed using TF-IDF vectorization and classified into positive, neutral, and negative sentiments. Naïve Bayes, SVM, and Logistic Regression models were trained and tested. The results showed that all models achieved nearly equal performance with F1-scores around 0.43–0.44. This indicates that the dataset size is small and sentiment classification on short tweets is challenging. For improved accuracy, future work can use a larger dataset and advanced NLP models such as word embeddings or deep learning techniques.

## (8) Student's details
- Name: Haneen Dalvi
- Roll No: 17
- UIN: 242A002
- YEAR: TE-AIDS
