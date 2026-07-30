# Image Classification using Convolutional Neural Networks (CNN)

## Objective

The objective of this project is to develop a Convolutional Neural Network (CNN) to classify images of cats and dogs. This project demonstrates the complete deep learning workflow, including image preprocessing, data generation, CNN model development, training, evaluation, and visualization of model performance using TensorFlow/Keras.

---

## Dataset Link

**Cats vs Dogs Dataset**

Kaggle: https://www.kaggle.com/datasets/bhavikjikadara/dog-and-cat-classification-dataset

---

## Libraries Used

The following Python libraries were used in this project:

- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

Modules from TensorFlow/Keras:

- ImageDataGenerator
- Sequential
- Conv2D
- MaxPooling2D
- Flatten
- Dense

Modules from Scikit-learn:

- confusion_matrix
- precision_score
- recall_score
- f1_score

---

## Methodology

The project was completed using the following steps:

1. Loaded the Cats vs Dogs image dataset.
2. Displayed the dataset folder structure and sample images.
3. Resized all images to **128 × 128** pixels.
4. Normalized pixel values to the range **0–1**.
5. Split the dataset into **80% training** and **20% testing**.
6. Created image data generators using TensorFlow/Keras.
7. Built a Convolutional Neural Network (CNN) with three convolutional layers followed by max-pooling layers, a flatten layer, and dense layers.
8. Compiled the model using the **Adam optimizer**, **Binary Crossentropy** loss function, and **Accuracy** metric.
9. Trained the model for **10 epochs**.
10. Evaluated the model using Test Accuracy, Precision, Recall, F1-Score, and a Confusion Matrix.
11. Visualized model performance using Accuracy vs Epoch and Loss vs Epoch graphs.

---

## CNN Architecture

The CNN model consists of:

- **Conv2D:** 32 filters (3×3), ReLU
- **MaxPooling2D:** 2×2
- **Conv2D:** 64 filters (3×3), ReLU
- **MaxPooling2D:** 2×2
- **Conv2D:** 128 filters (3×3), ReLU
- **MaxPooling2D:** 2×2
- **Flatten Layer**
- **Dense Layer:** 128 neurons, ReLU
- **Output Layer:** 1 neuron with Sigmoid activation

---

## Results

The CNN model successfully classified images into **Cat** and **Dog** categories. Model performance was evaluated using Test Accuracy, Precision, Recall, F1-Score, and a Confusion Matrix. The Accuracy vs Epoch and Loss vs Epoch graphs illustrated the learning progress during training. The trained CNN achieved strong classification performance, demonstrating its effectiveness for image recognition tasks.

---

## Conclusion

This project demonstrates the effectiveness of Convolutional Neural Networks (CNNs) for image classification using the Cats vs Dogs dataset. By combining convolutional and pooling layers, the model automatically learned important visual features while reducing the dimensionality of the input images. CNNs provide a significant advantage over traditional Artificial Neural Networks for image classification because they efficiently capture spatial patterns and local features. However, one limitation of CNNs is that they require large labeled datasets and considerable computational resources for effective training. Overall, the CNN model provides an accurate and reliable solution for binary image classification tasks.