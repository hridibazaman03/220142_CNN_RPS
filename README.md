# 220142_CNN_RPS

# Rock-Paper-Scissors Image Classification Using CNN

## Student Information

* **Student ID:** 220142
* **Course:** Machine Learning Lab
* **Project:** Assignment 8 – CNN Image Classification
* **Dataset:** Rock-Paper-Scissors

## Project Description

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify hand gestures into three categories:

1. Rock
2. Paper
3. Scissors

The model is trained using a standard Rock-Paper-Scissors image dataset. After training, the model is tested on 10 custom smartphone photographs of hand gestures.

## Technologies Used

* Python
* PyTorch
* Torchvision
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab
* GitHub
* PIL

## CNN Architecture

The CNN consists of:

* Three convolutional layers
* ReLU activation functions
* Max pooling layers
* Adaptive average pooling
* Fully connected layers
* Dropout
* Three output classes

### Data Preprocessing

The images are:

1. Resized to 128 × 128 pixels
2. Converted to RGB
3. Converted to PyTorch tensors
4. Normalized using mean = [0.5, 0.5, 0.5] and standard deviation = [0.5, 0.5, 0.5]

Data augmentation is also applied to the training images using random horizontal flipping and rotation.

## Training

The model uses:

* **Loss Function:** CrossEntropyLoss
* **Optimizer:** Adam
* **Learning Rate:** 0.001
* **Batch Size:** 64
* **Epochs:** 10

## Evaluation

The project evaluates the model using:

* Training loss
* Validation loss
* Training accuracy
* Validation accuracy
* Standard test-set accuracy
* Confusion matrix
* Visual error analysis

## Custom Smartphone Testing

Ten custom smartphone images were collected:

* Rock: 3 images
* Paper: 3 images
* Scissors: 4 images

The custom images are automatically downloaded from this GitHub repository when the Google Colab notebook runs.

The model predicts the class and confidence score for every custom image.

## Results

The notebook generates:

* Training and validation loss graph
* Training and validation accuracy graph
* Confusion matrix
* Three incorrectly classified test images
* Custom image prediction gallery
* Prediction confidence scores

## Reproducibility

The Google Colab notebook automatically:

1. Clones this GitHub repository
2. Downloads the standard RPS dataset
3. Preprocesses the images
4. Builds the CNN
5. Trains the model
6. Evaluates the model
7. Loads the custom smartphone images
8. Predicts Rock, Paper, or Scissors
9. Displays confidence scores

No manual image upload is required during notebook execution.

## Repository Structure

```text
220142_CNN_RPS/
│
├── dataset/
│   ├── rock1.jpg
│   ├── rock2.jpg
│   ├── rock3.jpg
│   ├── paper1.jpg
│   ├── paper2.jpg
│   ├── paper3.jpg
│   ├── scissors1.jpg
│   ├── scissors2.jpg
│   ├── scissors3.jpg
│   └── scissors4.jpg
│
├── model/
│   └── 220142.pth
│
├── 220142_CNN_RPS.ipynb
│
└── README.md
```
