**# SpaceX-Launch-Prediction**
This project involves extracting SpaceX launch data, performing data cleaning and wrangling, exploratory data analysis (EDA), and building machine learning models to predict the success of future launches. The goal is to determine which machine learning model best predicts the outcome of a SpaceX launch. This is a part of IBM - Data Science project

**Project Overview**
This project aims to predict the success of SpaceX rocket launches based on various features related to the launch. It involves the following steps:
1.Data Collection: Download launch data from an API, convert JSON to a flat file, and scrape additional information using BeautifulSoup.
2.Data Wrangling: Clean and preprocess the data, including calculating mission outcomes and sorting launches by success and failure.
3.Exploratory Data Analysis (EDA): Analyze the data to identify trends, perform feature engineering, and prepare the data for machine learning.
4.Machine Learning Models: Test various machine learning algorithms and tune them to find the best model for predicting launch success.
5.Interactive Visualizations: Create interactive maps and plots to visualize the data and model predictions.

**Data Collection**
API: The primary source of data is a SpaceX launch API. Data is downloaded in JSON format, which is then flattened for easier analysis.
Web Scraping: BeautifulSoup is used to scrape additional launch-related data from websites, enhancing the dataset with external information like launch site details and mission outcomes.
The data collection process ensures the dataset is comprehensive and up-to-date, incorporating as much relevant information as possible.

**Data Wrangling**
The following data wrangling steps were performed:
Launch Outcome Calculation: A key step was determining the outcome of each launch (e.g., successful, failed, or unknown). This was achieved by analyzing available metadata and logs.
Launch Site Data: The number of launches from each launch site was calculated, with sorting performed to identify sites with the worst launch outcomes.
Handling Missing Data: Missing values were handled by filling or dropping them based on the context of the data.
Feature Engineering: New features were created for use in machine learning models, including encoding categorical variables and deriving new variables based on launch data.

**Exploratory Data Analysis (EDA)**
The EDA process focused on understanding the relationships between various features and the success of the launches:
Correlation Analysis: Identified important attributes related to launch success.
Categorical Variable Encoding: Categorical variables like launch site and mission type were encoded using one-hot encoding to prepare them for machine learning algorithms.
Feature Importance: Conducted feature importance analysis to determine which features were most predictive of launch success.

**Machine Learning Models**
To predict the success of a launch, the following machine learning algorithms were tested:
Logistic Regression
Support Vector Machine (SVM)
Decision Tree Classifier
K-Nearest Neighbors (KNN)

**The following steps were performed for each algorithm:**
Data Standardization: Features were standardized using StandardScaler to ensure uniformity across the dataset.
Train-Test Split: The data was split into training and testing sets to evaluate model performance.
Hyperparameter Tuning: Hyperparameters were optimized using Grid Search to improve model accuracy.
Model Evaluation: Models were evaluated using a confusion matrix and accuracy score to determine the best-performing algorithm.

**Interactive Visualizations**
To make the data and analysis more accessible, interactive visualizations were created:
Folium Map: A map-based visualization was created to display launch sites and outcomes using Folium. This allows users to interact with the data and gain insights into launch patterns.
Plots: Interactive plots, including bar charts, histograms, and scatter plots, were generated to explore the relationships between different variables.

**Requirements**
The following Python libraries are required to run the project:
requests (for API calls)
beautifulsoup4 (for web scraping)
pandas (for data manipulation)
numpy (for numerical operations)
matplotlib (for basic plotting)
seaborn (for statistical data visualization)
scikit-learn (for machine learning algorithms)
folium (for interactive maps)
gridsearchcv (for hyperparameter tuning)
