# Sentiment Analysis on Amazon Fine Food Reviews

This project performs sentiment analysis on Amazon Fine Food Reviews using Natural Language Processing (NLP) techniques. The goal is to classify reviews as either positive or negative based on their content.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Results](#results)
6. [Technologies Used](#technologies-used)
7. [License](#license)

---

## Project Overview

This project analyzes the sentiment of Amazon Fine Food Reviews using a Logistic Regression model. The steps include:
- Data retrieval and loading
- Data visualization
- Data preprocessing
- Sentiment analysis
- Text preprocessing
- Model training and evaluation

The final model predicts whether a review is positive or negative based on the text content.

---

## Dataset

The dataset used in this project is the **Amazon Fine Food Reviews** dataset, which contains:
- **568,454 reviews** from Amazon users.
- Columns include:
  - `ProductId`: Unique identifier for the product.
  - `UserId`: Unique identifier for the user.
  - `Score`: Rating given by the user (1 to 5).
  - `Summary`: Brief summary of the review.
  - `Text`: Full text of the review.

The dataset is available on [Kaggle](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews).

---

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Irrfan47/Sentiment-Analysis.git
   cd sentiment-analysis
2. **Download the dataset:**
   - Download the dataset from [Kaggle](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews).
   - Place the Reviews.csv file in the project directory.
3. **Run the Jupyter Notebook:**
   ```bash
   jupyter notebook sentiment-analysis.ipynb

---

## Usage

1. Open the sentiment-analysis.ipynb notebook in Jupyter.
2. Run each cell sequentially to:
    - Load and preprocess the data.
    - Visualize the data.
    - Train the Logistic Regression model.
    - Evaluate the model's performance.

---

## Results

The Logistic Regression model achieved the following results:

### Classification Report

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| -1    | 0.70      | 0.81   | 0.75     | 15125   |
| 1     | 0.97      | 0.94   | 0.96     | 96663   |
| **Accuracy** | - | - | 0.93 | 111188 |
| **Macro Avg** | 0.83 | 0.88 | 0.85 | 111188 |
| **Weighted Avg** | 0.93 | 0.93 | 0.93 | 111188 |

**Explanation:**
  1. Class: Represents the sentiment classes (-1 for negative and 1 for positive).
  2. Precision, Recall, F1-Score: Metrics for each class.
  3. Support: Number of samples for each class.
  4. Accuracy, Macro Avg, Weighted Avg: Overall metrics for the model.

---

## Technologies Used

- Python: Primary programming language.
- Libraries:
  - pandas: Data manipulation and analysis.
  - numpy: Numerical computations.
  - matplotlib and seaborn: Data visualization.
  - nltk: Natural Language Processing (NLP).
  - scikit-learn: Machine learning model training and evaluation.
- Jupyter Notebook: Interactive environment for running the code.

---

## Acknowledgments

- Dataset provided by Kaggle.
- Inspired by various NLP and sentiment analysis tutorials.

---
