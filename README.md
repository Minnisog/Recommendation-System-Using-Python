# Movie Recommendation System

This project implements a movie recommendation system using a content-based filtering approach. The system suggests similar movies based on the content of the movies, including their overview, genres, keywords, cast, and crew.

## Table of Contents
- [Introduction](#introduction)
- [How it Works](#how-it-works)
- [Setup](#setup)
- [Usage](#usage)
- [Example](#example)
- [Credits](#credits)

## Introduction

A movie recommendation system, also known as a movie recommender system, predicts or filters users' film preferences based on their prior decisions and actions. This system uses machine learning algorithms to recommend movies similar to those the user has liked or interacted with before.

## How it Works

The recommendation system implemented in this project primarily uses content-based filtering. Here's an overview of how it works:

1. **Data Collection and Preprocessing**:
   - Load movie data from CSV files.
   - Merge data and select relevant columns.
   - Process features like genres, keywords, cast, and crew to make them usable.

2. **Feature Engineering**:
   - Combine multiple features into a single 'tags' column.
   - Convert text to lowercase and apply lemmatization.
   - Use CountVectorizer to convert text into numerical vectors.

3. **Similarity Calculation**:
   - Calculate cosine similarity between movie vectors.

4. **Recommendation**:
   - Define a function to recommend similar movies based on cosine similarity scores.

## Setup

To run this project, follow these steps:

1. Clone this repository:


2. Install the required libraries:


3. Download NLTK data:

```python
import nltk
nltk.download('wordnet')
```

Here's a simple example of how to use the recommendation system:
```python
recommend('Avatar')
```

Output:
``` python
Guardians of the Galaxy
Star Trek Beyond
Aliens
Star Trek Into Darkness
Guardians of the Galaxy Vol. 2
```

This project was created by Ebube Imoh. It is based on the concepts of content-based recommendation systems and uses data from https://drive.google.com/drive/folders/10P7C-suaBAA5_ZAi4oEO_Pmsb7kG6JMZ?usp=sharing.
