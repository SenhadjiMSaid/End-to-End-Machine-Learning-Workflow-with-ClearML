# IMDb Sentiment Analysis with ClearML

## **Overview**

This project performs sentiment analysis on the IMDb Movie Reviews dataset, classifying reviews as positive or negative. The project leverages ClearML for experiment tracking, comparison, and logging, providing a seamless platform for managing machine learning workflows.

## Project Objectives

1. Analyze and preprocess the IMDb dataset.
2. Train and evaluate machine learning models for sentiment classification.
3. Track experiments, visualize results, and compare model performance using ClearML.

---

## Features

- **Experiment Tracking**: Automatically logs metrics, hyperparameters, and artifacts to ClearML.
- **Model Comparison**: Evaluate and compare the performance of Logistic Regression and Naive Bayes classifiers.
- **Dataset Preprocessing**: Converts text reviews into numerical features using TF-IDF.
- **Reproducibility**: ClearML ensures all experiments are fully reproducible.

Project Structure

```graphql
IMDb-Sentiment-Analysis/
├── dataset/                     # Contains the IMDb dataset
│   └── imdb_reviews.csv         # Dataset file
├── notebook/                    # Contains the Jupyter Notebook
│   └── imdb_sentiment_analysis_with_clearml.ipynb
├── README.md                    # Project documentation
└── requirements.txt             # Required Python libraries

```

## Setup Instructions

### 1. Clone the Repository

```bash
git clone git@github.com:SenhadjiMSaid/End-to-End-Machine-Learning-Workflow-with-ClearML.git

git cd imdb-sentiment-analysis-clearml

```

### 2. Install Dependencies

Install the required Python libraries using `pip`:

```bash
pip install -r requirements.txt
```

### 3. Install ClearML

```bash
pip install clearml
clearml-init
```

### 4. Dataset

Download the IMDb Movie Reviews dataset and place it in the `dataset/` folder:

- [IMDb Dataset Source](https://www.kaggle.com/datasets/rajugc/imdb-top-250-movies-dataset)

## Usage

### 1. Open the Jupyter Notebook

```bash
jupyter notebook notebook/imdb_sentiment_analysis_with_clearml.ipynb

```

### 2. Follow the Workflow

- **Step 1**: Load and explore the dataset.
- **Step 2**: Preprocess the text data using TF-IDF.
- **Step 3**: Train and evaluate models (Logistic Regression and Naive Bayes).
- **Step 4**: Track experiments and log results using ClearML.

### 3. View Results on ClearML Dashboard

Visit [ClearML Dashboard](link) to view and analyze logged experiments.

## Results

**Model Performance**:

| Model               | Accuracy | Precision | Recall | F1 Score |
| ------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression | ---      | ---       | ---    | ---      |
| Random Forest       | ---      | ---       | ---    | ---      |
| ---                 | ---      | ---       | ---    | ---      |

**Future Enhancements**:

1. Integrate additional models like Naive Bayes or Neural Networks.
2. Automate the pipeline using ClearML Agents.
3. Deploy the best-performing model using ClearML Serving.
