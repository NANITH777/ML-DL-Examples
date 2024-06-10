# Email Spam Detection Model

This project aims to develop a machine learning model to classify emails as spam or non-spam (ham). The model utilizes the Multinomial Naive Bayes algorithm for classification.

## Dataset

The dataset used in this project is stored in the `emails.csv` file. It contains labeled emails with two columns: `text` (the content of the email) and `spam` (binary label indicating whether the email is spam or not).

### Exploratory Data Analysis (EDA)

- Load the dataset using Pandas and explore its structure and summary statistics.
- Check for missing values and duplicate entries, and handle them accordingly.
- Analyze the distribution of spam and non-spam emails in the dataset.

## Data Preprocessing

- Download the NLTK stopwords package to filter out common stopwords from the text data.
- Define a preprocessing function to clean and transform the text data by removing punctuation and stopwords.

## Feature Engineering

- Tokenize the text data and convert it into a matrix of token counts using the CountVectorizer from scikit-learn.
- Split the data into training and testing sets using the train_test_split function.

## Model Training

- Create an instance of the Multinomial Naive Bayes classifier.
- Train the classifier on the training data using the fit method.

## Model Evaluation

- Make predictions on the training and testing sets using the predict method.
- Calculate the accuracy of the model using accuracy_score from scikit-learn.
- Generate a classification report and confusion matrix to evaluate the model's performance.

## Results

The trained model achieves an accuracy of `99,03%` on the test set. The classification report provides precision, recall, F1-score, and support for both spam and non-spam classes. The confusion matrix visualizes the true positive, true negative, false positive, and false negative predictions made by the model.