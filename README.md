## Customer Churn Prediction using Machine Learning

This repository contains machine learning models developed for predicting customer churn in a telecommunications company. The goal of these models is to identify customers likely to churn so that proactive strategies can be employed to retain them. Using the Telco Customer Churn dataset, the project explores various machine learning techniques, with a special focus on Bayesian optimization for hyperparameter tuning. This project includes detailed Jupyter notebooks for each step of the process—from data preprocessing and exploratory data analysis to model training and evaluation. The goal is to develop a predictive model that can help businesses understand and mitigate customer churn, ultimately enhancing customer retention strategies. Whether you're a data science student, a professional looking to understand churn prediction, or someone interested in machine learning applications, this repository provides a comprehensive guide and all necessary tools for replication and further exploration.

### Components of the Repository:

Data: Original dataset and preprocessed data files.

Notebooks: Step-by-step Jupyter notebooks covering data preprocessing, exploratory data analysis, feature engineering, model training, hyperparameter tuning using Bayesian optimization, and model evaluation.

Scripts: Python scripts for more modular or production-ready code.

Model Card and Datasheet: Documentation providing details on model performance, usage, and dataset characteristics.

Results: Visualizations and output files showcasing the analysis and outcomes of the models.

### Data
The dataset used in this project is the Telco Customer Churn dataset. It can be found in the `data/` directory. This dataset includes customer data from a telecom company, where the main goal is to predict customer churn based on various features like monthly charges, tenure, and service type.

### Models

#### Random Forest
- **Description**: Utilizes ensemble learning technique for classification. Random Forest is robust against overfitting as it uses multiple decision trees to make predictions.
- **Performance**: Details about the accuracy, precision, recall, and F1-score are documented in the Random Forest model card.

#### Logistic Regression
- **Description**: A statistical model that estimates the probability of a binary outcome based on input features. It is useful for understanding the influence of several independent variables on a binary outcome.
- **Performance**: Metrics and evaluation are available in the Logistic Regression model card.

#### Neural Network
- **Description**: Employs a deep learning architecture to model complex relationships in data. The model used here is a fully connected deep neural network, structured to capture intricate patterns in customer behavior.
- **Performance**: Evaluation results can be found in the Neural Network model card.

### Model Cards

Model cards for each algorithm are included in this repository to provide insights into model performance, usage, and limitations.

- [Random Forest Model Card] Random Forest Model Card
- [Logistic Regression Model Card](Logistic_Regression_Model_Card.md)
- [Neural Network Model Card](Neural_Network_Model_Card.md)

### Setup and Usage
Instructions on how to set up and run these models are provided for each model within their respective directories.

### Contributing
Contributions to improve the models or approaches are welcome. Please refer to the contribution guidelines for more details on how to contribute.

### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

