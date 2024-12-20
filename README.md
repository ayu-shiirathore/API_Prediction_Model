# API Prediction Model

## Project Overview:
This project focuses on predicting the number of API calls within a user-defined time span based on historical API call data. The model leverages machine learning techniques to predict future API call frequencies, assisting in understanding API usage patterns. By using various regression models and preprocessing techniques, it aims to provide accurate predictions for API usage.

## Key Features:

- **Data Preprocessing**: The project includes methods for preparing the data, such as:
  - Converting timestamps into usable features (hours, minutes).
  - Calculating the time difference between API calls to generate the "time since last call."
  - Handling missing data and transforming the data for better model performance.

- **Clustering Algorithms**: Uses clustering techniques such as:
  - **K-Means**: To identify patterns in API usage.
  - **Hierarchical Clustering**: To find hierarchical relationships in the data.
  - **MeanShift**: To detect clusters of varying densities.

- **Model Training**: Multiple regression models are trained and evaluated:
  - **Random Forest Regressor**
  - **Gradient Boosting Regressor**
  - **Linear Regression**
  - **Decision Tree Regressor**
  - **Support Vector Regressor (SVR)**
  
  These models predict the number of API calls in the next user-defined time span (in minutes).

- **Time Span Prediction**: The user can input a time span (in minutes), and the model predicts how many API calls will occur within that period.

## Getting Started:

### Prerequisites:
To run this project, you will need to install the following Python libraries:

- `pandas`
- `scikit-learn`
- `openpyxl`

You can install these libraries using pip:

```bash
pip install pandas scikit-learn openpyxl
