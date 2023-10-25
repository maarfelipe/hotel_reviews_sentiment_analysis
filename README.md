# Hotel Reviews Sentiment Analysis

## Overview

This repository contains code for a sentiment analysis project focused on hotel reviews. The project aims to analyze hotel reviews to understand the sentiment of guests and provide insights into their experiences. The code is designed to load a dataset, perform sentiment analysis, and visualize the sentiment distribution.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Analysis Results](#analysis-results)
- [License](#license)

## Prerequisites

Before running the code, ensure that you have the following dependencies installed:

- Python (3.6 or higher)
- Jupyter Notebook or a Python IDE of your choice
- Required Python libraries (Matplotlib, Pandas, NLTK)

You can install the necessary libraries using pip:

```bash
pip install matplotlib pandas nltk
```

To utilize `nltk.sentiment.vader` effectively, you need to ensure the VADER lexicon is installed. Follow these steps:

1. Open a Python environment (e.g., by running `python` in your terminal).
2. Import the Natural Language Toolkit (NLTK):

   ```python
   import nltk
   nltk.download('vader_lexicon')
   ```

Make sure to execute these commands within a Python environment to download the VADER lexicon successfully.

## Getting Started

To use this code, follow these steps:

1. Clone the repository to your local machine:

```bash
git clone https://github.com/maarfelipe/hotel_reviews_sentiment_analysis
```

2. Navigate to the project directory:

```bash
cd hotel-reviews-sentiment-analysis
```

3. Open the Jupyter Notebook file `reviewer.ipynb` to run the code interactively.

## Project Structure

The project repository is organized as follows:

- `reviewer.ipynb`: The Jupyter Notebook containing the code for sentiment analysis.
- `dataset/`: A directory containing the dataset file `hotel_reviews.csv`.
- `README.md`: The documentation you are currently reading.

## Usage

### 1. Data Loading and Initial Exploration

The code begins by loading the dataset from `hotel_reviews.csv` and displaying the first few rows using Pandas. The structure of the dataset is explored using `.info()` and missing values are checked with `.isnull().sum()`.

### 2. Data Visualization

The code generates a pie chart to visualize the distribution of hotel review ratings, providing insights into the overall satisfaction levels of guests.

### 3. Sentiment Analysis

The sentiment analysis process is performed using the NLTK VADER SentimentIntensityAnalyzer. The code calculates positive, negative, and neutral sentiment scores for each review, adds these scores as new columns, and displays the first few rows of the updated dataset.

### 4. Overall Sentiment Analysis

An overall sentiment analysis is conducted by summing the sentiment scores, and a function is used to classify the dataset as 'Positive', 'Negative', or 'Neutral'. The results are printed to provide insights into the general sentiment of the reviews.

## Analysis Results

- The code reveals that most guests have provided 5-star and 4-star ratings, indicating a high level of satisfaction with the hotel services.

- Subsequent sentiment analysis shows that the majority of reviews are classified as 'Neutral,' and a substantial number are categorized as 'Positive,' reinforcing the notion that guests are content with their experiences.

- Negative reviews are relatively low in number, with less than 1,500 instances, further underscoring the positive sentiment.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.