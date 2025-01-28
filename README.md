# Sentiment Analysis Application

## Overview

The **Sentiment Analysis Application** is a tool designed to analyze the sentiment of textual data and classify it as **Positive**, **Neutral**, or **Negative**. This app is built using **Streamlit** and leverages a pre-trained machine learning model along with TF-IDF vectorization for feature extraction. The dataset and pre-trained model were sourced from **Hugging Face** and processed locally.

## Features

- Analyze text sentiment using a trained model.
- Supports the analysis of multiple reviews.
- Provides a clean and interactive interface built with **Streamlit**.
- Visual feedback with emoticons and color-coded results.
- Pre-trained assets and dataset for reproducibility.

## Files in Repository

Below is the list of files included in the repository:

### Model Files

1. `Tfidf vectorizer`:

   - Contains the saved TF-IDF vectorizer used for transforming text into numerical features.

2. `sentiment model`:

   - Pre-trained sentiment classification model used for predicting the sentiment of reviews.

3. ``:

   - Contains the label encoder to map numeric predictions back to categorical sentiments (Positive, Neutral, Negative).

### Dataset

4. ``:

   - Cleaned and preprocessed dataset used for training and testing the model. The dataset was obtained from **Hugging Face**.

5. ``:

   - Saved features for TF-IDF, including training and test splits: `X_train`, `X_test`, `y_train`, and `y_test`.

### Application Files

6. ``:

   - Main Streamlit application file for running the sentiment analysis app.

7. ``:

   - An image or banner used in the Streamlit interface for enhancing visual appeal.

### Other

8. ``:
   - Additional supporting files or scripts for the sentiment analysis app.

## How to Run the App

### Prerequisites

1. Install **Python 3.7+**.
2. Install the required libraries listed in `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/your_username/sentiment-analysis-app.git
   cd sentiment-analysis-app
   ```

2. Ensure all required files (e.g., models, datasets) are in the same folder.

3. Run the application:

   ```bash
   streamlit run sentiment__app.py
   ```

4. Open the provided URL in a web browser to access the application.

## Application Workflow

1. Enter a review or text in the input box.
2. Click the **Analyze Sentiment** button to get the result.
3. The sentiment (Positive, Neutral, or Negative) will be displayed with visual feedback.
4. Use the **Analyze New Review** button to reset and analyze another review.

## Dataset

The dataset used for training the model is available on **Hugging Face** and includes a variety of labeled textual reviews. It has been preprocessed and saved as `cleaned_dataset.csv` for easy reuse.

## Model Details

- **Vectorization**: TF-IDF vectorizer (`tfidf_vectorizer.pkl`).
- **Classification Model**: Pre-trained machine learning model (`sentiment model.pkl`).
- **Label Mapping**: Handled by `label_encoder.pkl`.

## Acknowledgments

- **Hugging Face** for providing the dataset.
- **Streamlit** for enabling the creation of interactive web applications.

## Future Enhancements

- Integration with **BERT** for improved sentiment classification.
- Support for multi-language sentiment analysis.
- Adding visualizations to display dataset insights.

## License

This project is licensed under the [MIT License](LICENSE).

