### Hotel Recommendation System Readme

This code implements a hotel recommendation system based on user descriptions and hotel tags. Here's a guide to understand and use this code:

#### 1. Introduction

This project aims to recommend hotels based on user descriptions and hotel tags. It preprocesses user descriptions, identifies relevant hotels in a specified location, and recommends hotels with the highest similarity to the description and the highest average score.

#### 2. Dataset

The dataset used in this project is the [Hotel Reviews dataset](https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe) available on Kaggle. It contains hotel reviews data in Europe.

#### 3. Installation

Before running the code, make sure you have installed the following Python libraries:

- nltk
- numpy
- pandas

You can install these libraries using pip:

```
pip install nltk numpy pandas
```

#### 4. Preprocessing

The code preprocesses the dataset by:
- Tokenizing user descriptions and hotel tags
- Removing stopwords
- Lemmatizing tokens

#### 5. Functionality

The code provides two functions for hotel recommendation:

- `recommend_hotel(location, description)`: This function preprocesses the description and finds the most relevant hotels in the specified location by comparing the description to the hotels' tags. It recommends hotels with the highest similarity to the description and the highest average score.

#### 6. Usage

To use the hotel recommendation system, call `recommend_hotel()` function with the location and description as arguments. For example:

```python
recommend_hotel('France', 'I am going for a business trip to a city center with good conference facilities')
recommend_hotel('UK', 'I need an affordable hotel with basic amenities for a budget-friendly stay')
recommend_hotel('Netherlands', 'I am going for a holiday, I need a suite room for 1 month near a beach')
```

#### 7. Note

Make sure to replace the dataset file path (`Hotel_Reviews.csv`) with the appropriate file path in your system before running the code.