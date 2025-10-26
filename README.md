# Tiktok Review from Google Play Store Sentiment Analysis

This repository contains the complete **Sentiment Analysis** workflow, covering data acquisition, cleaning, model training, and inference. The project is designed to classify text data (e.g., social media or app reviews) into different sentiment categories: Positive, Negative, or Neutral.

## Overview

This project provides a reproducible NLP pipeline for developing a text classification model. It's implemented using Python and Jupyter Notebooks, making it easy to follow, customize, adn extend to other natural language processing (NLP) tasks.

## Key Features

* **Data Scraping:** A dedicated notebook (`data_scraping.ipynb`) collect raw text data from an external source, e.g., Google Play Store app reviews
* **Text Preprocessing:** Includes steps for cleaning and preparing text data, using a custom `slangwords.json` dictionary for normalizing informal Indonesian or local slang. The dictionary was modified according to the dataset of TikTok reviews scraped from the Google Play Store
* **Sentiment Modeling:** A full notebook (`sentiment_analysis.ipynb`) that handles preprocessing, feature engineering, model training, and evaluation using Scikit-learn or TensorFlow.
* **Inference Pipeline:** A separate notebook (`inference.ipynb`) for loading the trained model and make predictions on new, unseen data efficiently.

## Technologies & Dependencies

The project is built primarily using **Python** and is encapsulated within **Jupyter Notebooks**. All required libraries are listed in `requirements.txt`.

* **Primary Language:** Python (Jupyter Notebook)
* **Core Libraries:**
    * `pandas`, `numpy` (Data handling)
    * `scikit-learn`, `tensorflow` (Modeling)
    * `requests` (Data scraping)
    * `nltk`/`sastrawi` (Text processing)

## Installation and Setup

Follow these steps to set up the project environment locally.

### 1. Clone the Repository

```bash
git clone https://github.com/laventilizz/review_sentiment_analysis.git
cd review_sentiment_analysis
```

### 2. Create and Activate Virtual Environment (Recommended)

```bash
python 3.11.9 -m venv sentiment-env
.\sentiment-env\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## Usage
Run the notebooks in the following order:
1. `data_scraping.ipynb`: Collect raw data from the Google Play Store.
2. `sentiment_analysis.ipynb`: Preprocess, normalize text (using slangwords.json), train, and evaluate the sentiment model.
3. `inference.ipynb`: Load the trained model and make predictions on new reviews.
   
## Repository File Structure

| File | Description |
|--------------|-------------|
| `data_scraping.ipynb` | Script for initial data collection. |
| `sentiment_analysis.ipynb` | Core notebook for data preprocessing, feature engineering, model training, and evaluation. |
| `inference.ipynb` | Notebook for loading the final model and performing sentiment prediction on new input. |
| `requirements.txt` | List of all Python dependencies. |
| `slangwords.json` | JSON file containing a dictionary of slang words and their standard counterparts for text normalization. |
| `README.md` | The main project documentation file. |



<pre>Notes: This project was created to fulfill the submission requirement for the a course. The dataset was collected from 
Google Play Store reviews of the TikTok app and preprocessed using a modified `slangwords.json` dictionary.
Feel free to explore, fork, or improve it for your own NLP projects
</pre>
