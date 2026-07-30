# Handwritten Digit Recognition using Artificial Neural Networks (ANN)

## Objective

The objective of this project is to develop an Artificial Neural Network (ANN) to classify handwritten digits (0–9) using the MNIST Handwritten Digits dataset. This project demonstrates the complete deep learning workflow, including data understanding, preprocessing, model development, training, evaluation, and visualization of model performance using TensorFlow/Keras.

---

## Dataset Link

**MNIST Handwritten Digits Dataset**

Kaggle: https://www.kaggle.com/datasets/oddrationale/mnist-in-csv

---

## Libraries Used

The following Python libraries were used in this project:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- TensorFlow / Keras
- Scikit-learn

Modules from TensorFlow/Keras:

- Sequential
- Dense
- to_categorical

Modules from Scikit-learn:

- train_test_split
- confusion_matrix
- classification_report

---

## Methodology

The project was completed using the following steps:

1. Loaded the MNIST dataset using Pandas.
2. Explored the dataset by displaying the first few records, dataset dimensions, and summary information.
3. Checked for missing values and separated the input features and target variable.
4. Normalized the pixel values to the range **0–1**.
5. Split the dataset into training (80%) and testing (20%) sets.
6. Converted the target labels into categorical format using **One-Hot Encoding**.
7. Built an Artificial Neural Network (ANN) with two hidden layers containing **128** and **64** neurons using ReLU activation.
8. Used a Softmax output layer with **10 neurons** for digit classification.
9. Compiled the model using the **Adam optimizer** and **Categorical Crossentropy** loss function.
10. Trained the model for **10 epochs**.
11. Evaluated the model using Test Accuracy, Confusion Matrix, and Classification Report.
12. Visualized training performance using Accuracy vs Epoch and Loss vs Epoch graphs.

---

## Model Architecture

The Artificial Neural Network consists of:

- **Input Layer:** 784 input features (28 × 28 pixels)
- **Hidden Layer 1:** 128 neurons with ReLU activation
- **Hidden Layer 2:** 64 neurons with ReLU activation
- **Output Layer:** 10 neurons with Softmax activation for multi-class classification

---

## Results

The ANN model successfully classified handwritten digits from the MNIST dataset. Model performance was evaluated using Test Accuracy, Confusion Matrix, and Classification Report. The Accuracy vs Epoch and Loss vs Epoch graphs demonstrated the learning progress of the network during training. The trained model achieved high classification performance, indicating that Artificial Neural Networks are highly effective for image recognition tasks.

---

## Conclusion

This project demonstrates the effectiveness of Artificial Neural Networks (ANNs) for handwritten digit recognition using the MNIST dataset. After preprocessing the data and training the model, the ANN successfully classified digits with high accuracy. The hidden layers enabled the network to learn complex patterns from pixel values, significantly improving prediction performance. Compared to traditional machine learning algorithms, deep learning models can automatically learn meaningful feature representations from raw data. However, one limitation of ANNs is that they require more computational resources and training time, especially when working with large datasets and deeper network architectures. Overall, the ANN provides an accurate and reliable solution for handwritten digit classification.