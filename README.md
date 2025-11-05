AI/ML Intermediate Project
# Sentiment Analysis of Social Media

## Overview
This project focuses on analyzing the sentiment of social media posts using Natural Language Processing (NLP) and Machine Learning (ML) techniques. The model classifies text data into three sentiment categories: Positive, Negative, and Neutral. This allows users to understand the general sentiment trends in social media data and can be extended for applications like brand monitoring, public opinion analysis, and online reputation management.

## Dataset
The dataset used in this project is the **Social Media Sentiments Analysis Dataset** from Kaggle. It contains real-world social media posts with various emotion and sentiment labels. 
Link : https://www.kaggle.com/datasets/kashishparmar02/social-media-sentiments-analysis-dataset
We did not download additional datasets manually for model training; instead, we cleaned and simplified the provided dataset by:
- Removing unnecessary columns (like timestamps, hashtags, etc.)
- Simplifying the sentiment labels to three categories: **Positive**, **Negative**, and **Neutral**
- Cleaning text by removing special characters, URLs, emojis, and extra spaces

After preprocessing, the data was balanced and split for training and testing.

## Project Workflow
1. **Data Loading and Exploration**
   - Loaded the dataset into a pandas DataFrame.
   - Explored structure, column names, and missing values.

2. **Data Cleaning and Preprocessing**
   - Removed duplicate and unnecessary columns.
   - Normalized sentiment labels to a simplified format.
   - Cleaned the text using regular expressions (removing links, punctuation, symbols, etc.).

3. **Feature Extraction**
   - Used TF-IDF (Term Frequency–Inverse Document Frequency) to convert text into numerical vectors suitable for ML models.

4. **Model Building**
   - Implemented a **Logistic Regression** classifier using scikit-learn.
   - Trained on 80% of the dataset and tested on the remaining 20%.

5. **Model Evaluation**
   - Achieved approximately **71% accuracy** on test data.
   - Evaluated using classification metrics such as precision, recall, and F1-score.
   - Visualized performance using a confusion matrix.

6. **Gradio App Integration**
   - Added an interactive interface using **Gradio**, allowing users to type or paste a social media post and instantly get the predicted sentiment.
   - The interface provides:
     - A text box for user input.
     - Real-time prediction with confidence percentage.
   - Gradio was chosen because it provides a fast and user-friendly way to deploy ML models for demonstrations and testing without complex backend setup.

## How It Works
- User enters a social media post in the Gradio interface.
- The text is cleaned, vectorized using TF-IDF, and passed to the trained Logistic Regression model.
- The model predicts whether the post is Positive, Negative, or Neutral.
- The result is displayed instantly with confidence level.

## Installation and Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/social-media-sentiment-analysis.git
   cd social-media-sentiment-analysis
   ```

## Contributing
Contributions are welcome!
Feel free to fork the repository, improve the game, and open a pull request. Let's grow this classic game together!

## License
This project is licensed under the [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

## Author
**Aarya Mehta**  
🔗 [GitHub Profile](https://github.com/AaryaMehta2506)


