# Neural Network Model Card

## Model Details
- **Developer**: Raha AlAssaf
- **Model Date**: June 2, 2024
- **Model Version**: 1.0
- **Model Type**: Neural Network
- **Model Framework**: TensorFlow / Keras

## Model Description
This Neural Network model has been developed to predict customer churn in the telecommunications sector. It leverages a deep learning architecture to capture complex patterns in customer behavior and service usage, aiming to provide accurate predictions that help in retaining customers.

**Input:** 
The model inputs consist of several features derived from customer data, including demographics, account information, and usage details, all numerically encoded or normalized to fit the model requirements.

**Output:** 
The model outputs a probability score indicating the likelihood of a customer churning, which is then converted to a binary outcome (1 for churn, 0 for no churn).

**Model Architecture:** 
The model uses a fully connected deep neural network architecture comprising multiple layers. Specifically, it includes:
- Input layer
- Several hidden layers with ReLU activation functions to introduce non-linearity
- Dropout layers to prevent overfitting
- Output layer with sigmoid activation function to produce a probability score

## Intended Use
- **Primary Use**: Predicting churn among customers of a telecom service provider.
- **Users**: Data science teams in telecom companies tasked with improving customer retention strategies.

## Training Data
- **Source**: The model was trained on the Telco Customer Churn dataset.
- **Type**: The dataset comprises customer demographics, account details, service usage, and churn labels.
- **Preprocessing**: Data preprocessing included normalization of numerical features, one-hot encoding of categorical variables, and handling of missing values.

## Evaluation Data
- **Source**: Same as training data, split into training and validation sets.
- **Preprocessing**: The evaluation data underwent the same preprocessing steps as the training data to ensure consistency in model evaluation.

## Performance
The performance of the Neural Network model is evaluated based on accuracy, precision, recall, F1-score, and the area under the ROC curve. The model was tested using a hold-out validation set after training on a large portion of the Telco Customer Churn dataset.

**Performance Metrics:**
- **Accuracy**: 79%
- **Precision**: 61%
- **Recall**: 56%
- **F1-Score**: 58%
- **AUC-ROC**: 83%

![Performance Graph](results/NN_performance_graph.png) 

## Limitations
- The model's performance may degrade if applied to customer data significantly different in distribution from the training dataset.
- The deep learning architecture requires a large amount of data to train effectively, which might not be feasible in all real-world scenarios.

## Trade-offs
- The model tends to prioritize minimizing false negatives at the cost of increasing false positives, which might not be ideal in scenarios where falsely predicting churn can lead to unnecessary retention costs.
- The complexity of the neural network results in longer training times compared to simpler models like logistic regression, which might be a consideration in environments where model training speed is a critical factor.

## Ethical Considerations
- **Potential Bias**: Efforts were made to identify and mitigate any bias in the training data. The model's performance was evaluated to ensure fairness across various customer segments.
- **Mitigation Strategies**: Techniques such as adjusting class weights and resampling were explored to address imbalance and potential bias.

## Caveats and Recommendations
- Model Limitations: While neural networks can model complex relationships, they require large amounts of data and can overfit if not properly regularized or if trained on unrepresentative data sets.
- Operational Use: Recommended continuous monitoring of the model's performance over time with new data, and regular updates to the model architecture or training data as needed.





