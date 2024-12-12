# Hoax_Detection_using_SVM
Detection and Analysis for Hoax News on Instagram in Indonesia using Support Vector Machine Methods
This project focuses on identifying and analyzing hoax news on Instagram within the Indonesian context. Using Support Vector Machine (SVM) methods, the system is designed to classify and evaluate content, assisting users in distinguishing between genuine and misleading information.

Table of Contents
Overview
Features
Technologies Used
Dataset
Methodology
Results

Overview
Hoax news has become a widespread issue in Indonesia, especially on social media platforms like Instagram. This project leverages machine learning techniques, specifically the Support Vector Machine (SVM) algorithm, to classify news content and identify potential hoaxes. The aim is to help combat misinformation and promote digital literacy.

Features
Data Preprocessing: Cleans and preprocesses Instagram post data, including text extraction and normalization.
Classification: Uses SVM to classify posts as genuine or hoax.
Visualization: Provides analytical insights through graphs and charts.
Localization: Tailored specifically for Indonesian language and culture.
Technologies Used

Programming Language: Python

Libraries:
scikit-learn (for SVM implementation)
pandas and numpy (for data manipulation)
matplotlib and seaborn (for data visualization)

Platform: Instagram API for data retrieval

Dataset
The dataset consists of 4,231 labeled Instagram posts in Indonesian, categorized as either hoax or genuine. 
It includes:
Textual content
Metadata (e.g., hashtags, user engagement metrics)
Note: The dataset used was sourced from Kaggle and includes two labels: hoax news (1) and real news (0). 

Dataset Details
Real news: 766 posts
Hoax news: 3,465 posts
The dataset is imbalanced, which required preprocessing to balance the training data for improved model reliability.

Methodology
Data Preprocessing:
Converted text to lowercase.
Applied stemming to reduce words to their root forms.
Tokenized text into individual words.
Balanced the dataset by randomizing entries labeled as hoax and merging them with real news entries, ensuring a more even distribution.

Model Training:
Used the Support Vector Machine (SVM) algorithm with a linear kernel and specific parameters (C=1.0, gamma="auto").
Split data into 70% training and 30% testing sets.

Evaluation:
Measured accuracy using test data.
Analyzed results to improve future iterations.

Results
The SVM model achieved an accuracy of 54.61%.
This indicates the model's moderate success in distinguishing between hoax and genuine news but highlights the need for further optimization.
Despite the limitations, this result demonstrates the potential of SVM in combating misinformation on Instagram in Indonesia.

Key Challenges and Future Directions
Imbalanced dataset: Future research should explore advanced preprocessing techniques or alternative algorithms like Random Forest or Neural Networks.
Feature expansion: Incorporating visual data and user behavior analysis could improve accuracy.
