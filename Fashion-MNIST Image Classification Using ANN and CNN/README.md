# Fashion-MNIST Image Classification Using ANN and CNN

## 📌 Overview

This project implements and compares three deep learning architectures—Artificial Neural Network (ANN), Basic Convolutional Neural Network (CNN), and Deeper CNN—to classify images from the Fashion-MNIST dataset using TensorFlow and Keras.

The project explores how different neural network architectures perform on image classification and uses evaluation metrics and visualizations to analyze their results.

## 🎯 Objectives

- Understand and implement ANN and CNN architectures.
- Preprocess image data for deep learning.
- Compare different neural network architectures.
- Evaluate model performance using accuracy, loss curves, and confusion matrices.
- Apply early stopping and model checkpointing during training.

## 📊 Dataset

**Fashion-MNIST** is a dataset of grayscale images representing clothing items.

- **Training images:** 60,000
- **Testing images:** 10,000
- **Image dimensions:** 28 × 28 pixels
- **Number of classes:** 10
- **Image format:** Grayscale

The dataset contains categories such as T-shirts, trousers, pullovers, dresses, coats, sandals, shirts, sneakers, bags, and ankle boots.

## 🛠️ Technologies and Skills

- Python
- TensorFlow and Keras
- Artificial Neural Networks (ANN)
- Convolutional Neural Networks (CNN)
- NumPy and Pandas
- Matplotlib, Seaborn, and Plotly
- Image preprocessing
- Deep learning model evaluation

## ⚙️ Project Workflow

### 1. Data Preprocessing

- Loaded the Fashion-MNIST dataset using Keras.
- Normalized pixel values from the range 0–255 to 0–1.
- Reshaped images to include the channel dimension required by CNNs.
- Applied one-hot encoding to the class labels.

### 2. Artificial Neural Network (ANN)

Built a fully connected neural network consisting of:
- Flatten layer to convert images into a one-dimensional vector.
- Dense layers with ReLU activation.
- Output layer with 10 neurons and Softmax activation.

### 3. Basic Convolutional Neural Network (CNN)

Implemented a CNN using:
- Convolutional layers to extract image features.
- Max-pooling layers to reduce spatial dimensions.
- Fully connected layers for classification.
- Softmax output layer to predict one of the 10 classes.

### 4. Deeper CNN

Developed a deeper architecture incorporating:
- Multiple convolutional layers.
- Batch normalization.
- Max pooling.
- Dropout for regularization.
- Dense layers for final classification.

### 5. Model Training

- Used the Adam optimizer.
- Applied categorical cross-entropy as the loss function.
- Monitored accuracy and loss during training.
- Implemented early stopping to stop training when validation performance stopped improving.
- Used model checkpointing to save model weights based on validation loss.

### 6. Model Evaluation

Compared the models using:
- Classification accuracy.
- Test loss.
- Confusion matrices.
- Training and validation accuracy curves.
- Training and validation loss curves.

Also visualized correctly and incorrectly classified images to understand model predictions.

## 📈 Results and Observations

The project compares ANN, Basic CNN, and Deeper CNN architectures to examine their classification performance.

The Basic CNN was identified as the best-performing model in the original project analysis. Exact accuracy values are not included here because the numerical results were not provided in the project description.

## ✅ Conclusion

This project demonstrates the application of deep learning to fashion image classification. By implementing and comparing ANN and CNN architectures, it explores how convolutional layers, batch normalization, and dropout can be used to build image classification models.

The evaluation process provides insights into model performance and classification errors.

## 🚀 Future Improvements

- Separate validation data from the test dataset for a more reliable final evaluation.
- Tune hyperparameters to improve classification performance.
- Experiment with data augmentation.
- Evaluate precision, recall, and F1-score for each class.
- Explore transfer learning with pretrained image classification models.

## 👩‍💻 Author

**Nandini Gupta**

- GitHub: [nandini17404](https://github.com/nandini17404)
- LinkedIn: [Nandini Gupta](https://www.linkedin.com/in/nandini-gupta-976aab275/)
