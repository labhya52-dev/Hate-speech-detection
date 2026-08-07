# Hate Speech Detection

A simple ML pipeline that classifies Twitter posts as hate speech or not, using TF-IDF features and a Decision Tree classifier.

## How it works
1. **Data loading** – reads tweet data from `twitter.csv`
2. **Text cleaning** – lowercases text, strips URLs, mentions, hashtags, and punctuation
3. **Labeling** – flags a post as hate speech (`1`) if it contains any of a predefined set of keywords (e.g. *hate, kill, stupid, idiot, racist, terrorist*); otherwise `0`
4. **Feature extraction** – converts cleaned text to TF-IDF vectors (top 5,000 features, English stopwords removed)
5. **Model** – trains a `DecisionTreeClassifier` on an 80/20 train-test split
6. **Evaluation** – reports accuracy, a classification report, and a confusion matrix heatmap

Thank you
