# Exploratory Data Analysis (EDA) - Falcon 9 Landing Prediction

## Overview

This README outlines the key aspects of the Exploratory Data Analysis (EDA) performed as part of a data science project focusing on Falcon 9 first-stage landing prediction. EDA is a critical initial step in any data science project, allowing us to gain insights into the dataset and identify patterns and relationships that can be leveraged for analysis and prediction.


#### Key Observations and Features:

- **Improvement in Success Rate:** The success rate of Falcon 9 landings has shown improvement since 2013, indicating progress in SpaceX's capabilities.

- **Launch Number as a Feature:** We incorporate the launch number as a feature, recognizing that success rates may be influenced by historical launch data.

- **Launch Site Impact:** Different launch sites have varying success rates. For example, CCAFS LC-40 has a success rate of 60%, while KSC LC-39A and VAFB SLC 4E have a success rate of around 77%. Launch site information can be valuable in predicting landing outcomes.

- **Mass as a Predictor:** Mass plays a role in landing success. When the payload mass is above 10,000 kg, the success rate is 100%. This suggests that payload mass can be a significant predictor.

- **Feature Combination:** Combining multiple features enhances our understanding and predictive capabilities. For instance, combining launch site information and payload mass can provide valuable insights.

### Data Preparation

We determine which attributes are correlated with successful landings and prepare the data for machine learning. Categorical variables will be converted using one-hot encoding, ensuring that the data is suitable for building machine learning models that predict the success of the first stage landing.

## Future Analysis

With the insights gained from EDA and data preparation, we are well-equipped to develop machine learning models that can automatically predict the outcome of Falcon 9 first stage landings. This predictive capability can be invaluable for mission planning and decision-making.

## Technologies Used

- Python
- Pandas for data manipulation
- Matplotlib and Seaborn for data visualization
- Machine learning libraries for model development (not covered in this README)

## Author

Aflah Al Abri

## License

This project is licensed under the [MIT License](LICENSE.md).
