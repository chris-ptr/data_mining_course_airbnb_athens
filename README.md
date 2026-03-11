# Data Mining University Project: Airbnb Athens Analysis

This project analyzes Airbnb listing and review data from Athens, Greece, comparing the years **2019** and **2023**. It was developed as part of the **Data Mining** course in the **Department of Informatics and Telecommunications (DIT)** at the **National and Kapodistrian University of Athens (NKUA/UoA)**.

## Team Members
* **Christos Petropoulos** sdi2100156)
* **Marina Papadimitriou** (sdi2100136)

## Project Overview

The project is structured into two main phases, each focusing on different data mining techniques, from initial preprocessing to advanced sentiment analysis and machine learning.

### [Exercise 1: Data Exploratory Analysis & Preprocessing](./ex1/)
Focuses on cleaning the raw data and performing initial exploratory analysis to understand the Airbnb landscape in Athens.

*   **Notebook:** `exercise_1_notebook.ipynb`
*   **Key Tasks:**
    *   **Data Manipulation:** Handling missing values, removing outliers using the Interquartile Range (IQR) method, and converting currency strings to numerical data.
    *   **Time Feature Engineering:** Extracting and aggregating data by month (e.g., February, March, April for 2019; March, June, September for 2023).
    *   **Price Trend Analysis:** Visualizing average price trends across different months and property types.
    *   **Geospatial Visualization:** Creating interactive property maps using `Folium`.
    *   **Text Analysis (Word Clouds):** Generating word clouds from listing descriptions to identify common themes for each year.
    *   **Amenities Simplification:** Categorizing raw amenity strings into simplified groups (e.g., "Kitchen", "Essentials", "Electronics") and analyzing their distribution.
    *   **Neighborhood Analysis:** Comparing listing counts and average prices across different Athens neighborhoods.
    *   **Room Type Analysis:** Investigating the distribution and pricing of different room types (Entire home/apt, Private room, etc.).

### [Exercise 2: Sentiment Analysis & Machine Learning](./ex2/)
An advanced study focusing on natural language processing (NLP) of user reviews and predictive modeling.

*   **Notebooks:** 
    *   `exercise_2_notebook_d2019.ipynb`
    *   `exercise_2_notebook_d2023.ipynb`
*   **Key Tasks:**
    *   **Sentiment Analysis:** Using the **VADER** Sentiment Analysis tool and custom sentiment pipelines to classify reviews (Positive, Negative, Neutral).
    *   **Review Preprocessing:** Handling long reviews through chunking/truncation, removing emojis, and detecting review languages using `langdetect`.
    *   **Feature Engineering:**
        *   **TF-IDF:** Extracting text features using Term Frequency-Inverse Document Frequency.
        *   **Word2Vec:** Training custom Word2Vec models to create word embeddings.
        *   **GloVe:** Utilizing pre-trained GloVe vectors for similarity analysis.
    *   **Machine Learning Classifiers:**
        *   Training and evaluating **SVM (Support Vector Machines)**, **Random Forest**, and **K-Nearest Neighbors (KNN)**.
        *   Implementing **Cross-Validation** to ensure model robustness.
    *   **Word Similarity & Neighborhoods:** Analyzing the impact of neighborhood size (N) on word similarity metrics and finding the most similar words in the review context.

## Requirements

The project is built using Python 3.10+. The following libraries are required:

| Library | Purpose |
| :--- | :--- |
| `pandas` | Data manipulation and analysis |
| `numpy` | Numerical computations |
| `matplotlib` / `seaborn` | Data visualization |
| `nltk` | Natural Language Toolkit for text processing |
| `wordcloud` | Generating word clouds |
| `folium` | Interactive maps |
| `langdetect` | Language detection for reviews |
| `vaderSentiment` | Sentiment analysis |
| `scikit-learn` | Machine learning models and evaluation |
| `gensim` | Word2Vec and embedding management |

