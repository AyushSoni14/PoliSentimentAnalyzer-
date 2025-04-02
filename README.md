# Political Sentiment Analyzer
Political Sentiment Analysis from YouTube Comments

## Dataset

The dataset consists of YouTube Hinglish comments on the two major Indian political parties:

- Bharatiya Janata Party (BJP)
- Indian National Congress (Congress)

The dataset is divided into two files, one containing comments related to BJP and another for Congress. The experiment is performed on merged comments from both files. Thanks to the original dataset author, available here: [Zenodo Dataset](https://zenodo.org/records/3055456#.XScftOhKhPZ)
.

## Input Files

### 1. YouTube comments  for Congress dataset.csv
This file contains extracted YouTube comments along with their labeled sentiment.

#### Sample Data:

| commentText | Label |
|-------------|-------|
| Modi ji super | 0 |
| You were fool, you are fool and you will be fool | 0 |
| Rahul fool | 0 |
| Rahul is best as PM | 1 |
| Rahul Gandhi thief he | 0 |

### 2. Youtube comments for BJP dataset.csv
This file contains classified YouTube comments after sentiment analysis.

#### Sample Data:

| commentText | Predicted_Label |
|-------------|----------------|
|WE NEED THE KING MAKER  ---- NARENDRA MODI | 1|
| RAHUL GANDHI LEFT THE CHAT | 1|
| Namo again Fir again  | 1 |
| Rahul is best as PM | 0 |
| Rahul Gandhi best he | 0 |

## What is Hinglish?

Hinglish is a code-mixed language combining Hindi and English. Many comments include English words within Hindi sentences. For example:

"Mera brother 5 months se work pe he."

This translates to: "My brother has been working for 5 months." where 'months', 'work', and 'brother' are English words. The challenge with Hinglish is the lack of standardized stopwords, stemmers, and lemmatizers, making it complex to process and analyze user-generated comments.

## AIM

This experiment analyzes YouTube political Hinglish comments related to BJP and Congress. The goal is to evaluate deep learning techniques for extracting political sentiments from these comments. This is a binary classification problem aimed at classifying comments as BJP-supported or Congress-supported.

## Employed Algorithms

- Multilayer Perceptron (MLP)
- LSTM - Long Short-Term Memory
- Convolutional Neural Network (CNN) with LSTM

## Vectorization Techniques

- TF-IDF (Term Frequency - Inverse Document Frequency)
- Keras Tokenizer Text-to-Sequence for Word Embedding

## Evaluation Metrics

- Binary Cross-Entropy for Accuracy
- Receiver Operating Characteristic (ROC) Curves

## Conclusion

Deep learning techniques demonstrated strong performance in extracting political tendencies from comments, achieving an accuracy of 80% or higher.

## Results & Visualization

The project generates:

- Accuracy scores for all models
- Pie charts displaying comment sentiment distribution
- ROC curves for model performance evaluation

## Contributing

Feel free to contribute by submitting a pull request or opening an issue!

