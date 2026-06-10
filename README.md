# Fashion Image Categorization using CNN

A Deep Learning project that classifies fashion product images into one of ten clothing categories using a Convolutional Neural Network (CNN) built with TensorFlow and Keras.

## Project Overview

Fashion image classification is a fundamental Computer Vision task where a model learns to identify clothing categories from images. This project uses the Fashion-MNIST dataset and a Convolutional Neural Network (CNN) to automatically categorize fashion products with high accuracy.

The model is trained on grayscale images of clothing items and can predict the correct category for unseen images.

---

## Features

- Uses the Fashion-MNIST dataset
- Image preprocessing and normalization
- CNN-based image classification
- Training and validation performance monitoring
- Accuracy and loss visualization
- Confusion Matrix generation
- Classification Report with Precision, Recall, and F1-Score
- Prediction on test images

---

## Dataset

The project uses the Fashion-MNIST dataset provided by TensorFlow.

### Dataset Statistics

| Dataset | Images |
|----------|---------|
| Training Set | 60,000 |
| Test Set | 10,000 |
| Total Images | 70,000 |

### Categories

| Label | Class |
|---------|---------|
| 0 | T-shirt/Top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle Boot |

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Google Colab / Jupyter Notebook

---

## CNN Architecture

```text
Input (28×28×1)
      ↓
Conv2D (32, ReLU)
      ↓
MaxPooling2D
      ↓
Conv2D (64, ReLU)
      ↓
MaxPooling2D
      ↓
Flatten
      ↓
Dense (128, ReLU)
      ↓
Dropout (0.3)
      ↓
Dense (10, Softmax)
```
## Model Highlights
Two Convolutional Layers for feature extraction
Max Pooling Layers for dimensionality reduction
Dropout Layer to reduce overfitting
Softmax Output Layer for multi-class classification
Data Preprocessing

## The following preprocessing steps are performed:

Load Fashion-MNIST dataset
Normalize pixel values from 0–255 to 0–1
Reshape images to:
(28, 28, 1)
Split data into training and testing sets
Training Configuration
Optimizer : Adam
Loss Function : Sparse Categorical Crossentropy
Epochs : 10
Validation Split : 20%
Metrics : Accuracy

## Project Workflow

```text
Load Dataset
      ↓
Normalize Images
      ↓
Reshape Data
      ↓
Build CNN Model
      ↓
Compile Model
      ↓
Train Model
      ↓
Evaluate Model
      ↓
Generate Predictions
      ↓
Visualize Results
Evaluation Metrics
```

## The model performance is evaluated using:

- Test Accuracy
- Training Accuracy
- Validation Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-Score
- Visualizations

## The project generates:

- Accuracy Curve
- Training Accuracy
- Validation Accuracy
- Loss Curve
- Training Loss
- Validation Loss
- Confusion Matrix

Visual representation of classification performance across all categories.

## Displays:

- Actual Label
- Predicted Label
- Installation

## Clone the Repository
git clone https://github.com/RadhaKrishna-02/Fashion-Image-Categorization.git

cd Fashion-Image-Categorization
Install Dependencies
pip install tensorflow numpy matplotlib seaborn scikit-learn

## Running the Project
Using Google Colab
Open Main.ipynb
Enable GPU:
Runtime → Change Runtime Type → GPU
Run all cells
Using Jupyter Notebook
jupyter notebook

Open:

Main.ipynb

and execute all cells sequentially.

Learning Outcomes

## This project demonstrates:

- Deep Learning Fundamentals
- Convolutional Neural Networks (CNNs)
- Image Classification Techniques
- Model Evaluation and Visualization
- TensorFlow/Keras Implementation
