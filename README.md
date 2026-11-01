# Rice Leaf Disease Detection

## Project Overview

This project focuses on detecting and classifying diseases in rice leaves using deep learning and computer vision techniques.

The objective is to classify rice leaf images into disease categories, helping demonstrate how machine learning can support agricultural disease identification.

The project explores two approaches:

* Convolutional Neural Network (CNN)
* MobileNetV2 Transfer Learning

## Objectives

* Explore and prepare rice leaf image data.
* Apply image preprocessing and data augmentation.
* Build a CNN image classification model.
* Implement transfer learning using MobileNetV2.
* Evaluate model performance using a confusion matrix and classification report.

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Project Structure

```text
rice-leaf-disease-detection/
│
├── RiceLeaf.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Models Used

### 1. CNN

A custom Convolutional Neural Network is implemented using:

* Convolutional layers
* Max pooling
* Fully connected layers
* Dropout

The model uses a softmax output layer for multi-class classification.

### 2. MobileNetV2

MobileNetV2 is used as a transfer learning model with ImageNet pretrained weights.

The architecture includes:

* MobileNetV2 feature extraction
* Global average pooling
* Dense classification layer

## Data Preprocessing

The notebook uses:

* Image resizing to 224 × 224 pixels
* Pixel normalization
* Image augmentation
* Training and validation split

Augmentation techniques include rotation, zoom, width and height shifts, and horizontal flipping.

## Dataset

The notebook expects a rice leaf image dataset organized into class-specific folders.

The original notebook uses a Google Drive path:

```python
dataset_path = '/content/drive/MyDrive/Rice leaf/Data'
```

To run the notebook, update this path to the location of your dataset.

The dataset is not included in this repository. Obtain it from the original source and follow its license and redistribution requirements.

## Model Evaluation

The notebook evaluates predictions using:

* Confusion matrix
* Classification report
* Precision
* Recall
* F1-score

Refer to the notebook outputs for the actual model results.

## Challenges

The notebook discusses challenges including:

* Limited dataset size
* Overfitting
* Data augmentation
* Model generalization

## Future Improvements

* Increase the diversity of training images.
* Apply hyperparameter tuning.
* Compare CNN and MobileNetV2 performance.
* Improve generalization on unseen rice leaf images.
* Develop a web application for image-based disease prediction.

## Author

Faizan Ali
