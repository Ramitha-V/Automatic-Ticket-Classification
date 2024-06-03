# Automatic-Ticket-Classification
The Automatic Ticket Classification project aims to automate the process of classifying customer complaint tickets in a financial institution. By leveraging machine learning techniques, this project ensures that customer complaints are efficiently categorized and assigned to the relevant departments, leading to quicker issue resolution and cost reduction. This project uses a Flask-based web application for user interaction.

## Introduction
Introduction
Financial institutions receive a high volume of customer complaint tickets. Manually categorizing and routing these tickets is time-consuming and resource-intensive. Automating this process can lead to:

- Reduced effort for support employees.
- Quick resolution of customer issues.
- Cost reduction through decreased operational expenses.
- Increased profit margins by optimizing resource allocation.

## Data Preprocessing
To prepare the data for modeling, the following preprocessing steps were performed:

- Dropping Unnecessary Columns: Columns that do not contribute to the classification task were removed.
- Handling Null Values: Null values in relevant columns were dropped.
- Text Normalization: All characters were converted to lowercase.
- Expanding Contractions: Common contractions were expanded for consistency.
- Removing Punctuations: Punctuations and text enclosed within square brackets were removed.
- Stopwords Removal: Common stopwords were removed to reduce noise.
- Lemmatization: Words were lemmatized to their base forms.
- POS Tagging: Parts of speech tagging for adjectives and nouns was performed.
- TF-IDF Vectorization: The text was vectorized using the TF-IDF method.

## Topic Modelling
Topic modeling helps in automatically categorizing and organizing text documents into coherent topics. Latent Dirichlet Allocation (LDA) was used for topic modeling, identifying five major topics:

- Loans and Mortgages
- Account Services
- Credit and Prepaid Cards
- Theft and Fraud Reports
- Bookings and Refunds

## Classification Models
Five classification models were implemented:

- K-Nearest Neighbors (KNN)
- Naive Bayes
- Logistic Regression
- Random Forest
- Decision Tree
From the performance evaluation, Logistic Regression emerged as the best-suited model with the highest F1-score (0.89).

## Deployment
The project includes a Flask-based web application consisting of two webpages:

- Customer Query Submission: A webpage where customers can submit their complaints.
- Ticket Categorization: A webpage where tickets are categorized into relevant topics, facilitating efficient resolution by employees.

<img width="427" alt="Screenshot 2024-06-03 101706" src="https://github.com/Ramitha-V/Automatic-Ticket-Classification/assets/162662008/a096abbf-deb5-4dd8-b2d9-ec15c8f687a3"> <img width="430" alt="Screenshot 2024-06-03 101821" src="https://github.com/Ramitha-V/Automatic-Ticket-Classification/assets/162662008/3eb10049-d16e-4cc6-9501-6d5b0783c5cb">

