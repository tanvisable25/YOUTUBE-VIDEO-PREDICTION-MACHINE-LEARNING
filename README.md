
YouTube Video Performance Prediction using Machine Learning
Project Overview

This project predicts YouTube video views using machine learning.
The model analyzes engagement features such as likes, dislikes, comments, video category, and upload time to estimate how many views a video might receive.

The project demonstrates data analysis, visualization, and predictive modeling using Python.

Dataset

The dataset contains information about YouTube videos including engagement metrics and video categories.

Column	Description
categoryId	Numeric ID representing video category
Category_Name	Human-readable category name
publish_hour	Hour when the video was uploaded
likes	Number of likes
dislikes	Number of dislikes
comment_count	Number of comments
views	Total views (target variable)

Example dataset structure:

categoryId	Category_Name	publish_hour	likes	dislikes	comment_count	views
10	Music	14	52000	2000	1500	500000
20	Gaming	18	83000	1500	3200	900000
Technologies Used

Python

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

Project Workflow

The project follows a standard machine learning pipeline.

1 Data Collection

Load dataset from CSV file.

2 Data Exploration

Understand the dataset using:

head()

info()

describe()

3 Data Visualization

Analyze relationships between variables using:

category distribution charts

correlation heatmap

4 Feature Selection

Separate input features and target variable.

Features:

categoryId

publish_hour

likes

dislikes

comment_count

Target:

views

5 Train-Test Split

Split dataset into training and testing sets:

80% training data

20% testing data

6 Model Training

Train a Linear Regression model to learn relationships between engagement metrics and video views.

7 Model Prediction

Use the trained model to predict views for unseen data.

8 Model Evaluation

Evaluate performance using R² Score.

9 Visualization

Compare actual vs predicted views using scatter plots.

Example Visualizations
Category Distribution

Shows how many videos belong to each category.

Correlation Heatmap

Displays relationships between features such as likes, comments, and views.

Prediction Visualization

Scatter plot comparing predicted views with actual views.

Machine Learning Model

Model used in this project:

Linear Regression

Linear regression estimates the relationship between input features and the target variable using a linear equation.

Goal:

Predict YouTube video views based on engagement metrics.

Project Structure
YouTube-Performance-Prediction
│
├── youtube_performance_dataset.csv
├── youtube_prediction.ipynb
├── README.md
Results

The model predicts YouTube video views using engagement metrics such as likes, dislikes, and comments.

Evaluation metric used:

R² Score

Higher values indicate better predictive performance.

Future Improvements

Possible improvements for this project:

Use more advanced models such as Random Forest or XGBoost

Include additional features like subscriber count or video duration

Build a dashboard for video performance analysis

Deploy the model as a web application
