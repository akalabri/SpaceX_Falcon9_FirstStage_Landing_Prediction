# SpaceX Data Analysis and Predictive Modeling

## Overview

This README provides an overview of the data collection, wrangling, analysis, and predictive modeling tasks performed in this project. We explore SpaceX launch data, build interactive visual analytics tools, and create machine learning models for predicting Falcon 9 landing success.

## Data Collection and Wrangling

- **Data Sources:** We collect data from multiple sources, including the SpaceX REST API and web scraping of relevant Wiki pages. This data includes launch records, Falcon 9 launch details, and geographical information.

- **Data Transformation and Wrangling:** We perform data preprocessing and cleaning, including handling null values, filtering Falcon 1 launches, and preparing data for analysis. This step ensures data consistency and readiness for modeling.

## Interactive Visual Analytics and Dashboard

- **Interactive Map with Folium:** We use Folium to create an interactive map showcasing launch site locations and their proximities. This map aids in selecting optimal launch sites.

- **Dashboard Application with Plotly Dash:** We build a dynamic dashboard with Plotly Dash, featuring interactive components like dropdown lists and range sliders. The dashboard offers real-time data exploration and visualization.

## Predictive Analysis

- **Machine Learning Pipeline:** We construct a machine learning pipeline to predict the success of the Falcon 9 first stage landing. The pipeline includes preprocessing, train-test split, model training, grid search for hyperparameter tuning, model evaluation, testing, and confusion matrix output.

- **Considered Models:** Our analysis explores the predictive capabilities of multiple models, including Logistic Regression, Support Vector Machines, Decision Tree Classifier, and K-Nearest Neighbors.

## Future Exploration

The project lays the foundation for future exploration and analysis, including model refinement, feature engineering, and advanced machine learning techniques. We aim to improve predictive accuracy and gain deeper insights into Falcon 9 landing outcomes.

## Technologies Used

- Python for data collection, preprocessing, analysis, visualization, and machine learning
- Scikit-learn, Folium, and Plotly Dash for interactive tools and models
- SpaceX datasets (not included in this README)

## Author

Aflah Al Abri

## License

This project is licensed under the [MIT License](LICENSE.md).
