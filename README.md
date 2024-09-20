# Transaction-fraud-detection-model

Summary of the Fraud Detection Model

Model Overview:
he model is designed to detect fraudulent transactions in a credit card dataset. It is a neural network built using TensorFlow and Keras, which leverages multiple dense (fully connected) layers with ReLU activations and dropout layers to prevent overfitting. The final layer uses a sigmoid activation function to output a probability score between 0 and 1, indicating the likelihood of a transaction being fraudulent. The model is trained using binary cross-entropy loss and the Adam optimizer.


The dataset used is the Credit Card Fraud Detection dataset, available on Kaggle. It contains transactions made by credit cards in September 2013 by European cardholders. The dataset includes:

-Time: The seconds elapsed between this transaction and the first transaction in the dataset.

-V1 to V28: The principal components obtained with PCA (Principal Component Analysis), which are anonymized features that have been transformed to protect sensitive information.

-Amount: The transaction amount.

-Class: The target variable, where 1 indicates a fraudulent transaction and 0 indicates a legitimate transaction.


Data Characteristics:

-Imbalanced Dataset: The dataset is highly imbalanced, with fraudulent transactions constituting a very small fraction of the total transactions. This characteristic requires careful handling during model evaluation and training to avoid biased results.

-Preprocessing Steps: The data preprocessing includes separating features and the target variable, splitting the data into training, validation, and test sets, and normalizing the features using StandardScaler to ensure all features contribute equally to the model.


Model Evaluation metrics:

-Confusion Matrix: Shows true positives, true negatives, false positives, and false negatives, giving a clear picture of the model's performance.

-Precision and Recall: Precision indicates how many of the predicted frauds were actual frauds, while recall indicates how many of the actual frauds were correctly identified by the model.

-F1-Score: The harmonic mean of precision and recall, providing a balance between the two.

-ROC-AUC Score: Measures the area under the receiver operating characteristic curve, summarizing the model's ability to distinguish between the classes at various thresholds.

These metrics help in understanding the model's effectiveness in identifying fraudulent transactions while minimizing false positives and false negatives.

